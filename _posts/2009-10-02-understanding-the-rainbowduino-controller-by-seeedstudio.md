---
id: 188
title: Understanding the Rainbowduino Controller by Seeedstudio
date: '2009-10-02 19:33:04 +0000'
permalink: "/2009/10/02/understanding-the-rainbowduino-controller-by-seeedstudio/"
layout: post
categories:
- Arduino & Co.
tags:
- howto
- Arduino
- seeedstudio
- RainbowDuino
comments:
- id: 380
  author: j4k3
  author_email: andreas.sauer@gmxpro.de
  author_url: ''
  date: '2009-12-19 12:24:55 +0000'
  date_gmt: '2009-12-19 11:24:55 +0000'
  content: "Hi Toby,\r\nich hab gerade &uuml;ber die Youtube-Videos dein Blog gefunden,
    vielleicht kannst du mir ja mit meinem Rainbowduino helfen. Ich hab mir letztes
    Jahr einen Arduino mit ethernet shield zugelegt und viel damit rumgespielt um
    meine Microcontroller-Kenntnisse aufzufrischen. Nach einiger Zeit bin dann auf
    den Rainbowduino gesto&szlig;en und habe mir gleich einen bestellt.\r\n\r\nDie
    Sache mit den farbigen Pixeln war dann aber leider nicht so einfach, wie ich mir
    das vorgestellt habe. Ich war bisher nicht in der Lage, irgendwas damit zum laufen
    zu bekommen, um genau zu sein hab ich erst nach zwei Monaten die Zeit gehabt mir
    das Ding mal so weit an zu sehen, dass ich das Rainbow-Pattern angezeigt bekommen
    habe. Mein Arduino stellt wohl &uuml;ber die Pinouts nicht genug Spannung zur
    verf&uuml;gung oder so oder ich weiss auch nicht. Jedenfalls will das Ding &uuml;berhaupt
    nur dann was anzeigen, wenn ich die Spannung direkt anschliesse.\r\n\r\nAuf dem
    Teil sollte doch im Auslieferungszustand schon ein sketch sein, mit dem man von
    einem Host aus Daten zur Anzeige senden kann, oder? Wie stellt man das denn an?
    Ich habe den seedmaster-sketch in meinen Arduino geladen, aber ich weiss nicht
    mal, wie ich den Rainbowduino anschliessen muss. Stellt man die I2C-Verbindung
    &uuml;ber rx,tx und reset respektive rxd, txd und sda her? Dann m&uuml;sste sich
    doch auf der Matrix was tun, oder?"
- id: 412
  author: Martijn
  author_email: spamtrap@online.nl
  author_url: ''
  date: '2010-01-14 13:27:06 +0000'
  date_gmt: '2010-01-14 12:27:06 +0000'
  content: "Hi Tobi,\r\n\r\nThanks for the informative post.\r\n\r\nSeeedstudio (in
    the Rainbowduino) use three MBI5168 to control the colour channels (one driver
    for each channel) and switch power using Arduino's ports. About this you write
    \"Unfortunately the row pins are not all on one port: rows 1-3 are on PORTB Bit
    1-3, rows 4-8 are on PORTD Bit 4-8. This makes the method kind of bit ugly\".
    I agree ;)\r\n\r\nI am going to build a Rainbowduino clone from scratch for educational
    purposes and now I wonder: would it pose technical difficulties if a fourth MBI5168
    were used to control power? That way, only Arduino's serial input would be required
    to drive the display, freeing a bunch of ports. It might also make adding more
    RGB matrices easier (i.e.: make a 8x16 display)."
- id: 414
  author: tobi
  author_email: t.bielohlawek@gmail.com
  author_url: http://
  date: '2010-01-16 14:29:13 +0000'
  date_gmt: '2010-01-16 13:29:13 +0000'
  content: |-
    Hey Marijn!
    True, I was wondering why they didn't used a forth MBI, too. I think the reason is that you may wouldn't be able to control multiple matrixes with just one rainbowduino having 6bit color support? 16mhz may be just to slow for that!? Please keep me updated on your work, I'm curious which super controller you gonna create ;-)
- id: 1006
  author: jim
  author_email: g0ldmagik@hotmail.co.uk
  author_url: ''
  date: '2012-03-23 14:23:59 +0000'
  date_gmt: '2012-03-23 13:23:59 +0000'
  content: Hi i'm a complete novice at this whole Arduino/Rainbowduino stuff and would
    really appreciate a simple step by step tutorial from the wiring to the coding
    on how to get the rainbowdruino to make any sort of light images.
---
As you may know, I've orderd a [Rainbowduino from Seeedstudio](http://www.seeedstudio.com/blog/?page_id=187). They delivered quite fast and I'm very happy of the price/quality/functionality ratio. In my opinion, the Rainbowduino is the cheapest ready-to-go 8x8 RGB LED Controller Set at the moment - for just 43.4$ ( 19.90$ Board + 23.50$ Matrix) you are set for taking of!

My first tests went quite well. The Rainbowduino comes with a ready to use the program/[sketch](http://www.seeedstudio.com/depot/images/product/RaibowduinoCMD_Bata.rar) which allows you basic controls via I2C bus easily, like writing letters & lines in different color and light strength. But soon I hit the limits when it came so single control each LED to my will. So no doubt, I had to dig deeper in understanding how to control the Rainbowduino. Here a short summery of my results:

To understand how the Rainbowduino works, I kind of reverseengineered the sketch by seeedstudio which came with the controller. As usual for driving those Matrixes, [PWM](http://en.wikipedia.org/wiki/Pulse-width_modulation) is used as basic concept. This means the frame image is created row by row by high frequency, so human eye puts it all together to one single image.

To simplify this process I created the Rainbowduino.h Library, which comes with some nice methods to set frames and draw those to the Rainbowduino. It's part of the mtXcontrol firmware an can be [downloaded from github](http://github.com/rngtng/mtXcontrol/tree/master/firmware/rainbowduino/)

![](http://www.seeedstudio.com/depot/images/product/rainbowblock.jpg)

**How it works:**  
To tell rainbowduino which row to draw the method 'open_row' is called. As each row is represented by a one output PIN, this method sets the according PIN to high, all others to low. Unfortunately the row pins are not all on one port: rows 1-3 are on PORTB Bit 1-3, rows 4-8 are on PORTD Bit 4-8. This makes the method kind of bit ugly ;-)

After the row is selected, its time to set the pixels. One pixel consists of 3 LEDs: red, green & blue. Each LED has to be separately to high or low to mix the final color (e.g. red + green is yellow). First all blue values of a row are set, then red and finally green. This happens in serial on PORTC. First bit is the value input, second bit is clock, bit 3 the write mode bit and bit 4 to display the shifted value. Call the method 'draw_row' to display a row. First parameter is the row number (0-7), second the intensity (1-16) and then the red, blue & green values for the row. e.g passing the color values 1,0,0 would light the first pixel red and all other off, where as 255, 255, 255 would light up all LED and all colors, to the full row would be white.

To store the row values the Library comes with a frame buffer for 10 frames. (That the amount of frames we can store to EEPROM without compression as well). You can pre fill the buffer and set the frame number to display. By calling draw() the frame of the current _frame number is drawn.

It makes sense to call this function by a timer interrupt to not disturb your actual program progress and to ensure it's call in regular frequency to avoid different display colors.

To set up the timer, include this in your code:

[c]  
Rainbowduino rainbow = Rainbowduino(10); //max 10 Frames

void setup_timer() {  
 TCCR2A = 0;  
 TCCR2B = 1\<<cs22></cs22> TIMSK2 = 1\<<toie2></toie2> TCNT2 = 0;  
 sei();  
}

ISR(TIMER2_OVF_vect) {  
 rainbow.draw();  
}  
[/c]

Now, just fill you frames with

[c]  
rainbow.set_frame(0, \*data);  
[/c]

and your're ready to go. Have fun!

First tests of the library with earlier version of [mtXcontrol](/mtXcontrol), an Editor to create images on the Matrix easily:  
<http://www.youtube.com/watch?v=MVj1YPzREKI>

Stay tuned for more examples soon...