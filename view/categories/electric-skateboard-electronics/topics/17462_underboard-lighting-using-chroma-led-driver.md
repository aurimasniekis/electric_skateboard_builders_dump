# Underboard Lighting using Chroma LED driver

### Replies: 36 Views: 2606

## \#1 Posted by: JonathanLau1983 Posted at: 2017-02-09T20:11:08.045Z Reads: 286

```
I've been thinking of adding underboard lighting to my board for a while but never saw a solution I liked.

I then came across the Chroma LED driver which was designed for racing quads, but works a treat on my board.
It's limited to controlling 25 sequential LEDs, but can run up to 50 so I ran two lots of 25 in parallel.

https://www.youtube.com/watch?v=MNQ3afoXEJc
```

---
## \#2 Posted by: mmaner Posted at: 2017-02-09T20:12:40.810Z Reads: 278

```
Post how you did it, I'm really interested.  What equipment did you use and what code?
```

---
## \#3 Posted by: mptrs Posted at: 2017-02-09T20:16:42.272Z Reads: 275

```
That's a very cool light show! Was thinking about this as well, but was thinking about a arduino nano or something like that.

Would love to know how you did this.
```

---
## \#4 Posted by: JonathanLau1983 Posted at: 2017-02-09T20:17:05.993Z Reads: 267

```
The Chroma has everything built in, I bought it from the site below. I had to buy a 6S to 12V voltage regulator as wasn't sure if the Chroma could take such a high voltage.
I then bought a 60 LED 1M WS2812B strip from Ebay which i cut into 2 x 25 LED strips.

https://shop.neofpv.com/products/chroma-led-driver-controller
```

---
## \#5 Posted by: jimbosays Posted at: 2017-02-09T20:39:41.998Z Reads: 252

```
That's awesome, did you hook it up straight to your battery I'm assuming then? How'd you do that?
```

---
## \#6 Posted by: mmaner Posted at: 2017-02-09T20:56:28.748Z Reads: 240

```
I cant seem to find the Chroma LED Controller in the US.  Does anyone no of an addressable WS2812B LED controller that has multiple modes & colors, that is available in the US?  I really dont know anything about these LED's but I've been wanting to do this for awhile now.
```

---
## \#7 Posted by: JonathanLau1983 Posted at: 2017-02-09T21:32:43.741Z Reads: 218

```
I used a 12V regulator, the Chroma has a 5V regulator built in, but I didn't think it could take 6S ~24V.
```

---
## \#8 Posted by: IsTalo Posted at: 2017-02-09T22:09:34.431Z Reads: 213

```
Could I use a Mosfet LM317T? Or some mosfet like this that enter 40V and outoput 12v?
```

---
## \#9 Posted by: Norco Posted at: 2017-02-09T23:01:05.702Z Reads: 208

```
Love to see a vid of the light pattern this casts as you ride - great work
```

---
## \#10 Posted by: jimbosays Posted at: 2017-02-10T04:41:40.554Z Reads: 197

```
right, but is the regulator hooked up straight to the XT90 (or whatever connector) coming off the battery pack, or did you use a splitter and then another splitter (if using a dual motor)?
```

---
## \#11 Posted by: JonathanLau1983 Posted at: 2017-02-10T09:12:05.662Z Reads: 181

```
That should work fine, but Linear voltage regulators are not as efficient as switching regulators which I used. I used the one below (it's an affiliate link, are those allowed here?).
http://eu.banggood.com/Wholesale-Warehouse-3A-UBEC-Module-Low-Ripple-Bluesky-Mini-Switch-Mode-DC-BEC-5V-12V-2-6S-Supply-wp-Eu-993056.html?p=RV04089380152014121B

@jimbosays I have a wire coming off the XT60s connector going to the above voltage regulator, with the positive going through a switch. This was an additional wire tagged on the outside of the connector, the inside was taken up by the lower guage wiring to the ESC.
```

---
## \#12 Posted by: saul Posted at: 2017-02-10T09:56:42.010Z Reads: 167

```
I didn't know drivers like that existed for ws2812. I like how they use the micro buck converters on the back. should be good for about 22v.
```

---
## \#13 Posted by: HTownBomber Posted at: 2017-02-10T14:06:35.940Z Reads: 166

```
Adafruit might be the way to go. Plenty of guides, LED strips, controllers and code libraries here:

https://learn.adafruit.com/adafruit-neopixel-uberguide/neopixel-strips
```

---
## \#14 Posted by: mmaner Posted at: 2017-02-10T14:25:56.765Z Reads: 166

```
[quote="HTownBomber, post:13, topic:17462"]
Adafruit might be the way to go
[/quote]

Cool, I'll give it a look.  thanks
```

---
## \#15 Posted by: JonathanLau1983 Posted at: 2017-02-10T22:55:47.055Z Reads: 157

```
Here it is in action. The fimware seems to have an issue with two LEDs not lighting up in pulse mode, works perfect is all other modes. I've let them know so hopefully this gets fixed in future.
https://youtu.be/TV5cEk_lHwI
```

---
## \#16 Posted by: saul Posted at: 2017-02-11T08:43:03.427Z Reads: 144

```
I'm using that library with the attiny85 for my lights, they are the same ws2812 addressable rgbs.
```

---
## \#17 Posted by: RogerD Posted at: 2017-02-11T10:04:16.019Z Reads: 137

```
Nice. I've ordered all the bits :-) chroma, leds, ubec
```

---
## \#18 Posted by: mptrs Posted at: 2017-02-11T10:07:05.465Z Reads: 144

```
Thanks for the info, looks pretty and it looks to be easy with the Chroma board.
On my todo, but first I need to get a board rollin' hehe
```

---
## \#19 Posted by: RogerD Posted at: 2017-02-11T11:36:40.609Z Reads: 144

```
For those who like a parts list:

http://www.ebay.co.uk/itm/222292817001?_trksid=p2057872.m2749.l2649&var=521130571571&ssPageName=STRK%3AMEBIDX%3AIT

I bought 1m 60 LED waterproof

http://www.ebay.co.uk/itm/221655594331?_trksid=p2057872.m2749.l2649&ssPageName=STRK%3AMEBIDX%3AIT

An obviously the Chroma board - I bought it from the direct link in this thread.

I'll use a 12v toggle switch which I'll recess into the tail of my board
```

---
## \#20 Posted by: ElskerShadow Posted at: 2017-02-11T12:15:35.812Z Reads: 140

```
Is it possible to show the connection and how to set up the system ? How do you control the LEDS?
```

---
## \#21 Posted by: Sander Posted at: 2017-02-11T16:26:26.851Z Reads: 126

```
[quote="JonathanLau1983, post:11, topic:17462"]
That should work fine, but Linear voltage regulators are not as efficient as switching regulators which I used. I used the one below (it's an affiliate link, are those allowed here?).http://eu.banggood.com/Wholesale-Warehouse-3A-UBEC-Module-Low-Ripple-Bluesky-Mini-Switch-Mode-DC-BEC-5V-12V-2-6S-Supply-wp-Eu-993056.html?p=RV04089380152014121B
[/quote]

Do you know any others regulators that handles >44.4V and gives output of 3.3V and <50mA
```

---
## \#22 Posted by: Okami Posted at: 2017-02-11T16:40:54.362Z Reads: 122

```
 Did you show all 5 modes of that chroma board in the video?

I wonder what other ''effects'' there are besides that ''pulsing'' and ''falling dot'' effect :)
```

---
## \#23 Posted by: JonathanLau1983 Posted at: 2017-02-13T09:13:32.840Z Reads: 117

```
@ElskerShadow I don't see the need post a wiring diagram, it could not be simpler. Power goes to the Chroma, power from the Chroma to LEDs and one additional wire for the signal. Labelled on Chroma and LED strips.

@Okami I 3d printed an enclosure for the Chroma in flexible material, this allows me to press the button from the outsite. I also put a hole in the design which I filled in with hot glue so that I could still see the green LED on the Chroma. You can make this out in the first video.
```

---
## \#24 Posted by: Norco Posted at: 2017-02-13T13:58:47.487Z Reads: 119

```
I'd be interested too if you find one...
```

---
## \#25 Posted by: JonathanLau1983 Posted at: 2017-02-13T14:26:08.872Z Reads: 119

```
Here's one, says 48V. Not sure if it requires 48V constant but I would assume it has a fairly big window of input voltage.

[Banggood - DC/DC 48V To 12V 10A 120W Reducer Converter Regulator Waterproof Power Voltage](http://www.banggood.com/DCDC-48V-To-12V-10A-120W-Reducer-Converter-Regulator-Waterproof-Power-Voltage-p-1056723.html?p=RV04089380152014121B)

You could then step it down again using another regulator. I have no idea if there's any issues doing two step downs in series.
```

---
## \#26 Posted by: Norco Posted at: 2017-02-13T16:01:21.808Z Reads: 109

```
Good find...This is becoming a lot more work for some flashy lights though...
```

---
## \#27 Posted by: RogerD Posted at: 2017-02-14T09:32:43.204Z Reads: 102

```
Another good reason for running low voltage :-) (6s)
```

---
## \#28 Posted by: Okami Posted at: 2017-02-14T09:36:58.755Z Reads: 107

```
No, I meant that I read that this Chroma driver has 5 modes.. as you didnt really see any ''text description'' for your video.. I just wanted to know, whenever you went through all of them..
```

---
## \#29 Posted by: JonathanLau1983 Posted at: 2017-02-14T10:10:35.417Z Reads: 109

```
Ah, I see what you mean. I did click through them in the first video, but I didn't zoom out in all of them.
Check out the review below, he goes through the board features in more detail.
https://www.youtube.com/watch?v=vg3YN0C5RQY
```

---
## \#30 Posted by: RogerD Posted at: 2017-02-14T11:58:55.108Z Reads: 106

```
This link has a good wiring diagram:

Also, the driver board takes up to 4s (16.8volts) so no need for such extremme voltage reduction from high voltage packs

https://oscarliang.com/chroma-led-driver/
```

---
## \#31 Posted by: Jaraya92881 Posted at: 2017-02-14T23:18:44.120Z Reads: 100

```
So this might be cool to add for some and I may try it on my buildt http://jamie2015.en.ec21.com/DIY_Aluminum_Extrusion_Flexible_LED--9753214_10175297.html 
some flexible extrusions would be a nice solid piece to put under your board to keep a clean look instead of the taping or glueing of LED's to the bottom of the board. :)
```

---
## \#32 Posted by: RogerD Posted at: 2017-02-14T23:50:58.567Z Reads: 103

```
I'm going to run a router along the sides and recess the LEDs - probably....
```

---
## \#33 Posted by: JonathanLau1983 Posted at: 2017-02-15T09:39:36.271Z Reads: 98

```
@RogerD Great idea, also good for running cabling.
I used copper tape instead of normal wiring for most of it, so it looks tidier.
```

---
## \#34 Posted by: Philxu007 Posted at: 2017-02-16T16:39:28.511Z Reads: 96

```
it is cool,
but I think the [ws2813b](http://www.rgbledcolor.com/sale-8995264-ws2813-dual-signal-led-smd.html) or the [sk6822](http://www.rgbledcolor.com/) is much more stable with the dual signal ic,
when one led broken the other led still works(will not influence the signal transfer)
```

---
## \#35 Posted by: Norco Posted at: 2017-02-16T17:26:31.711Z Reads: 89

```
There is probably a good reason why this wouldn't work but could this step down the voltage in one go for us with 10s?

http://www.hobbytronics.co.uk/d24v3f5-5v-regulator
```

---
## \#36 Posted by: MikeChan006 Posted at: 2019-04-10T11:42:51.392Z Reads: 22

```
I have found there are some dc12v pixel strips http://addressable-led.com/Products/LC8808-LED-Strip.html
so i can use the bigger battery and can use for a longer time,
but what type of controller protocol should I choose for the [lc8808](http://addressable-led.com/Products/DC12V-Pixel-LED-LC8808.html) ?
```

---
