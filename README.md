Protocoder
==========

[![Build Status](https://travis-ci.org/victordiaz/protocoder.svg?branch=develop)](https://travis-ci.org/victordiaz/protocoder)

Protocoder is a coding environment + framework in Javascript for quick prototyping on Android devices having some emphasis on rapid software and hardware hacking. 

Install the app in your Android device and access the web IDE from your computer. 
Code in javascript using the protocoder framework. No needs to write dozends of lines to access sensors or write an UI, simple to use, fast to code.

```
//how to get sensor data
sensors.startAccelerometer(function(x, y, z)) { 
	console.log(x + " " + " " + y + " " + z); 
}

//send and sms
android.sendSMS(number, "text");

//play a video
ui.addVideoView("fileName", 0, 0, 500, 200);
```

It uses a webserver and a websockets server inside the project to do some of the magic.

It has support of most android hardware functionality, networking using OSC and websockets, audio synthesis and processing using Pure Data though libPd, OSMmaps, IOIO support and muuuuuuuch more. 

A bit about the folders 

AndroidApp 
----------
Contains the Protocoder android app. It contains two folders Protocoder which is the app it self and Protocoder_custom which is a skeleton to reuse your scripts and compile them into a standalone APK.

DesktopApp
----------
It's (was) the app companion for USB support. The previous solution used node webkit which it was a bit too overkilling. I want to do a simple app to do the routing through USB. If you know a bit of c++ qt give me a touch! :) 

Protocoder.org
-------------- 
It's the Protocoder website itself. If you see any english mistake please let me know as I am not native english speaker! :) Design and content can be improved too! :) 

Scripts 
-------
Run the adb_tunnel_local.sh to forward the connection trough USB. Atm only scripts form mac os x. Contributions welcomed!


How to compile 
--------------
Clone the project, import it in eclipse, make sure the API version you are using to compile is 18 or greater. Eclipse tends to change it when importing projects. 
Press compile et voila.


It all started during the http://www.makewithmoto.com tour. A 5 month cross country roadtrip across the US with a fearless crew from Motorola ATAP on a velcro-covered van and a VW bus full of 3d printers, hackable phones, arduinos, ioios, electronics components. 
During the roadtrip we hacked together with university students and hackerspaces fellows and we realized we needed a better tool for prototyping, which we decided to start coding during the trip. Protocoder has been developed inside cars, hotel lobbys, cafes, restaurants, parks, here and there.
