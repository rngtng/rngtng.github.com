---
id: 131
title: RainbowDuino here it is! (and how to program it)
date: '2009-06-25 11:32:50 +0000'
permalink: "/2009/06/25/rainbowduino-here-it-is-and-how-to-program-it/"
layout: post
categories:
- Arduino & Co.
tags:
- Arduino
- RainbowDuino
- program
- uart
- mtXcontrol
comments:
- id: 55
  author: charlie from LOST
  author_email: astralk@hotmail.com
  author_url: ''
  date: '2009-09-25 17:03:04 +0000'
  date_gmt: '2009-09-25 16:03:04 +0000'
  content: "hi,\r\n\r\nAm I supposed to use the reset that's next to the 5v and ground?"
- id: 56
  author: tobi
  author_email: t.bielohlawek@gmail.com
  author_url: http://
  date: '2009-09-25 17:10:52 +0000'
  date_gmt: '2009-09-25 16:10:52 +0000'
  content: Ehm yes! And make sure to have a blank sketch uploaded on the (master)
    arduino...
- id: 57
  author: outstanda
  author_email: outstanda@gmail.com
  author_url: ''
  date: '2009-09-28 13:51:20 +0000'
  date_gmt: '2009-09-28 12:51:20 +0000'
  content: "hello, i see on your youtube page some editor program for the rainbowduino...
    can you share it with an another curious (and newbie) rainbowduino user ? :)\r\n\r\nthanks"
- id: 58
  author: tobi
  author_email: t.bielohlawek@gmail.com
  author_url: http://
  date: '2009-09-28 14:14:03 +0000'
  date_gmt: '2009-09-28 13:14:03 +0000'
  content: yes I'll post it soon here! It's not yet fully finished and ready to publish,
    but I'm working hard on it! For sure it'll be OS and free for download, more on
    this soon - so stay tuned!
- id: 61
  author: tobi
  author_email: t.bielohlawek@gmail.com
  author_url: http://
  date: '2009-10-07 10:57:13 +0000'
  date_gmt: '2009-10-07 09:57:13 +0000'
  content: Alright, it's published, please see http://www.rngtng.com/mtxcontrol/ for
    more!
- id: 68
  author: LD
  author_email: ldunand@gmail.com
  author_url: ''
  date: '2009-10-24 22:59:01 +0000'
  date_gmt: '2009-10-24 21:59:01 +0000'
  content: "Hi I loaded both Firmware and Processing code.\r\nUploading of Firmware
    seems fine -> Rainbowduino started to show random patterns\r\nFor connection with
    processing I changed the serial port (as mine shows up second in the list). But
    the rainbowduino seems to not do anything when recieving Mxt Controls.\r\n\r\nAny
    ideas?"
- id: 69
  author: tobi
  author_email: t.bielohlawek@gmail.com
  author_url: http://
  date: '2009-10-25 02:28:27 +0000'
  date_gmt: '2009-10-25 01:28:27 +0000'
  content: 'hm did you use the latest one? Please try 1.02, you''ll find it here:  http://github.com/rngtng/mtXcontrol/downloads'
- id: 70
  author: the noob
  author_email: andreaandrandy@sympatico.ca
  author_url: ''
  date: '2009-10-25 02:41:21 +0000'
  date_gmt: '2009-10-25 01:41:21 +0000'
  content: "I'm a noob, do you think one day you'll put together a \"how to for noobs\"
    read me file on how to get it up and running?\r\n\r\nbtw way awesome job and the
    youtube clip with the accelerometer looks pretty cool!"
- id: 72
  author: Tony
  author_email: tony@jongra.com
  author_url: ''
  date: '2009-10-26 19:38:58 +0000'
  date_gmt: '2009-10-26 17:38:58 +0000'
  content: "Hi,\r\n\r\nWhen I attach my rainbowduino to my arduino mega with only
    the 5v and gnd, I only see red LEDs on my matrix. When I attach the power supply
    to the rainbowduino, I see the sample sketch. I tried flipping the switch on there
    but I don't know what I'm doing wrong."
- id: 73
  author: mistake
  author_email: mistake@sandiego.de
  author_url: http://markus.jabs.name
  date: '2009-10-29 09:07:54 +0000'
  date_gmt: '2009-10-29 08:07:54 +0000'
  content: "Hi Tobi,\r\nich h&auml;nge leider schon beim Programmieren des Rainbowduinos
    mit Deiner Firmware &uuml;ber einen Arduino. Ich denke, ich habe die beiden korrekt
    miteinander verkn&uuml;pft (5 Kabel), in meiner IDE habe ich den Duemilanove mit
    atmega168 aus gew&auml;hlt - aber ich bekomme alle Nase lang nur dusellige Fehlermeldungen
    (protocol error, expect=0x14, resp=0x51).\r\nHast Du auf Anhieb eine Idee?"
- id: 74
  author: tobi
  author_email: t.bielohlawek@gmail.com
  author_url: http://
  date: '2009-10-29 10:06:51 +0000'
  date_gmt: '2009-10-29 09:06:51 +0000'
  content: "Hey mistake, i just updated the blog post, I think I forgot to mention
    to upload a blank sketch onto the Arduino first. ;-)\r\nAnd make sure that DTR
    on Rainbowduino is connected to Reset on Arduino. Does this work?"
- id: 75
  author: mistake
  author_email: mistake@sandiego.de
  author_url: http://markus.jabs.name
  date: '2009-10-29 10:29:40 +0000'
  date_gmt: '2009-10-29 09:29:40 +0000'
  content: "Ok, I'll try it in english ;)\r\nI already found the part with the blank
    sketch somewhere on the net - but I'm afraid the blank sketch I chose was just
    a little bit blanker than the one you showed above ;) :(\r\nI hope this was the
    simple reason for failing, as the DTR and the Reset-Line were connected.\r\nI'm
    @work right now - I'll try it in a few hours.\r\nThanks :)"
- id: 76
  author: mistake
  author_email: mistake@sandiego.de
  author_url: http://markus.jabs.name
  date: '2009-10-29 13:36:59 +0000'
  date_gmt: '2009-10-29 12:36:59 +0000'
  content: "Update. Just one step ahead.\r\nI uploaded the blank sketch. success.\r\nI
    uploaded your firmware. success.\r\nAt least I guess success, because:\r\nI removed
    VCC, GND and Reset, instead I used an external 9v battery. I started mtxcontrol,
    the rx & tx-leds on the arduino are blinking - but nothing's happening on
    the rainbowduino. :(\r\nI'm going to try again after 4:30 pm..."
- id: 77
  author: tobi
  author_email: t.bielohlawek@gmail.com
  author_url: http://
  date: '2009-10-29 13:46:58 +0000'
  date_gmt: '2009-10-29 12:46:58 +0000'
  content: "cool congrats! Well by default mtXcontrol runs in Free mode, so Rainbowduino
    doesn't show the frames at all, until you click the 2nd top right Button saying
    'MATRIX: Free' or hit alt+ENTER. This puts Rainbowduino in Slave mode and displays
    1:1 what you're doing with mtXcontrol. Maybe I should make this the default option..\r\n\r\nah
    yes, and english please as we have a lot of international readers... ;-) and nice
    Blog btw."
- id: 78
  author: mistake
  author_email: mistake@sandiego.de
  author_url: http://markus.jabs.name
  date: '2009-10-29 14:01:03 +0000'
  date_gmt: '2009-10-29 13:01:03 +0000'
  content: "Thank you, particularly for your help and your compliment :)\r\nThe last
    thing I tried in my break was changing the free/slave-mode - the blinking rx/tx
    started on the arduino, nothing was blinking on the rainbowduino. But as I mentioned
    already: just about 3 hours and I'll try on ;)"
- id: 79
  author: mistake
  author_email: mistake@sandiego.de
  author_url: http://markus.jabs.name
  date: '2009-10-29 17:52:30 +0000'
  date_gmt: '2009-10-29 16:52:30 +0000'
  content: "Still no luck... I've checked that uploading the firmware to the rainbowduino
    now works fine by uploading the original data from seeedstudio again - all leds
    lit up. After that I uploaded your firmware again, started the editor - the tx/rx-leds
    of the arduino reacted (after setting the slave mode, of course), but not the
    rainbowduino.\r\nAny idea now?"
- id: 80
  author: tobi
  author_email: t.bielohlawek@gmail.com
  author_url: http://
  date: '2009-10-29 22:50:31 +0000'
  date_gmt: '2009-10-29 21:50:31 +0000'
  content: "@mistake: I've send you an email with detailed questions/tasks which may
    track the problem down.."
- id: 81
  author: mistake
  author_email: mistake@sandiego.de
  author_url: http://markus.jabs.name
  date: '2009-10-30 20:50:30 +0000'
  date_gmt: '2009-10-30 19:50:30 +0000'
  content: "Interesting. I discovered, that my leds weren't as bright as they should
    be - and now I know why:\r\nI used VCC and GND right next to TX and RX on the
    rainbowduino... Now that I've changed to the green terminal connector and switched
    the switch, it's shining as bright as before when I used an 9V battery on the
    JST jack...\r\nThank you for you're great getting you're great piece of software
    running :)"
- id: 82
  author: Dave Menninger
  author_email: dave.menninger@gmail.com
  author_url: http://davemenninger.blogspot.com/
  date: '2009-11-03 02:55:31 +0000'
  date_gmt: '2009-11-03 01:55:31 +0000'
  content: I'm getting "programmer is not responding" in the arduino IDE when I try
    to upload.  Which Board did you choose under the Board menu?
- id: 83
  author: Dave Menninger
  author_email: dave.menninger@gmail.com
  author_url: http://davemenninger.blogspot.com/
  date: '2009-11-03 03:28:24 +0000'
  date_gmt: '2009-11-03 02:28:24 +0000'
  content: I got it to work by taking the atmega out of my arduino!
- id: 84
  author: Tony
  author_email: tony@jongra.com
  author_url: ''
  date: '2009-11-03 07:32:06 +0000'
  date_gmt: '2009-11-03 05:32:06 +0000'
  content: "When I upload the firmware using the Arduino IDE the matrix goes all white.
    Is that what it's supposed to do? Do I need to run something in Processing also?
    Or just upload the firmware and rum mtxcontrol?\r\n\r\nThanks!"
- id: 85
  author: Tony
  author_email: tony@jongra.com
  author_url: ''
  date: '2009-11-03 08:08:08 +0000'
  date_gmt: '2009-11-03 06:08:08 +0000'
  content: Which .pde files to I upload to rainbowduino? What are all of the rest
    of them for? Do I just upload the firmware and then launch mtxcontrol application?
- id: 86
  author: tobi
  author_email: t.bielohlawek@gmail.com
  author_url: http://
  date: '2009-11-03 10:02:52 +0000'
  date_gmt: '2009-11-03 09:02:52 +0000'
  content: "@Dave: well to upload the sketch on the Arduino choose ATmega 328 (first
    item from the IDE Board menu), for upload on Rainbowduino it's ATmega 168\r\n\r\n@Tony:
    Start the Processing IDE and load the mtXcontrol.pde and run it. (Don't get confused,
    this will load all other files as well.) For the firmware, open Arduino IDE, load
    firmware.pde and upload it to your rainbowduino. By default, the firmware loads
    it's data from EEPROM. If you've never used it before it's likely that each byte
    has 255 as value which would result in a white screen - seems allright!"
- id: 88
  author: Tony
  author_email: tony@jongra.com
  author_url: ''
  date: '2009-11-03 18:34:03 +0000'
  date_gmt: '2009-11-03 16:34:03 +0000'
  content: Thanks... What about the mtxcontrol standalone application? Where do I
    use that?
- id: 89
  author: tobi
  author_email: t.bielohlawek@gmail.com
  author_url: http://
  date: '2009-11-03 18:36:00 +0000'
  date_gmt: '2009-11-03 17:36:00 +0000'
  content: hehe well actually the standalone app should replace the need of using
    processing IDE and loading the mtXcontrol.pde file, but users reported the standalone
    doesn't work for some reasons. Maybe give it a try and tell me if it works for
    you..
- id: 90
  author: Tony
  author_email: tony@jongra.com
  author_url: ''
  date: '2009-11-03 19:10:07 +0000'
  date_gmt: '2009-11-03 17:10:07 +0000'
  content: I got it working. When you open the .pde file with Processing it alerts
    you that you need to move it to it's own folder. So you have to say continue,
    and then put all of the other files besides the firmware folder inside the new
    mtxcontrol folder. Then it started working just fine! Thanks!
- id: 91
  author: Tony
  author_email: tony@jongra.com
  author_url: ''
  date: '2009-11-03 19:12:36 +0000'
  date_gmt: '2009-11-03 17:12:36 +0000'
  content: Also how do you type letters and numbers like in the video?
- id: 92
  author: Tony
  author_email: tony@jongra.com
  author_url: ''
  date: '2009-11-03 21:54:31 +0000'
  date_gmt: '2009-11-03 19:54:31 +0000'
  content: Nevermind! I should have read that you h0ld down Ctrl
- id: 100
  author: Jose
  author_email: as3580094@sapo.pt
  author_url: ''
  date: '2009-11-06 17:13:41 +0000'
  date_gmt: '2009-11-06 16:13:41 +0000'
  content: "Hi,\r\nI try to use your standalone application (.exe) but I wasn&acute;t
    sucessfull.\r\n\r\nLater I found another project in seeestudio (Raindrops) that
    uses your library \r\nRainbowduino.h. I upload it with success and I begin to
    understand the code (I don&acute;t know \r\nto much about C language.\r\n\r\nAfter
    run my arduino connected to rainbowduino it begin to work ok (I&acute;dont have
    \r\nthe accelometer module, but for this porpose I think it is not necessary).\r\n\r\nBut
    there is a problem the LEDs are flickerin, I don&acute;t have a stable image.
    \r\n&Icirc; know that in the game the lines are scrooling, but even after changing
    the code a little for\r\ndisplaing some LED in one line I have the same behabiour.\r\n\r\nIs
    this normal ??"
- id: 101
  author: LD
  author_email: ldunand@gmail.com
  author_url: ''
  date: '2009-11-09 22:33:51 +0000'
  date_gmt: '2009-11-09 21:33:51 +0000'
  content: "Hi tobi,\r\n\r\nWorks fine with 1.02. Great Job!\r\n\r\nThanks"
- id: 102
  author: Ross D
  author_email: rngtng@the-dargans.co.uk
  author_url: ''
  date: '2009-11-11 23:34:01 +0000'
  date_gmt: '2009-11-11 22:34:01 +0000'
  content: "Ok, this program looks fab! I have all the hardware and the mtXcontrol
    downloaded... but I can't find the firmware anywhere. Do I need to upload something
    to the rainbowduino, or to the arduino? If so could you tell me where I can get
    them files.\r\n\r\nHoping to build something on Friday with this - looks good!\r\n\r\nThanks\r\n\r\nRoss"
- id: 103
  author: tobi
  author_email: t.bielohlawek@gmail.com
  author_url: http://
  date: '2009-11-12 09:50:40 +0000'
  date_gmt: '2009-11-12 08:50:40 +0000'
  content: 'hey Ross, you have to get the firmware from source, find it here: http://github.com/rngtng/mtXcontrol/tree/master/firmware/'
- id: 366
  author: Rene
  author_email: client@renehagen.nl
  author_url: ''
  date: '2009-12-17 20:51:06 +0000'
  date_gmt: '2009-12-17 19:51:06 +0000'
  content: Very nice. Thanks!
- id: 372
  author: Rene
  author_email: client@renehagen.nl
  author_url: ''
  date: '2009-12-18 12:40:40 +0000'
  date_gmt: '2009-12-18 11:40:40 +0000'
  content: "Hi,\r\n\r\nIs there a way to control the brightness of the leds? They
    are to bright for my application."
- id: 373
  author: tobi
  author_email: t.bielohlawek@gmail.com
  author_url: http://
  date: '2009-12-18 12:54:57 +0000'
  date_gmt: '2009-12-18 11:54:57 +0000'
  content: Hey Rene, unfortunately, by now, there's nothing like this... but it's
    on my todo list, stay tuned ;-)
- id: 413
  author: DeFex
  author_email: d_fex@sympatico.ca
  author_url: http://neutron-sound.blogspot.com/
  date: '2010-01-16 03:47:53 +0000'
  date_gmt: '2010-01-16 02:47:53 +0000'
  content: "Hello, thank you for posting this.\r\n\r\nIt was very helpful for me,
    I programmed the rainbowduino with the test plasma sketch \"through\" a arduino
    mega. the only thing that confused me was that\r\nAfter loading the blank sketch
    with the IDE set to \"mega\" and connecting the rainbowduino,\r\nI had to switch
    the IDE to an \"diecimila duemilanove or nano atmega168\" arduino to program the
    rainbow through the arduino mega serial.\r\n\r\nIf you are using an arduino other
    than diecimila duemilanove or nano you will probably have to change it or you
    will get a avrdude serial error.\r\n\r\nonce that happens you cant reprogram the
    arduino either unless you press the reset while reconnecting the usb/power"
- id: 415
  author: tobi
  author_email: t.bielohlawek@gmail.com
  author_url: http://
  date: '2010-01-16 14:31:03 +0000'
  date_gmt: '2010-01-16 13:31:03 +0000'
  content: hm I havn't tried the Arduino mega yet. But as far I've heard there're
    no differences in way how to program the controller..
- id: 417
  author: Taras Slawnych
  author_email: tslawnych@thestar.ca
  author_url: http://www.lightfromastone.com
  date: '2010-01-18 03:57:55 +0000'
  date_gmt: '2010-01-18 01:57:55 +0000'
  content: "Hi tobi\r\n\r\nI can't get the mtxcontrol to work, I've connected my seeduino
    mega to the rainbowduino, loaded the blank code and then loaded the firmware code.
    When I launch the mtxcontrol the program doesn't work, nothing displays, no grid,
    no buttons, nothing.  Have you changed the program, I noticed you recently did
    a upgrade\r\n\r\nThanks"
- id: 418
  author: tobi
  author_email: t.bielohlawek@gmail.com
  author_url: http://
  date: '2010-01-18 13:51:11 +0000'
  date_gmt: '2010-01-18 11:51:11 +0000'
  content: what OS are you using? please get the source code from github and run mtXcontrol
    within the processing IDE. What errors do you get?
- id: 419
  author: Taras Slawnych
  author_email: tslawnych@thestar.ca
  author_url: http://www.lightfromastone.com
  date: '2010-01-19 00:10:19 +0000'
  date_gmt: '2010-01-18 22:10:19 +0000'
  content: "I'm running 10.5.8 when I run mtxcontrol nothing comes up. I'll email
    a link for a short video tonight.\r\n\r\nThanks T"
- id: 420
  author: Taras Slawnych
  author_email: tslawnych@thestar.ca
  author_url: http://www.lightfromastone.com
  date: '2010-01-19 00:18:10 +0000'
  date_gmt: '2010-01-18 22:18:10 +0000'
  content: "This is the link I used to download the zip file for my Mac. Do I need
    any other files?\r\n\r\nT"
- id: 421
  author: Taras Slawnych
  author_email: tslawnych@thestar.ca
  author_url: http://www.lightfromastone.com
  date: '2010-01-19 02:45:01 +0000'
  date_gmt: '2010-01-19 00:45:01 +0000'
  content: "Here's a link to my short video \r\n\r\nhttp://screencast.com/t/YWZjYjlh\r\n\r\nThanks
    T"
- id: 423
  author: Ola
  author_email: ola.benderius@hotmail.com
  author_url: ''
  date: '2010-01-21 19:11:10 +0000'
  date_gmt: '2010-01-21 17:11:10 +0000'
  content: "Hi!\r\n\r\nI have problems loading the firmware to my Rainbowduino. I
    uploaded the blank sketch to my Duemilanove (168) as usual.\r\nBut when I then
    try to upload the firmware I get a \"protocol error\" just like someone mentioned
    above. I checked the connections and re-uploaded the empty sketch. It never works.
    At some point the default rainbow-pattern stopped working so I guess something
    was uploaded. Can the Rainbowduino get corrupt?\r\n\r\nI have the board \"Arduino
    Diecimila, Duemilanove, or Nano w/ ATmega168\" selected all the time.\r\n\r\nThanks!\r\n/Ola"
- id: 446
  author: king levi
  author_email: king02levi2004@yahoo.ca
  author_url: ''
  date: '2010-01-27 07:32:28 +0000'
  date_gmt: '2010-01-27 05:32:28 +0000'
  content: i finaly receive the rainbow ard. i am new to this i followed you instructions
    but anly got the full white lights the Mtx controler does not reconise the board
    it gives me this ( no output device found running in standalone mode) please can
    somewon tell me what am i doing wrong
- id: 447
  author: tobi
  author_email: t.bielohlawek@gmail.com
  author_url: http://
  date: '2010-01-27 11:20:35 +0000'
  date_gmt: '2010-01-27 09:20:35 +0000'
  content: Hey Ola! Apparently this uploading trick doesn't work if your host arduino
    is a ATmega168 as well, you need an ATmega328 as 'host' to pass serial communication
    through...
- id: 449
  author: king levi
  author_email: king02levi2004@yahoo.ca
  author_url: ''
  date: '2010-01-27 23:05:07 +0000'
  date_gmt: '2010-01-27 21:05:07 +0000'
  content: i looks like onley a rocket sintinces can get these things to work my advice
    to aneyon dont buy this its garbage
- id: 450
  author: king levi
  author_email: king02levi2004@yahoo.ca
  author_url: ''
  date: '2010-01-27 23:13:05 +0000'
  date_gmt: '2010-01-27 21:13:05 +0000'
  content: i am sorer about that coment but after trying every thing it stil dosent
    work yes ihave a ATMega328 just like the one in your picture
- id: 454
  author: tobi
  author_email: t.bielohlawek@gmail.com
  author_url: http://
  date: '2010-01-28 13:17:26 +0000'
  date_gmt: '2010-01-28 11:17:26 +0000'
  content: hey levi, no worries rocket science is fun ;-) what mtXcontrol Version
    are you using, which OS (mac, win, linux - version number)? if rainbwoduino turned
    white, connection should be all fine..
- id: 455
  author: DatManChris
  author_email: chris.loxton@mclaren.com
  author_url: ''
  date: '2010-01-29 00:52:36 +0000'
  date_gmt: '2010-01-28 22:52:36 +0000'
  content: "Well I got mine tuesday and had it running in an evening. \r\nIf you can
    take the 168 / 328 out then that seems to help.\r\nIt works really well but wish
    that you could send it a longer stream from processing. \r\nI want to set up say
    8 in a row and use it as a scrolling message display.\r\nMy idea is to send 1
    row at a time from processing to the first rainbowduino via serial RX and as it
    reaches row 8, shunt that row using the serial TX to the the second and so on.
    \r\nIf I could just get to the bottom of how the source code works then I'b be
    half way there...\r\nI've built an analog clock using 480 RGB led's in 7 8*8 and
    1 4*8 matrix's and It would be really nice to scroll a message round the face.\r\nIf
    you release another version of the source code, Can you put a few more comments
    in to help us not so hardcore programers a chance???\r\n\r\nGreat work and the
    Rainbowduino wouldn't be half the product without mtXcontrol..."
- id: 456
  author: king levi
  author_email: king02levi2004@yahoo.ca
  author_url: ''
  date: '2010-01-29 02:50:56 +0000'
  date_gmt: '2010-01-29 00:50:56 +0000'
  content: hi thanks   i am using   windows vista 64  yes i do get the all white screne  i
    dont understand the part about the processing yes i did down load the  processer  but
    do ihave to load the  xtxcon. to the processor or to the original ard. prosser.
- id: 457
  author: king levi
  author_email: king02levi2004@yahoo.ca
  author_url: ''
  date: '2010-01-29 03:10:59 +0000'
  date_gmt: '2010-01-29 01:10:59 +0000'
  content: "thanks  TOBI  Iam shure i have the wright  mtx  the part idont understand
    is\r\ne. Using the Arduino IDE, load the firmware.pde sketch and then transfer
    it."
- id: 459
  author: KING LEVI
  author_email: KING02LEVI2004@YAHOO.CA
  author_url: ''
  date: '2010-02-01 00:23:30 +0000'
  date_gmt: '2010-01-31 22:23:30 +0000'
  content: "FINALY GOT SOME LIFE OUT OF  THE RAINBODU STILL CANT USE THE  MTX CONT.BUT
    THE LINK AND THE RAINROW WORKS  THE ONLY THING IT RUNS IS #include \"Rainbowduino.h\"\r\n#include
    \"RCodes.h\" //API Cod  DO YOU HAVE ENY SUGESTION ON WHAT I DONT UNDERST OR IAM
    DOING WRONG. THANKS AND GOD BLESS"
- id: 524
  author: xphere
  author_email: xpherezn@gmail.com
  author_url: http://www.xphere.me
  date: '2010-05-13 21:49:24 +0000'
  date_gmt: '2010-05-13 19:49:24 +0000'
  content: |-
    Hi!!

    I've tried but it does not work for me... what I do is the following:
    1- Connect Arduino (328) with Rainbowduino as your connections (tx-tx, rx-rx)
    2- Upload the blank sketch to the 328 arduino
    3- Change the Board to "Arduino Diecimila, Duemilanove or nano Atmega/168" and upload the firmware.pde
    At this point, the upload is not succesful and I get the error: "avrdude: stk500_recv(): programmer is not responding"

    Any idea?


    Thanks in advance,
    xphere.
- id: 526
  author: xphere
  author_email: xpherezn@gmail.com
  author_url: http://www.xphere.me
  date: '2010-05-17 22:08:50 +0000'
  date_gmt: '2010-05-17 20:08:50 +0000'
  content: now it works! and error from my side... sorry!
- id: 527
  author: Rainbowduino&#8230; a virus in my Arduino!
  author_email: ''
  author_url: http://xphere.me/2010/05/rainbowduino-a-virus-in-my-arduino/
  date: '2010-05-17 22:17:54 +0000'
  date_gmt: '2010-05-17 20:17:54 +0000'
  content: "[...] rainbowduino cannot be connected via USB, as Arduino does), after
    1min search in google, I found&nbsp;this post, with good instructions about how
    to use Arduino as a host for programming it. In the same page, [...]"
- id: 532
  author: al
  author_email: alinke@yahoo.com
  author_url: ''
  date: '2010-06-28 04:49:40 +0000'
  date_gmt: '2010-06-28 02:49:40 +0000'
  content: "Hi sweet looking app. I have a newer Rainbowduino with an Atmel 328\r\n\r\nThe
    blank sketch loads fine on my Arduino 328 but when trying to upload to the Rainbowduino
    (after following the wiring in the blog pic), I get this\r\n\r\ntried both setting
    128 and 328 in the arduino IDE, any ideas?\r\n\r\n\r\navrdude: stk500_paged_write():
    (a) protocol error, expect=0x14, resp=0x64\r\navrdude: failed to write flash memory,
    rc=-4\r\navrdude: stk500_disable(): protocol error, expect=0x14, resp=0x51"
- id: 535
  author: neophob.com &raquo; Rainbowduino fun &#8211; aka neorainbowduino
  author_email: ''
  author_url: http://www.neophob.com/2010/07/rainbowduino-fun-aka-neorainbowduino/
  date: '2010-07-07 12:03:06 +0000'
  date_gmt: '2010-07-07 10:03:06 +0000'
  content: "[...] your Arduino serial ports with the serial port of the Rainbowduino:
    \  (img source) This allows us to flash the Rainbowduino with the Arduino IDE
    (I use Rainbowduinos with an Atmel [...]"
- id: 543
  author: lastcoolnameleft
  author_email: lastcoolnameleft@yahoo.com
  author_url: http://lastcoolnameleft.com
  date: '2010-08-13 06:46:32 +0000'
  date_gmt: '2010-08-13 04:46:32 +0000'
  content: "Al,\r\n\r\nAny luck with your problem?  I'm experiencing a similar issue,
    although I'm unable to even program the blank sketch.\r\n\r\n I have the newer
    Rainbowduino, but cannot program it through my existing Arduino 328.  I have been
    able to program it with the Uarb_SB, but only have one available usb hub and have
    to keep swapping between programming the master and the rainbowduino."
- id: 544
  author: Dave
  author_email: david_a_hanson@msn.com
  author_url: ''
  date: '2010-08-16 09:21:58 +0000'
  date_gmt: '2010-08-16 07:21:58 +0000'
  content: If the Arduino and the Rainbowduino are both 328 you cannot program through
    the Arduino, you will need a usb - uart rs232 board i think.
- id: 546
  author: Rainbowduino mit Arduino verbinden und programmieren &laquo; SUSAY &#8211;
    Design, Technik und Trends
  author_email: ''
  author_url: http://www.susay.de/index.php/rainbowino-mit-arduino-verbinden-und-programmieren/
  date: '2010-08-27 17:39:16 +0000'
  date_gmt: '2010-08-27 15:39:16 +0000'
  content: "[...] hat eine Anleitung auf Englisch geschrieben. Auf dem unteren Foto
    k&ouml;nnt ihr erkennen wie man den Raibowduino mit dem Arduino [...]"
- id: 666
  author: Paul
  author_email: a@a.com
  author_url: ''
  date: '2011-02-22 00:19:30 +0000'
  date_gmt: '2011-02-21 22:19:30 +0000'
  content: "Hi Guys,\r\n\r\nI managed to get my Rainbowduino (328) programmed via
    a seedunio (328).  I experienced the same error stk500_paged_write() ..... when
    following the instruction the way I achived this was todo the reset for the boot
    loader manually.\r\n\r\nHere is what I did.\r\n\r\n1. Connect the RST to GND on
    the seeedunio board (hold chip in reset state)\r\n2. Connect RX,TX,GND and VCC
    (5V) from seeedunio to Rainbowduino\r\n3. Setup arudino IDE read with the firmware.pde
    and 328 board format.\r\n4. Press reset on the Rainbowduino and then quickly press
    the upload button (I think it needs to be under 0.5 seconds).\r\n\r\nThis should
    then download the new firmware to the Rainbowduino board.\r\n\r\nP.S I found that
    I needed to change \r\n#include     ----- >>   #include \"MsTimer2.h\"\r\nin a
    couple of places"
- id: 707
  author: kin37ik
  author_email: dr.grumbles99@hotmail.com
  author_url: ''
  date: '2011-05-08 11:13:23 +0000'
  date_gmt: '2011-05-08 09:13:23 +0000'
  content: ive done exactaly what youve described here but i cannt get mine to work,
    im using an arduino mega 2560 and 2 rianbowduino's, ive tried uploading the MTX
    firmware onto the rainbowduino but the compiler just throws alot of errors and
    doesnt upload it to the rainbowduino at all
- id: 762
  author: ortsac
  author_email: ortsac@pacbell.net
  author_url: ''
  date: '2011-08-16 21:40:13 +0000'
  date_gmt: '2011-08-16 19:40:13 +0000'
  content: "Hi,\r\n\r\nI am using the latest files from, the firmware is dated 8/2/2011
    from the githup site zip file &ldquo;latest_mtxcontro_and_firmware_windows&rdquo;,
    Seeeduino 328, and Windows XP.\r\n\r\nI&rsquo;m new to Rainbowduino&hellip;.I
    was able to successfully the following using the Adruino IDE:\r\n1. Blank the
    Seeeduino Atmega328 (I am using it as a pass a USB-serial comunication to the
    Rainbowduino board.)\r\n2. Upload the &ldquo;Rainbow_Plasma.pde&rdquo; into the
    Rainboeduino and watch it perform in Standalone mode.\r\n3. Blank out the &ldquo;Rainbow_Plasma&rdquo;
    from the Rainbowduino and watch the display turn off.\r\n4. Upload the firmware
    the &ldquo;mtxfirmware.pde&rdquo; into the Rainbowduino and watch it all go white.\r\n\r\nThe
    problem is it seems that the&rdquo;mtXcontrol.exe&rdquo; does not seem to work.
    There is a message at the top of the window that says &ldquo;No output device
    found, running in standalone mode&rdquo;. I do not know what that means and how
    to correct it. Please help!!!!\r\n\r\nortsac"
- id: 916
  author: Chad
  author_email: wsarles@gmail.com
  author_url: ''
  date: '2012-01-16 01:30:28 +0000'
  date_gmt: '2012-01-16 00:30:28 +0000'
  content: Has anyone gotten this to work with v3.0 Rainbowduino hardware?  I can
    successfully flash the Rainbowduino, Mtxcontrol finds the board ok and I see the
    rx/tx lights light up when I send activity to the board, but the lights do not
    light up. The only thing I can get working with this 3.0 board is the included
    examples that come with the stock 3.0 firmware.  Ideas?
- id: 945
  author: Rob Sherratt
  author_email: rob.sherratt@gmail.com
  author_url: http://openstudiolive.com
  date: '2012-01-20 21:19:48 +0000'
  date_gmt: '2012-01-20 20:19:48 +0000'
  content: There is now a RainbowDuino version 3.0 with on-board USB for programming.  You
    no longer have to use a separate Arduino for programming.  http://www.seeedstudio.com/wiki/Rainbowduino_v3.0
- id: 970
  author: Imanuel
  author_email: imanuel.siman@yahoo.co.id
  author_url: ''
  date: '2012-02-28 18:11:11 +0000'
  date_gmt: '2012-02-28 17:11:11 +0000'
  content: |-
    anyone have an example program for scrolling text?
    because I do not understand using rainbowduino to display the letters in an 8x8 RGB LED matrix.
    If you have an example of this program please send to my email: @ yahoo.co.id imanuel.siman
    thank you
- id: 972
  author: markus.jabs.name &raquo; RGB-8&#215;8-LED-Matrix
  author_email: ''
  author_url: http://markus.jabs.name/2009/10/rgb-8x8-led-matrix/
  date: '2012-02-29 13:17:30 +0000'
  date_gmt: '2012-02-29 12:17:30 +0000'
  content: "[...] m&ouml;chte ich hervorheben, dass Tobi auf meinen Kommentar mehr
    als flott geantwortet hat.&nbsp; Ich glaube auch, dass alle Informationen, die
    ich hier [...]"
- id: 1055
  author: Laurence
  author_email: laurencearlidge@hotmail.com
  author_url: ''
  date: '2012-04-20 07:55:13 +0000'
  date_gmt: '2012-04-20 06:55:13 +0000'
  content: Can someone please help me to get my Rainbowduino V3 to work with MTX Control,
    i have uploaded the firmware to the Rainbowduino, no Arduino board needed as the
    new Rainbowduino allows for sketches to be uploaded directly, When i start MTX
    Control, it just says NO DEVICE FOUND, and tryint ALT + ENTER does nothing, i
    am running MACOSX 10.6.8 snow leopard, Please help
- id: 1233
  author: voidnoise.co.uk &raquo; Star Wars glowing mask
  author_email: ''
  author_url: http://voidnoise.co.uk/blog/?p=429
  date: '2012-08-07 15:11:55 +0000'
  date_gmt: '2012-08-07 14:11:55 +0000'
  content: "[...] links; Rainbowduino Manual seedstudio rainbowduino wiki Guide of
    programming Getting started [...]"
- id: 4420
  author: 8&#215;8 RGB LED Display | Mike:Enabled
  author_email: ''
  author_url: http://mikecchin.wordpress.com/2013/08/10/8x8-rgb-led-display/
  date: '2013-08-10 11:51:12 +0000'
  date_gmt: '2013-08-10 10:51:12 +0000'
  content: "[...] http://www.rngtng.com/2009/06/25/rainbowduino-here-it-is-and-how-to-program-it/
    [...]"
- id: 7966
  author: Calvin
  author_email: calvinc307@gmail.com
  author_url: ''
  date: '2013-11-22 05:10:02 +0000'
  date_gmt: '2013-11-22 04:10:02 +0000'
  content: "hey guys, can anybody help with this, I'm almost about to give up, tried
    so many things and I still can't get my arduino to talk via I2C with my Rainbowduino/8x8matrixLED.
    \r\n\r\ni flashed the firmware correctly onto the rainbowduino, but after uploading
    the master code from: \r\n\r\n http://code.google.com/p/rainbowduino-firmware/\r\n\r\n
    to my arduino uno, it doesn't seem to communicate with the rainbowduino w/ 8x8LED
    matrix; no lights at all =(."
- id: 15740
  author: Hoctrimede
  author_email: t.mendoche@yahoo.fr
  author_url: ''
  date: '2014-03-10 16:59:48 +0000'
  date_gmt: '2014-03-10 15:59:48 +0000'
  content: "Hello. Thanks a lot for this nice article.\r\nI'm french, so sorry in
    advance for all my english faults...\r\n\r\nI have two questions :\r\n1. On the
    Arduino (use to pass serial communication through), did you remove the ATm328
    circuit ? I see on the picture that the circuit is on the board.\r\n\r\n2. Concerning
    the connection between Arduino et Rainbow : It's not necessary to cross RX and
    TX connection between Arduino and Rainbow ?\r\n\r\nThanks a lot for your help."
---
![rainbowduino2](/files/2009/06/rainbowduino2.jpg)  
Yay - I finally got my [RainbowDuino](http://www.seeedstudio.com/blog/?p=410). Unluckily I did sth wrong with the external power connection (JST 2 pin jack) and smashed a capacitor. Maybe the polarity was wrong or it couldn't stand the 12 volts? But luckily no damage to the main system so it still works using the terminal connector (right through the 5volts of the Arduino). \*phew\*

The first real basic problem I ran into [was how to program the Rainbowduino](http://www.seeedstudio.com/forum/viewtopic.php?f=4&t=328) as there's no USB connector and I don't have an UART interface.  
[But well, nothing simpler than that:](http://www.seeedstudio.com/blog/?p=420) Just connect your Arduino's Tx,Rx,GND,Reset and Vcc ports with those of the Rainbowduino, choose the right controller type in your IDE and program it as usual - works perfect for me!

Check out my [Rainbowduino Editor mtXcontrol here](/mtXcontrol) - it's an easy way to draw shapes on your rainbowduino!

Btw. _DTR_ on Rainbowduino is _Reset_ on Arduino

**UPDATE:**  
Sorry I forgot to mention, this trick does NOT work if your host arduino is a ATmega168 - you need an ATmega328 to pass serial communication through. Before that, make sure you upload this blank sketch to your host Arduino first:

[code]  
/\* blank sketch to upload on Arduino \*/  
void setup()  
{  
}

void loop()  
{  
}

[/code]

And, as multiple times requested, a picture of my complete setup:  
 ![arduino_rainbowduino](/files/2009/06/arduino_rainbowduino.jpg)

Make sure you've selected the switch right. It has to point to the same side as the green Terminal connectors are. If you power rainbowduino through the white JST jack, flip it!