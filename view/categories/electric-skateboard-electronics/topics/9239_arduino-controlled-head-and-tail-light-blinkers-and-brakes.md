# Arduino controlled head and tail light + blinkers and brakes

### Replies: 11 Views: 2491

## \#1 Posted by: lilracerboi Posted at: 2016-09-09T03:34:23.191Z Reads: 240

```
I've thought about the idea of front and rear lights which are white and red respectively.
I figured since the channel 1 wheel on the mini remote (or any car rc remote, like GT2B) goes completely unused, I could re-purpose it for use as indicator control. I also included brake lights.

Just yesterday I started working with some spare WS2801 LED strips.
While I was in class <strike>paying attention</strike>, I went ahead and started writing up the code for the Arduino Uno.

I won't actually be using the Arduino Uno in my board as it's too big and has higher possibility for failure.
I will instead be using the Adafruit Pro Trinket. It's basically a way smaller Arduino Uno. This will also allow me to make it more shock resistant.

Here it is compared to the Arduino Uno. The Pro Trinket is in the center while the standard Trinket is right.
<img src="/uploads/db1493/original/3X/b/8/b820a4fe2fe2f719afbaf58cd119b6f49397e0dc.jpg" width="666" height="500">

Either one of these buck converters will be used to connect everything to the Space Cell
https://www.amazon.com/SMAKN%C2%AE-Converter-Voltage-MICRO-USB-Waterproof/dp/B00PXDEZ3C/ref=sr_1_1?ie=UTF8&qid=1473391070&sr=8-1&keywords=48v+to+5v+buck+converter
https://www.amazon.com/Voltage-Step-Down-Converter-converter-Waterproof/dp/B010F95G2M/ref=sr_1_2?ie=UTF8&qid=1473391070&sr=8-2&keywords=48v+to+5v+buck+converter

Here is a demo video using a GT2B:
https://youtu.be/NAFW3BMy4-s

The nice thing about using an Arduino is I can do what ever I want with my lights.
For example, my friend suggested I put 4 strips around my board, head and tail lights and one strip on each side, and make one whole side blink when using my indicators.
I can also add some animations.

I just wish the mini remote had a third channel.
```

---
## \#2 Posted by: Kaly Posted at: 2016-09-09T03:40:55.743Z Reads: 229

```
This is great :-)
```

---
## \#3 Posted by: racidon Posted at: 2016-09-09T04:10:39.346Z Reads: 220

```
ha! I was planing on doing this with an iteration of my own :) beat me to it :) 
good job
```

---
## \#4 Posted by: lilracerboi Posted at: 2016-09-09T04:59:15.832Z Reads: 214

```
Haha thanks.

I plan on upgrading the mini remote to lipo and adding an NRF24L01 and another Trinket for more wireless control over things.
```

---
## \#5 Posted by: saul Posted at: 2016-09-09T05:57:49.260Z Reads: 199

```
pretty cool I was doing a similar setup but for some reason once I connect power and the ch1 to the rx the vesc doesn't power on. Need to try with a diferent buck converter....

I would look at nano clones, $3 on ebay..just takes a while to ship.
```

---
## \#6 Posted by: susplus Posted at: 2016-09-09T11:24:05.819Z Reads: 180

```
Awesome thing....would like to replicate that :D 
take a look at this little thing. Will offer you an 2A 5v Usb power and also extra power for any other things ( V out next to the USB ) 

http://www.ebay.de/itm/131214854776?_trksid=p2060353.m2749.l2649&ssPageName=STRK%3AMEBIDX%3AIT
```

---
## \#7 Posted by: capfirepants Posted at: 2016-11-14T15:37:12.565Z Reads: 136

```
Would it be possible to use an arduino nano with the 5v 1A output of the VESC for this?
```

---
## \#8 Posted by: SORRENTINO Posted at: 2016-11-14T15:41:03.352Z Reads: 135

```
Could use this for 5v and 12v. https://hobbyking.com/en_us/turnigy-multistar-twin-output-5-10-amp-6-50v-sbec-for-lipoly.html
```

---
## \#9 Posted by: mmaner Posted at: 2016-11-14T16:05:54.972Z Reads: 128

```
It would be great if you shared the code and maybe did a build tutorial.  This is a function that adds needed functionality to an electric skateboard and will go along way to making the general public be more accepting of them.
```

---
## \#10 Posted by: lilracerboi Posted at: 2016-11-14T16:36:46.963Z Reads: 124

```
I was planning on sharing the code once it was in a condition I deemed good, but I haven't actually touched it in a long time as I've gotten busy doing other things + school.

I can upload what I have though. It'll be done later in the day.
```

---
## \#11 Posted by: lilracerboi Posted at: 2016-11-14T18:45:40.747Z Reads: 121

```
I uploaded my code to my GitHub.
https://github.com/pdien/arduino_led_blinker

There are two different .ino files.
One for the Adafruit WS2801 library and the other for the FastLED library.

It may or may not work for other setups.
I coded it based on a straight line of LEDs.
```

---
