---
id: 90
title: 'Arduino: Fade and pulse a LED with just using a DigitalPort'
date: '2009-05-17 14:40:45 +0000'
permalink: "/2009/05/17/arduino-fade-and-pulse-a-led-with-just-using-a-digitalport/"
layout: post
categories:
- Arduino & Co.
tags:
- Arduino & Co.
- led
- fade
- dimm
comments:
- id: 93
  author: J.Martich
  author_email: jmartich1@gmail.com
  author_url: ''
  date: '2009-11-05 03:01:13 +0000'
  date_gmt: '2009-11-05 02:01:13 +0000'
  content: What line would I modify to make the LED completely turn off then fade
    on? Or is that even possible w/ the digital channels? Thanks though this code
    is the shizzle fo rizzle...
- id: 94
  author: tobi
  author_email: t.bielohlawek@gmail.com
  author_url: http://
  date: '2009-11-05 10:36:31 +0000'
  date_gmt: '2009-11-05 09:36:31 +0000'
  content: 'well sure! I admit, this code was first version and is kind of crap, I
    should come up with an updated one. But to solve your problem turing off the LED,
    just change the low/high interval ratio to a maximum of low. Try playing around
    with the values in line 17, e.g. change them into:  blinkl( a+100, 200 - a );'
- id: 405
  author: BiLL
  author_email: bambino_sporos@hotmail.com
  author_url: ''
  date: '2009-12-31 14:50:21 +0000'
  date_gmt: '2009-12-31 13:50:21 +0000'
  content: Nice work m8, im try to do samething for a project for my university. i
    work with pic 18F1320 ( c programming ) . Could u want to send me a code in this
    pic or something like that in order to fix it to work . Im already thank u for
    this idea a read.
- id: 461
  author: jason
  author_email: kintovision@gmail.com
  author_url: ''
  date: '2010-02-12 11:35:29 +0000'
  date_gmt: '2010-02-12 09:35:29 +0000'
  content: What about having one LED fade into another?  For example, a red LED fading
    into a blue LED?
- id: 472
  author: andrewcaveman
  author_email: andrewcaveman@gmail.com
  author_url: http://www.whatiswas.com
  date: '2010-03-10 21:25:38 +0000'
  date_gmt: '2010-03-10 19:25:38 +0000'
  content: "Excellent solution for the digital write. I've been trying to find a good
    solution for button input to LED lights using the analogwrite, but the delay function
    would always null my button input until the loop was complete. This works very
    well. \r\nThanks for giving me new ideas."
- id: 541
  author: MetaCipher
  author_email: tim@metacipher.com
  author_url: http://www.sdltutorials.com
  date: '2010-07-24 17:00:17 +0000'
  date_gmt: '2010-07-24 15:00:17 +0000'
  content: "Simple example, using a shift register - makes all 8 LEDs pulsate together
    (from complete brightness, to nothing):\r\n\r\nint data = 2;\r\nint clock = 3;\r\nint
    latch = 4;\r\n\r\nboolean Pins[8];\r\n\r\nint Count = 0;\r\n\r\nint Brightness
    = 0;\r\nint BrightnessInc = 1;\r\n\r\nvoid setup() {\r\n  pinMode(data, OUTPUT);\r\n
    \ pinMode(clock, OUTPUT);\r\n  pinMode(latch, OUTPUT);\r\n}\r\n\r\nvoid loop()
    {\r\n  digitalWrite(latch, 0);\r\n  digitalWrite(clock, 0);  \r\n  digitalWrite(data,
    0);\r\n  \r\n  for(int i = 0;i < 8;i++) {\r\n      if(Count = 50) { \r\n    Count
    = 0;\r\n    Brightness += BrightnessInc;    \r\n  }\r\n  \r\n  if(Brightness >
    50) {\r\n    BrightnessInc = -1;\r\n  }else\r\n  if(Brightness < 0) {\r\n    BrightnessInc
    = 1;\r\n  }\r\n  \r\n  for(int i = 0;i < 8;i++) {\r\n    digitalWrite(clock, 0);\r\n
    \   \r\n    digitalWrite(data, Pins[i]);\r\n    \r\n    digitalWrite(clock, 1);\r\n
    \   digitalWrite(data, 0);\r\n  }\r\n \r\n  digitalWrite(clock, 0); \r\n  digitalWrite(latch,
    1);\r\n}"
- id: 542
  author: MetaCipher
  author_email: tim@metacipher.com
  author_url: http://www.sdltutorials.com
  date: '2010-07-24 17:02:17 +0000'
  date_gmt: '2010-07-24 15:02:17 +0000'
  content: "Comment system totally butchered my code. Is using htmlspecialchars really
    that hard? Replace ~ with less than sign.\r\n\r\nint data = 2;\r\nint clock =
    3;\r\nint latch = 4;\r\n\r\nboolean Pins[8];\r\n\r\nint Count = 0;\r\n\r\nint
    Brightness = 0;\r\nint BrightnessInc = 1;\r\n\r\nvoid setup() {\r\n  pinMode(data,
    OUTPUT);\r\n  pinMode(clock, OUTPUT);\r\n  pinMode(latch, OUTPUT);\r\n}\r\n\r\nvoid
    loop() {\r\n  digitalWrite(latch, 0);\r\n  digitalWrite(clock, 0);  \r\n  digitalWrite(data,
    0);\r\n  \r\n  for(int i = 0;i ~ 8;i++) {\r\n      if(Count ~ Brightness) {\r\n
    \       Pins[i] = 1;\r\n      }else{\r\n        Pins[i] = 0;\r\n      }\r\n  }
    \ \r\n  \r\n  Count++;\r\n  \r\n  if(Count >= 50) { \r\n    Count = 0;\r\n    Brightness
    += BrightnessInc;    \r\n  }\r\n  \r\n  if(Brightness > 50) {\r\n    BrightnessInc
    = -1;\r\n  }else\r\n  if(Brightness ~ 0) {\r\n    BrightnessInc = 1;\r\n  }\r\n
    \ \r\n  for(int i = 0;i ~ 8;i++) {\r\n    digitalWrite(clock, 0);\r\n    \r\n
    \   digitalWrite(data, Pins[i]);\r\n    \r\n    digitalWrite(clock, 1);\r\n    digitalWrite(data,
    0);\r\n  }\r\n \r\n  digitalWrite(clock, 0); \r\n  digitalWrite(latch, 1);\r\n}"
- id: 597
  author: Andri
  author_email: andri1987@libero.it
  author_url: ''
  date: '2010-12-09 13:05:11 +0000'
  date_gmt: '2010-12-09 11:05:11 +0000'
  content: "Hi tobi,\r\n\r\nvery nice code!! Fabulous...\r\nbut I have a question...which
    mathematical formula  \"pt = period * high / (low + high )\" is??\r\nHas it a
    name? Or do you know where I can find it?\r\nI want to work with it to get one
    cycle of fading-in led...then a piezo works...and finally one cycle of fading-out
    led...WHITOUT DELAY :D"
- id: 598
  author: Marco
  author_email: marco.righetto@gmail.com
  author_url: ''
  date: '2010-12-09 20:48:57 +0000'
  date_gmt: '2010-12-09 18:48:57 +0000'
  content: "Hi Tobi!\r\nVery nice trick! I am prototyping my thesis project, which
    involves 24 LEDs fading in and out according to the 24  photoresistors used as
    on/off switches. I am using n. 3 4051 for the INPUTS and probably I'll use TLC
    5940 for OUTPUTS. Do you think your code it's suitable for my project? Did you
    came up with a newer version of the code? That would be awesome and extremely
    helpful! Please let me know"
- id: 599
  author: tobi
  author_email: t.bielohlawek@gmail.com
  author_url: http://
  date: '2010-12-10 11:52:58 +0000'
  date_gmt: '2010-12-10 09:52:58 +0000'
  content: sorry no updated code and not quite sure about the math formula, neither
    its name :-) it was just a quick hack to get prepared controlling the 8x8 LED
    Matrix... happy u like it :-)
- id: 600
  author: Andri
  author_email: andri1987@libero.it
  author_url: ''
  date: '2010-12-10 16:47:55 +0000'
  date_gmt: '2010-12-10 14:47:55 +0000'
  content: "No problem Tobi...I've found another code and with a little bit \"patiece\"...it
    works :D\r\nI post the code that I've modified...have a nice day!! Thanks!\r\n\r\n\r\nvoid
    setup()  \r\n{ \r\n  pinMode(9, OUTPUT);\r\n} \r\n\r\nvoid fade(int pin, int start,
    int finish, int milliseconds)\r\n{\r\n  uint32_t startMillis = millis();  // remember
    when we started\r\n  while (true)  // we will 'break' when we are done\r\n  {\r\n
    \   uint32_t elapsedTime = millis() - startMillis;  // track the time\r\n    \r\n
    \   // convert the elapsed time into a brightness range\r\n    int brightness
    = map(elapsedTime, 0, milliseconds, start, finish);\r\n    analogWrite(pin, brightness);\r\n
    \   \r\n    // exit when milliseconds have elapsed\r\n    if (elapsedTime >= milliseconds)\r\n
    \   {\r\n      break;\r\n    }\r\n    delay(1);\r\n  }\r\n}\r\n\r\nvoid loop()
    \ \r\n{ \r\nfade(9, 0, 255, 1000);  // fade led on pin 9 from min to max over
    one second\r\ndelay(2000);  // hold for 2 seconds\r\nfade(9, 255, 0, 2000);  //
    fade pin 9 from max to min over 2 seconds\r\ndelay(1000);  // hold for 1 second\r\n}"
- id: 687
  author: Marc de Gier
  author_email: marc@marcdegier.com
  author_url: http://www.marcdegier.com
  date: '2011-03-31 00:04:56 +0000'
  date_gmt: '2011-03-30 22:04:56 +0000'
  content: "This is easier:\r\n\r\nint ledPin = 13;   \r\nunsigned int i=0;\r\nboolean
    rise=true;\r\nint period=1000;\r\n\r\n \r\nvoid setup()\r\n{\r\n  pinMode(ledPin,
    OUTPUT);     \r\n}\r\n \r\nvoid loop()\r\n{\r\n  if(i == period)\r\n  {\r\n    i=1;\r\n
    \   rise= !rise;\r\n  }\r\n  if(rise == false)\r\n  {\r\n    digitalWrite(13,
    LOW);\r\n    delayMicroseconds(i);\r\n    digitalWrite(13, HIGH);\r\n    delayMicroseconds(period-i);\r\n
    \   i=i+1;\r\n  }\r\n  \r\n  if(rise == true)\r\n  {\r\n    digitalWrite(13, LOW);\r\n
    \   delayMicroseconds(period-i);\r\n    digitalWrite(13, HIGH);\r\n    delayMicroseconds(i);\r\n
    \   i=i+1;\r\n  }\r\n  \r\n}"
- id: 688
  author: tobi
  author_email: t.bielohlawek@gmail.com
  author_url: http://
  date: '2011-03-31 11:03:02 +0000'
  date_gmt: '2011-03-31 09:03:02 +0000'
  content: nice
- id: 1569
  author: Rolf
  author_email: rolfje@rolfje.com
  author_url: http://rolfje.wordpress.com
  date: '2012-12-22 21:52:18 +0000'
  date_gmt: '2012-12-22 20:52:18 +0000'
  content: "Standing on the shoulder of giant Marc:\r\n\r\n\r\nint ledPin = 13;\r\nunsigned
    int i=0;\r\nboolean rise=true;\r\nint period=1000;\r\n\r\nvoid setup() {\r\n  pinMode(ledPin,
    OUTPUT);\r\n}\r\n\r\nvoid loop() {\r\n\r\n  digitalWrite(13, LOW);\r\n  delayMicroseconds(i);\r\n
    \ digitalWrite(13, HIGH);\r\n  delayMicroseconds(period-i);\r\n\r\n  if (rise)
    {\r\n    i++;\r\n  }   \r\n  else {\r\n    i--;\r\n  }\r\n\r\n  if (i == period
    || i == 0) {\r\n    rise != rise;\r\n  }\r\n}"
- id: 7213
  author: Bartek
  author_email: bartek@env.pl
  author_url: ''
  date: '2013-11-05 01:39:03 +0000'
  date_gmt: '2013-11-05 00:39:03 +0000'
  content: "Compact version.\r\n\r\nunsigned int i=1;\r\nboolean rise=false;\r\nint
    period=1000;\r\n\r\nvoid setup() {\r\n}\r\n\r\nvoid loop() {\r\n  if(i == period-1
    || i == 1) {\r\n    rise=!rise;\r\n  }\r\n  if(rise == true) {\r\n    i++;\r\n
    \ } else {\r\n    i--;\r\n  }\r\n  digitalWrite(13, LOW);\r\n  delayMicroseconds(period-i);\r\n
    \ digitalWrite(13, HIGH);\r\n  delayMicroseconds(i);\r\n}"
---
This is a nice experiment I did to fade and pulse a LED by just using a _digital_ port. Digital? On/Off, 1/0 - how can this work? Well it does, check this out:

<http://www.youtube.com/watch?v=kB62BrQBjTg>

The key is, I'm switching the LED on & off very fast which appears the human eye as it's on all the time (similar to a LED Matrix). Now, I change the time period between switching the LED on and off. Is the off period time longer, the LED lights low, is the off period time short, the LED lights high. Fading the period time, makes the LED pulse... nice!

Check this (still quite ugly) code:  
[c]  
int ledPin = 13; // LED connected to digital pin 13  
int value = LOW; // previous value of the LED  
long cnt = 0; // will store last time LED was updated  
long low = 0; // interval at which to blink (milliseconds)  
long high = 1000; // interval at which to blink (milliseconds)  
int op = 3;  
long a = 0;

void setup()  
{  
 pinMode(ledPin, OUTPUT); // sets the digital pin as output  
}

void loop()  
{  
 a += op;  
 blinkl( a+30, 10 );  
 if( a \> 200 || a \< 0 ) op \*= -1;  
}

void blinkl(long low, long high )  
{  
 int c = 5;  
 while ( c \> 0 ) {  
 blink( low, high );  
 c-=1;  
 }  
}

void blink( long low, long high )  
{  
 long period = 4000;  
 long pt = period \* high / (low + high );  
 int value = LOW;  
 digitalWrite(ledPin, value);

while( period \> 0 ) {  
 if (period \< pt && value == LOW ) {  
 value = HIGH;  
 digitalWrite(ledPin, value);  
 }  
 period -= 1;  
 }  
}  
[/c]