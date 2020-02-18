# Help? Can&rsquo;t get full power to motor

### Replies: 43 Views: 1048

## \#1 Posted by: Kaden Posted at: 2017-11-22T04:29:25.727Z Reads: 102

```
 So I have all my batteries hooked up and I tested the voltage coming from my vesc and it was only 3 volts,  each battery has 16.8, is this normal? I Have not been able to get full power to my motor.
```

---
## \#2 Posted by: MysticalDork Posted at: 2017-11-22T04:39:51.211Z Reads: 101

```
Post a photo of your setup, how you're measuring, and what your configuration settings are in the BLDC tool. We can't help until we have enough information.
```

---
## \#3 Posted by: Kaden Posted at: 2017-11-22T04:55:56.736Z Reads: 94

```
<img src="/uploads/db1493/original/3X/e/3/e3026c88552dbee3044ce5a5604a9128590a60cf.jpg" width="374" height="500">
```

---
## \#4 Posted by: Kaden Posted at: 2017-11-22T04:56:22.582Z Reads: 85

```
<img src="/uploads/db1493/original/3X/6/a/6ad6aa4b52b8a7fa92ebf917e2f4a6e3039fb92d.jpg" width="374" height="500">
```

---
## \#5 Posted by: Kaden Posted at: 2017-11-22T04:57:16.136Z Reads: 83

```
My vesc won't detect on bldc and there are no fault codes
```

---
## \#6 Posted by: MysticalDork Posted at: 2017-11-22T05:01:19.378Z Reads: 83

```
it looks like you have one or more of your batteries connected backwards. Looking at the connectors, it seems like you have them going positive to positive, rather than positive to negative.
```

---
## \#7 Posted by: Jinra Posted at: 2017-11-22T05:01:37.342Z Reads: 82

```
What the hell is going on here...?

You have two packs in parallel with the positive going nowhere, and another pack with the negative in parallel and positive going to antispark.. You're running like 11 volts nominal assuming each of those packs are 3s
```

---
## \#8 Posted by: MysticalDork Posted at: 2017-11-22T05:04:52.927Z Reads: 79

```
Yeah, his wiring is all kinds of jacked up.
```

---
## \#9 Posted by: Kaden Posted at: 2017-11-22T05:17:58.064Z Reads: 77

```
The batteries are wired In series? And the board ran before.  I soldered in the on and off switch and then since then and a spark I can't get full power out of the motor. Turns on, spins the motor, just not full power
```

---
## \#10 Posted by: Jinra Posted at: 2017-11-22T05:19:17.738Z Reads: 76

```
Well if you're running 10~ volts, you're probably triggering the low voltage cutoff which is why it's not spinning very much. Your battery is wired up wrong. Disconnect it and try again.

Post your schematic here if you want us to help you fix it, but it makes no sense right now. It's surprising you haven't blown them up yet.
```

---
## \#11 Posted by: Kaden Posted at: 2017-11-22T05:23:26.753Z Reads: 75

```
<img src="/uploads/db1493/original/3X/e/a/ea51b85dc7b0bdb3161dd08f5ce1fb7e4226e3a4.jpg" width="374" height="500">
```

---
## \#12 Posted by: MysticalDork Posted at: 2017-11-22T05:25:25.126Z Reads: 69

```
You're basically running your board off of just one of those batteries. The other two are just sitting there not connected fully. Looc closely at the connections. 

They should go Vesc negative>> 
antispark negative>>
battery 1 negative(then comes out positive)>>
battery 2 negative(then comes out positive)>>
battery 3 negative(then comes out positive)>>
antispark positive>>
vesc positive.

Nope, still wrong. Look at the top left two batteries. Red to red. That's not right.
```

---
## \#13 Posted by: Kaden Posted at: 2017-11-22T05:26:06.045Z Reads: 62

```
All three batteries are wired in series, they are 4s. This is what I ran before and everything was fine.  I soldered In the anti spark switch, and one of the batteries sparked on me, and I didn't know if that ruined my vesc, or shorted the motor, @MysticalDork @Jinra
```

---
## \#14 Posted by: MysticalDork Posted at: 2017-11-22T05:27:19.049Z Reads: 61

```
Look, if you don't listen to our advice, we can't help you. We're telling you that the reason you're having problems is that your batteries are wired wrong. BELIEVE US.
```

---
## \#15 Posted by: Jinra Posted at: 2017-11-22T05:27:27.646Z Reads: 62

```
It's possible you permanently damaged something on your setup due to the incorrect setup of the batteries. Listen to @MysticalDork's reply and setup your batteries to run in a neg -> pos daisy chain fashion.
```

---
## \#16 Posted by: Kaden Posted at: 2017-11-22T05:29:15.308Z Reads: 64

```
Not once did I day I didn't believe you, I'm looking for how to fix it, but I don't know where to begin
```

---
## \#17 Posted by: E1Allen Posted at: 2017-11-22T05:32:04.235Z Reads: 64

```
<img src="/uploads/db1493/original/3X/e/7/e734fa1ca67c671bfc88861a97cc3b404a9f9512.jpg" width="375" height="500">

Wire the anti spark on plus lead
```

---
## \#18 Posted by: MysticalDork Posted at: 2017-11-22T05:32:18.374Z Reads: 59

```
<img src="/uploads/db1493/original/3X/9/3/93312d0be3a632beada22e0452354053743a1ee4.jpg" width="374" height="500"> I'm working on a more complete drawing, but take a look at this in the mean time. Think about how the electricity is supposed to go. Play "What's wrong with this picture?" wit this image and your setup.
```

---
## \#19 Posted by: Jinra Posted at: 2017-11-22T05:32:23.313Z Reads: 61

```
See here, this is how your battery should be hooked up if you want it in series.

<img src="/uploads/db1493/original/3X/3/2/3299782c0c5c07cc24955d8c7d9ed524464bdd27.png" width="494" height="372">
```

---
## \#20 Posted by: E1Allen Posted at: 2017-11-22T05:33:56.454Z Reads: 58

```
Probably a good idea to unplug all that and test voltages as well
```

---
## \#21 Posted by: Kaden Posted at: 2017-11-22T05:36:18.552Z Reads: 57

```
I see what you mean, I bought two of these to wire the batteries together, Uploading...]()
```

---
## \#22 Posted by: Kaden Posted at: 2017-11-22T05:38:43.297Z Reads: 59

```
<img src="/uploads/db1493/original/3X/1/d/1d235c931700c7c06c0537c295829555b4663841.jpg" width="375" height="500">
```

---
## \#23 Posted by: MysticalDork Posted at: 2017-11-22T05:40:39.040Z Reads: 60

```
All you have to do is change your setup from this: <img src="/uploads/db1493/original/3X/e/d/ed57785b3aa6e201a4d6875abe2aed12eeb83c3d.png" width="690" height="388">
to Jinra's diagram. It's just some simple soldering.
```

---
## \#24 Posted by: E1Allen Posted at: 2017-11-22T05:40:57.551Z Reads: 54

```
Yeah, that's for two Batts in series
```

---
## \#25 Posted by: Kaden Posted at: 2017-11-22T05:42:01.416Z Reads: 54

```
I'll try it. Thank you guys.
```

---
## \#26 Posted by: E1Allen Posted at: 2017-11-22T05:43:04.983Z Reads: 51

```
Make sure you check each battery👍👍👍
```

---
## \#27 Posted by: Kaden Posted at: 2017-11-22T07:08:48.733Z Reads: 50

```
Okay I wired correctly and now have full power, but my on and off switch doesn't work, the board stays on, any ideas??
```

---
## \#28 Posted by: Kaden Posted at: 2017-11-22T07:09:02.018Z Reads: 51

```
@MysticalDork @Jinra
```

---
## \#29 Posted by: Jinra Posted at: 2017-11-22T07:09:31.816Z Reads: 51

```
You likely fried the mosfet and now it's perma on.
```

---
## \#30 Posted by: Kaden Posted at: 2017-11-22T07:22:25.802Z Reads: 51

```
Mosfet In the on and off switch? Is there any fix?
```

---
## \#31 Posted by: Kaden Posted at: 2017-11-22T07:29:30.824Z Reads: 49

```
 The switch worked with one battery, I got my wiring right, so now it doesn't work, do I need a new switch possibly? @MysticalDork @Jinra @E1Allen
```

---
## \#32 Posted by: mccloed Posted at: 2017-11-22T07:39:55.741Z Reads: 50

```
Sounds like you need a new switch. Unfortunately, those switches are prone to failure. Where did you get it from? If it was , it may be under warranty.
```

---
## \#33 Posted by: Kaden Posted at: 2017-11-22T07:44:43.798Z Reads: 47

```
It was from there. But I cut the connectors off so I could get it to fit, would that void warranty?
```

---
## \#34 Posted by: wafflejock Posted at: 2017-11-22T07:56:28.713Z Reads: 48

```
If you remove shrink wrap or desolder anything typically it voids any sort of warranty.  Not sure they'd cover this anyhow since it's not likely manufacturer error or component failure in regular use (maybe they cover it though worth checking).  Personally big proponent of just using a loop key with xt-90 antispark plugs far less failure prone and added safety feature if you make it easy to pull while riding.
```

---
## \#35 Posted by: danielz Posted at: 2017-11-22T08:32:43.301Z Reads: 48

```
Why dont people read and understand the theory before jumping in. Im surprised you've not barbecued yourself and your home! Please be careful.
```

---
## \#36 Posted by: pat.speed Posted at: 2017-11-22T09:43:46.868Z Reads: 44

```
Don't worry about the switch you don't need it uneless you want it to look cool. If you just unsolder the switch it will work normally. Your lucky you didn't fry the batteries
```

---
## \#37 Posted by: Kaden Posted at: 2017-11-22T15:02:34.356Z Reads: 33

```
Can you explain where the loop key would go?
```

---
## \#38 Posted by: Kaden Posted at: 2017-11-22T15:02:46.157Z Reads: 33

```
@wafflejock
```

---
## \#39 Posted by: MysticalDork Posted at: 2017-11-22T15:32:25.692Z Reads: 28

```
@Kaden http://makersnebula.com/wp-content/uploads/2016/10/WiringDia.jpg
```

---
## \#40 Posted by: themegak Posted at: 2017-11-22T15:45:21.500Z Reads: 28

```
Don't mean to pile on here but either heat shrink or cover all of the soldered wires with tape or something.  You are asking for shorts the way it is.   Also, there is a great "diagrams" forum post where so many of us posted diagrams of our setups, check it out and all will be clear.  Just search "diagrams" and you will see the post.
```

---
## \#41 Posted by: Kaden Posted at: 2017-11-22T18:42:40.682Z Reads: 24

```
So you can put the loop in just the negative wire?
```

---
## \#42 Posted by: MysticalDork Posted at: 2017-11-22T18:55:42.022Z Reads: 24

```
I personally would put it on the positive wire, but yes. It just breaks the circuit. If you need more info, just search "loop key" here on the forum. Lots of info and advice to be had.
```

---
## \#43 Posted by: wafflejock Posted at: 2017-11-22T23:33:32.118Z Reads: 22

```
Sorry missed your question but yeah use the search for loop key or antispark loop key and quite a few threads outlining different options.  Since the whole circuit needs to be complete for current to flow it can be basically anywhere between the battery and the "load" or VESC in this case, positive or negative shouldn't really make a difference.  If you use an "antispark" instead of just regular xt-90 added benefit the connectors won't spark when plugging them in if you use higher voltage at some point (10 or 12S can fry the connectors while power is flowing into the capacitors on the VESC).
```

---
