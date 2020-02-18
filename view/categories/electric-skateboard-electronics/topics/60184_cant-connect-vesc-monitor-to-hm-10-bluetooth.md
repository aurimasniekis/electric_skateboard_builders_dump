# Can&rsquo;t connect VESC Monitor to HM-10 bluetooth

### Replies: 22 Views: 1270

## \#1 Posted by: Eboosted Posted at: 2018-06-27T07:01:47.337Z Reads: 188

```
Is anyone else having issues trying to connect to VESC monitor to HM-10 bluetooth lately?

I can't connect to any of my boards, I wonder if VESC Monitor has changed their bluetooth parameters on their latest update.

I can't even detect the bluetooth when I click on scan.
```

---
## \#2 Posted by: L3chef Posted at: 2018-06-27T08:10:29.945Z Reads: 181

```
What os are you running? I heard peeps had issues woth hm 10 and android oreo
```

---
## \#3 Posted by: ROFEN13 Posted at: 2018-06-27T12:29:53.163Z Reads: 167

```
I ordered this one.
[http://s.aliexpress.com/FJBJJ3qI](http://s.aliexpress.com/FJBJJ3qI)
 
I had issues with other modules but someone suggested this and has been solid.
```

---
## \#4 Posted by: Acido Posted at: 2018-06-27T12:35:56.312Z Reads: 166

```
turn on location on your phone, i can not find my module without location on
```

---
## \#5 Posted by: rey8801 Posted at: 2018-06-27T12:36:13.709Z Reads: 163

```
You probably updated to Android Oreo. You can either upload a new firmware on your module https://forum.arduino.cc/index.php?topic=393655.0 or buy another module. In case you want modules with the orinal HM-10 firmware I have some left wired up for cheap :smile:
http://www.electric-skateboard.builders/t/esk8-flea-market-eu-ww-small-cheap-parts-hm-10-bluetooth-android-oreo-compatible-volt-meter-3dprinting/57463?u=rey8801
```

---
## \#6 Posted by: Battosaii Posted at: 2018-06-27T12:36:35.839Z Reads: 156

```
I have android oreo and I been having issues I have hm10 module and they connect sometimes or more recently not at all :/
```

---
## \#7 Posted by: rey8801 Posted at: 2018-06-27T12:38:10.579Z Reads: 150

```
how the module shows up on your phone?
```

---
## \#8 Posted by: Battosaii Posted at: 2018-06-27T12:40:58.760Z Reads: 146

```
 Shows up as HMsoft in fact I have problems with my Raptor 2 bluetooth also but it does work better.
```

---
## \#9 Posted by: rey8801 Posted at: 2018-06-27T12:42:24.741Z Reads: 142

```
That's wierd. Where do you place the module? I had problem when it was close to the motor wires and the battery output. Since I put it somewhere else really stable connection.
```

---
## \#10 Posted by: Battosaii Posted at: 2018-06-27T12:57:02.877Z Reads: 131

```
That may be it cause my current enclosure is very tight.
```

---
## \#11 Posted by: rey8801 Posted at: 2018-06-27T12:59:27.593Z Reads: 122

```
Me too but really few centimeters can make the different. I moved it in the center and far from the motor wires and the signal is much better. I notice when basically I was loosing the signal after hard accelerations when indeed the current rises.
```

---
## \#13 Posted by: accrobrandon Posted at: 2018-06-28T15:57:17.308Z Reads: 109

```
Yes... It'll connect but no data.. And if the data shows at a stop as soon as I move it freezes =\
```

---
## \#14 Posted by: Eboosted Posted at: 2018-06-28T16:22:15.341Z Reads: 108

```
I'll try a phone with older OS and will report back
```

---
## \#15 Posted by: rey8801 Posted at: 2018-06-28T16:42:44.077Z Reads: 109

```
As does your module shows up on the phone? Based on that it's possible to understand which clone it is
```

---
## \#16 Posted by: Mikenopolis Posted at: 2018-06-28T17:07:07.321Z Reads: 109

```
iOS here. I use the HM10 module from Metr.  It worked perfect on my first few test rides on the new build, but in two 15 miles rides, the app only recorded 2 miles and nothing after. I then used the "eSkate VESC" and "Telematics" app and they both record my entire ride.

So I'm not sure where MY problem is
```

---
## \#17 Posted by: Eboosted Posted at: 2018-06-28T18:33:22.188Z Reads: 105

```
Is that eSkate VESC app only available in iOS?
```

---
## \#18 Posted by: Mikenopolis Posted at: 2018-06-28T18:50:16.812Z Reads: 102

```
@Eboosted sadly, it looks that way @emmaanuel doesn't have any plans for Android version 

https://www.electric-skateboard.builders/t/new-version-2-1-ios-eskate-vesc-app-for-standard-and-ackmaniac-fw/32340/162
```

---
## \#19 Posted by: Lionpuncher Posted at: 2018-07-06T03:38:34.873Z Reads: 92

```
@accrobrandon did you solve this? Having a similar issue with a module that worked before but won't show data now. It connects, but doesn't show any info on the app.
```

---
## \#20 Posted by: Eboosted Posted at: 2018-07-06T04:16:49.760Z Reads: 92

```
No, nothing on my side
```

---
## \#21 Posted by: rey8801 Posted at: 2018-07-06T05:48:02.753Z Reads: 91

```
Hi, which module and phone do you have?
Edit: usually the easiest test is to try to connect it with another phone. So you know whether is the module or your phone not fully compatible anymore
```

---
## \#22 Posted by: Lionpuncher Posted at: 2018-07-06T18:07:19.495Z Reads: 84

```
I have a HM-10 and an 'older' android phone. I solved the problem; was stupid mistake on my part. Forgot to write app config so the tool didn't change to PPM + Uart. Made the adjustment and the app worked fine. :smiley:
```

---
## \#23 Posted by: rey8801 Posted at: 2018-07-06T19:12:23.339Z Reads: 81

```
Better like that!
```

---
