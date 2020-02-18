# Any Idea how to add an Odometer (not using a VESC)

### Replies: 16 Views: 977

## \#1 Posted by: Orin635 Posted at: 2017-10-20T21:52:02.239Z Reads: 150

```
Hi guys,

I love the idea of adding an odometer (I think that's what it is called) and being able to track how many km/miles in total I have travelled without using a VESC

The boosted board has this feature and I'd love to add it to my future build, but, I do not know how I would achieve this: frowning:

I've done a little bit of research and found some bulky, ugly odometers on eBay. I guess I could dissect it and just add the circuit into my board but I would prefer to go the DIY route (since it will probably be better and less expensive) and maybe hopefully somehow send that info to an app on my phone (but that's getting a little ahead of my self )

If anyone has done this I'd love to know how you achieved this. Or even if you have an idea please comment, thanks :)
```

---
## \#2 Posted by: wafflejock Posted at: 2017-10-20T21:57:58.295Z Reads: 146

```
I use a bluetooth module and the http://metr.at application to track things for the most part.  Also google track my every move so I just use the timeline in google maps for overview (also lots of good apps for tracking biking/running on phones that can utilize your GPS and other sensors in the phone to get accurate numbers).  I think the VESC also keeps an overall odometer count on the revolutions of the motor but not sure if that just counts while running or gets persisted into ROM.
```

---
## \#3 Posted by: Orin635 Posted at: 2017-10-20T21:59:56.460Z Reads: 142

```
what does your bluetooth module track, also I would like to track my total distance ever (like on a car) without using my phone
```

---
## \#4 Posted by: wafflejock Posted at: 2017-10-20T22:01:15.216Z Reads: 136

```
The bluetooth module relays information to the phone which actually logs the data and plots it for you and gives you a button to upload the data to a site where you can view it in a browser or share the link with others, it doesn't really store anything itself just acts as a relay for info the VESC captures.  Can see a data dump here:

https://metr.at/r/rKZvg
```

---
## \#5 Posted by: mmaner Posted at: 2017-10-20T22:01:41.684Z Reads: 119

```
I would suggest an hours meter like John Deere uses, they make digital versions but this is all could find in a hurry.
https://www.amazon.com/Round-Meter-Gauge-Tractor-Loader/dp/B00C0SQCPM
```

---
## \#6 Posted by: Orin635 Posted at: 2017-10-20T22:02:59.558Z Reads: 111

```
do you need a vesc to use that?
```

---
## \#7 Posted by: Orin635 Posted at: 2017-10-20T22:03:57.822Z Reads: 106

```
sorry I am confused on how it works :P ??
```

---
## \#8 Posted by: wafflejock Posted at: 2017-10-20T22:04:14.378Z Reads: 106

```
Ah yeah sorry I saw "VESC" in your first sentence but didn't really read clearly, without VESC bluetooth module is no help anyhow.

---

Believe the meter sent just shows the on time in hours for a power source.
```

---
## \#9 Posted by: Orin635 Posted at: 2017-10-20T22:05:05.314Z Reads: 102

```
its grand :joy: Im sure i can find something else
```

---
## \#10 Posted by: wafflejock Posted at: 2017-10-20T22:17:46.429Z Reads: 104

```
If you're interested in programming and arduino you could embed a magnet in the wheel and put a hall sensor in your board and just have the arduino count the times the hall sensor gets triggered by the magnet going past it, would just need a sensitive enough hall sensor to pick up the magnetic force from a couple inches away (ones I have trigger at about an inch with small neodymium magnets).  The arduino has read only memory as well so you could save the new counter every time or every 10 or 100 times it increments so you're never too far off on count, sure you can find odometers that are premade and do the same but might spend as much time modifying that to work rather than building it up from simple components.
```

---
## \#11 Posted by: Orin635 Posted at: 2017-10-20T22:19:28.328Z Reads: 96

```
sounds interesting might try that. not very good at coding
```

---
## \#12 Posted by: GIP_longboard Posted at: 2017-10-21T00:07:32.692Z Reads: 81

```
If your motors are sensored you can also use the built in hall sensors instead of building them into the wheel. You can also add external hall sensors to an unsensored motor. Just an idea.
```

---
## \#13 Posted by: mmaner Posted at: 2017-10-21T01:43:53.738Z Reads: 76

```
An hour meter is simple, when it has power it's counting.  Get one that will support your pack voltage or use a voltage converter to generate 12 volts and hook up the hour meter. That's all there is to it, it just works.
```

---
## \#14 Posted by: Okami Posted at: 2017-10-21T15:49:09.251Z Reads: 58

```
Not sure what is minimum wheel size for bicycle speedometers but i know certain speedos could be used for mountainboard tires
```

---
## \#15 Posted by: Orin635 Posted at: 2017-10-21T16:26:26.097Z Reads: 53

```
Alright thanks guys for all the ideas!!! I will decide which is best for my build will keep everyone updated
```

---
## \#16 Posted by: Chewie Posted at: 2017-10-28T13:36:33.355Z Reads: 33

```
It wouldn't be stored in your board, which would be way more convenient, but runtracker type apps on your phone would work as well.
```

---
