# Current Settings Recommendation for dual 6374 10S6P set up

### Replies: 11 Views: 268

## \#1 Posted by: RafaelinMissouri Posted at: 2019-03-12T14:35:24.280Z Reads: 97

```
![20190311_214839|690x388](upload://z51fzamEdYxDWnKdC8x6pQhl0lX.jpeg) 

Hey kids.

I am moving on from dual 6355 170kV to dual 6374 190kV(Flipsky Sensored Motors)

Can anyone recommend current settings?

I an running dual FOCBOXES over Canbus.  Using Ackmaniac.

I have a 10S6P 756wh battery, with charge only BMS.

I was planning on running sensored BLDC.  had some issues with one of the motors last night.  did not do too much trouble shooting.  It would run detection fine, but when setting the PPM it woudl not actually spin.  it would just wine.  it ran fine unsensored.  

when it seemed to run fine unsensored i had set each Focbox at
80 motor max
-40 motor min
40 battery max
-12 battery min
32 battery cutoff
30 battery cutoff

I weight 210lbs(95kG)  
plan on running 107s
18/38t   or  18/36t

with the 6355 170kv motors. it was all the same(18/38t) and i was getting top speed at most 32mph(51.5kmh)
```

---
## \#2 Posted by: ryansinatra Posted at: 2019-03-12T14:37:48.851Z Reads: 88

```
Discharge only BMS? How do you balance while charging then?
```

---
## \#3 Posted by: mmaner Posted at: 2019-03-12T14:54:04.749Z Reads: 83

```
80/-40 is ok, I would consider 60/-60 for a more linear throttle.  

[quote="ryansinatra, post:2, topic:86955, full:true"]
Discharge only BMS? How do you balance while charging then?
[/quote]

I think he meant charge only, I make the same mistake all the time :).
```

---
## \#4 Posted by: ryansinatra Posted at: 2019-03-12T14:55:05.717Z Reads: 82

```
Was hoping so 😂
```

---
## \#5 Posted by: RafaelinMissouri Posted at: 2019-03-12T15:20:51.075Z Reads: 79

```
**charge only....
```

---
## \#6 Posted by: RafaelinMissouri Posted at: 2019-03-12T15:22:56.026Z Reads: 76

```
So I was under the impression going to the 6374 improves breaking. does the -60 make the breaks even stronger?

and when you mean linear do you mean a similar increase from start to top speed?

i kind of like the punch feeling.
```

---
## \#7 Posted by: mmaner Posted at: 2019-03-12T15:32:47.848Z Reads: 73

```
[quote="RafaelinMissouri, post:6, topic:86955"]
I was under the impression going to the 6374 improves breaking
[/quote]

I have heard that, but in my experience it's the same.  The only major difference is mass, meaning it stays cooler and operates more efficiently on heavy loads (meaning my fat ass :slight_smile:  ).

[quote="RafaelinMissouri, post:6, topic:86955"]
and when you mean linear do you mean a similar increase from start to top speed?
[/quote]

I mean accelerates and decelerates at the same force at the same trigger position.  Even with a throttle curve, assuming you have identical top/bottom curve values.

Try this, set your motor max at 60a and your motor min at -60a, set the throttle curve to the values in the screen shot below assuming your using 2.54.  If you using 3.02 use -20/-20 nominal.

![image|690x49](upload://uFhZmeE7CldPDT9Az3kNBjV4baV.png) 

Then you can adjust up and down from there.
```

---
## \#8 Posted by: RafaelinMissouri Posted at: 2019-03-12T15:36:29.249Z Reads: 69

```
Ohhh doggie, I have been meaning to mess with the throttle curve thing...

sorry, i don;t know what 2.54 or 3.02 are?
```

---
## \#9 Posted by: mmaner Posted at: 2019-03-12T15:38:07.608Z Reads: 66

```
Those are the firmware version of the @Ackmaniac VESC firmware.  The major versions are 2.54 and 3.102.  The throttle curve is defined differently depending on the firmware you are using.
```

---
## \#10 Posted by: RafaelinMissouri Posted at: 2019-03-13T00:49:27.131Z Reads: 48

```
Ok. I went 60 -60. 40 -12 on battery and set up the throttle curve.  I could not get it going sensored. Messed around with moving the phase wires and got one motor going sensored and the other one would only work sensored spinning in the wrong direction and the wizard could not change the direction... Weird stuff. They sound good unsensored. Off course it is raining so I have to wait a couple days to ride.![20190312_191942|690x388](upload://hBgg6203wHnkPxgij8b8WKYuQ0l.jpeg)
```

---
## \#11 Posted by: RafaelinMissouri Posted at: 2019-03-14T01:33:53.218Z Reads: 33

```
Well. I'm sure not smart enough or patient enough to figure it out. I opened it all back up. Reprogrammed the Focboxes. 1 worked sensored on the first go.  2 not so lucky... I tried all variations of the phase wires and it would detect fine Everytime sensored. But when it came time to set the ppm it would not run right. A couple would run stuttering. A couple would not run. One the motor would just whine... And one worked fine but was going the wrong freaking direction.  So I ended up leaving the 2nd Focbox unsensored. The master is running sensored. Ground is wet right now. Will see how it goes tomorrow
```

---
