---
id: 367
title: launchpad
date: 2009-12-20 16:50:32.000000000 +01:00
permalink: "/launchpad/"
layout: page
categories:
- Lost in Web
tags: []
comments:
- id: 653
  author: Sebastian Lex
  author_email: lexsebastian@gmx.de
  author_url: http://www.weissesbuero.de
  date: '2011-02-14 19:47:14 +0000'
  date_gmt: '2011-02-14 17:47:14 +0000'
  content: "Hi,\r\n\r\nkurzes Danke f&uuml;r Deine super Bibliothek. Habe mir dadurch
    einen feinen Sequencer basteln k&ouml;nnen. \r\n\r\nhttp://www.weissesbuero.de/2011/02/whiteout-processing-sequencer-launchpad/\r\n\r\nViele
    Gr&uuml;&szlig;e,\r\nslx"
- id: 816
  author: Justin
  author_email: cacheflowe@cacheflowe.com
  author_url: http://cacheflowe.com
  date: '2011-09-24 21:18:19 +0000'
  date_gmt: '2011-09-24 19:18:19 +0000'
  content: "I built a realtime equalizer with it :)\r\n\r\nhttp://vimeo.com/29517018\r\n\r\nI
    think some of the color constants might be off - some yellows are red, and vice
    versa. I'll take a look at the source soon. Thank you for the library!!\r\n\r\n-Justin"
- id: 1409
  author: Renzo
  author_email: renzolut@gmail.com
  author_url: ''
  date: '2012-11-28 20:01:43 +0000'
  date_gmt: '2012-11-28 19:01:43 +0000'
  content: "Hi, very nice library you got there, i will use it for a project, thank
    you very much. I have a couple of questions though: \r\n\r\n*Can I use your library
    to just read the current button states? i mean polling the launchpad to see what
    color is some button currently in, for instance?\r\n\r\n*Dou you know if it's
    even possible to use the Launchpad with the Ableton Software WHILE AT THE SAME
    TIME use your library to do some other stuff?\r\n\r\nWhen I'm done with my project
    I'll send you a video and of course put you in the credits :)\r\n\r\nThx!"
- id: 307212
  author: Logan
  author_email: lrpcat1215@yahoo.com
  author_url: ''
  date: '2016-12-18 04:15:16 +0000'
  date_gmt: '2016-12-18 03:15:16 +0000'
  content: I'd love to use this library, but I have a Launchpad S and it refuses to
    find the midi device. I really hope this gets updated to use any launchpad model.
    I can't figure out how to change the java source myself.
- id: 307721
  author: Mattia
  author_email: jadison.fly@gmail.com
  author_url: ''
  date: '2017-07-02 20:00:47 +0000'
  date_gmt: '2017-07-02 19:00:47 +0000'
  content: Hi! I've purchased a LP mk2 to use with this programm , it doesn't work...
    please upgrade! :'(
- id: 307969
  author: admin
  author_email: t.bielohlawek@web.de
  author_url: http://
  date: '2018-01-27 22:44:01 +0000'
  date_gmt: '2018-01-27 21:44:01 +0000'
  content: Pls send me a LP mk2 and I will ;)
- id: 308372
  author: Khaled
  author_email: kmeg@free.fr
  author_url: ''
  date: '2018-11-08 22:09:47 +0000'
  date_gmt: '2018-11-08 21:09:47 +0000'
  content: "Dear sir i have download rgbmtx and processing 3.4 i have an error when
    i compiled the rgbmtx\r\n\r\nThe function getToolkit() does not exist.\r\n\r\nRegards"
---
The [Novation's launchpad](http://www.novationmusic.com/products/launchpad) is a 8x8 RG LED MIDI controller similar to the [Monome](http://monome.org/). In addition, it has 8 Button on the top and 8 Scene Button on the left. Originally meant as MIDI Controller its bundled with Ableton Live to pimp your DJ Sets and Tunes. All over it's a wonderful device, not only for your music, but for doing some LED ouput & input hacking.

Thomas Jachmanns released a [ruby library gem](http://github.com/thomasjachmann/launchpad) quite soon after the device was released. But by now, I couldn't find any Processing/Java support, so it's was time to create a proper wrapper library... and here it is!

The library provides an interface to access novation's launchpad programmatically and is heavily based on ruby launchpad gem which you can see by it's similar APIs. LEDs can be lighted and button presses can be listened to.

In addition, it includes a wrapper for the Monomic Library, so you can port all Monome Processing code to Launchpad easily!

It's [project page](http://rngtng.github.com/launchpad/) and its [source](http://github.com/rngtng/launchpad) is hosted on github. Please feel free to use it for your proposes and fork and improve the source!  
<http://www.vimeo.com/7832566>

more Video examples comming soon!