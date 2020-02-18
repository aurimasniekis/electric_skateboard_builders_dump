# Motor is shaking and jerking a lot and barely spins at all even after a new vesc. Please help!

### Replies: 46 Views: 2659

## \#1 Posted by: dg798 Posted at: 2017-09-10T20:52:35.044Z Reads: 201

```
even when my motor is connected to nothing it gives me some resistantce. when plugged in it gives bad motor detection. it shakes and jerks alot
```

---
## \#2 Posted by: Rinzler Posted at: 2017-09-10T20:54:18.509Z Reads: 198

```
Your motor is very likely to have shorted, if it did dont use it it will fry your controller.
```

---
## \#3 Posted by: dg798 Posted at: 2017-09-10T20:54:50.395Z Reads: 195

```
is there  way to fix it
```

---
## \#4 Posted by: Rinzler Posted at: 2017-09-10T20:57:12.379Z Reads: 187

```
Did you ride it alot, what battery count do you use, did you ride hills or flats?
```

---
## \#5 Posted by: dg798 Posted at: 2017-09-10T20:57:53.747Z Reads: 180

```
didnt ride it once yet. it was doing this ever since i started trying to program the vesc
```

---
## \#6 Posted by: dg798 Posted at: 2017-09-10T20:58:11.666Z Reads: 179

```
and i use 2 6s batteries in series
```

---
## \#7 Posted by: Rinzler Posted at: 2017-09-10T21:06:49.416Z Reads: 172

```
If its new, maybe it isnt burned out, startup stutter is common on an unsensored motor. Do you have another brushless motor to compare the rolling resistance. It is normal for a motor to have some rolling resistance, when you turn it by hand you will feel magnets as you are rotating. In case it is burned out turning it will feel smooth, with energy sucking resistance.
```

---
## \#8 Posted by: Rinzler Posted at: 2017-09-10T21:09:07.749Z Reads: 165

```
But the bad motor detection is weird, i really dont know my vesc stuff so you should probably wait for someone to chime in.
Maybe put VESC in the title of the thread.
```

---
## \#9 Posted by: dg798 Posted at: 2017-09-10T21:09:17.404Z Reads: 156

```
so now its not giving me resistance but this is what happens when i try to do a motor detection: https://photos.app.goo.gl/fGEeWqDd4vsdZUK63. listen to the sound
```

---
## \#10 Posted by: Rinzler Posted at: 2017-09-10T21:11:41.513Z Reads: 153

```
Change the title of the thread, and read this. Your answer is likely here 
http://www.electric-skateboard.builders/t/new-vesc-user-read-this-complete-walktrough-of-the-vesc/2980
```

---
## \#11 Posted by: dg798 Posted at: 2017-09-10T21:12:06.398Z Reads: 143

```
ok thank you
```

---
## \#12 Posted by: dg798 Posted at: 2017-09-10T23:51:23.525Z Reads: 135

```
Can someone please help
```

---
## \#13 Posted by: dg798 Posted at: 2017-09-11T00:40:44.644Z Reads: 127

```
has anyone had this problem and found a solution???
```

---
## \#14 Posted by: GrecoMan Posted at: 2017-09-11T00:41:33.300Z Reads: 127

```
If someone had found a solution, they would have already posted it.  Please stop creating so many topics, we are not here to spoon feed you
```

---
## \#15 Posted by: dg798 Posted at: 2017-09-11T00:44:01.116Z Reads: 125

```
i did my searching there was no topic that would help me
```

---
## \#16 Posted by: LordChaos Posted at: 2017-09-11T03:06:50.021Z Reads: 122

```
Hey there @dg798

This sounds exactly like my motor did when i got it. My issue was the motor mount screws were shorting the motor out. Try loosening the mounting screws a bit and spinning the motor. If that works file down your mounting screws little by little until they can be tight but not short the motor.

http://www.electric-skateboard.builders/t/motor-stalling-under-load/31584/12?u=lordchaos
```

---
## \#17 Posted by: Clonkex Posted at: 2017-09-11T04:45:19.076Z Reads: 115

```
On a lot of motors you can literally look in the side at the end to see if the screws are touching/close to the windings. #randomTips
```

---
## \#18 Posted by: dg798 Posted at: 2017-09-11T10:48:11.085Z Reads: 108

```
I tried even without the mount but it still didn't work
```

---
## \#19 Posted by: GrecoMan Posted at: 2017-09-11T10:50:26.634Z Reads: 110

```
I already recommended him to try that 😉
```

---
## \#20 Posted by: TarzanHBK Posted at: 2017-09-11T11:14:53.704Z Reads: 101

```
have you tried swapping your phase wires around?
```

---
## \#21 Posted by: GrecoMan Posted at: 2017-09-11T11:20:38.601Z Reads: 100

```
That could be it, make sure the middle wire coming from your motor is plugged into the middle wire of the VESC
```

---
## \#22 Posted by: Namasaki Posted at: 2017-09-11T11:51:49.095Z Reads: 96

```
Check you phase wire connections. 
If one of your phase wires is not connecting, the motor will just shake and studder and fail detection. 
Cold solder joints can cause poor or no connection

If your motor was shorted, you would not be able to spin the motor by hand. It would act like the brakes where on

Also make sure that the circlip on the moto shaft is not rubbing on the mounting plate. 

If you have sensors connected. Try detection without sensors.
```

---
## \#23 Posted by: dg798 Posted at: 2017-09-11T13:00:19.556Z Reads: 91

```
Already tried swapping the phase wires, still didn't work
```

---
## \#24 Posted by: dg798 Posted at: 2017-09-11T13:00:40.696Z Reads: 89

```
And how do I move the circlip
```

---
## \#25 Posted by: dg798 Posted at: 2017-09-11T13:05:00.587Z Reads: 87

```
This is what my motor does
https://photos.app.goo.gl/fGEeWqDd4vsdZUK63.
Listen to the sound it makes
```

---
## \#26 Posted by: Namasaki Posted at: 2017-09-11T13:49:49.241Z Reads: 82

```
I already watched the video
I didn't say to swap the phase wires. 
I said to check the connections for cold solder joints. 
If the circlip is rubbing on the plate, you don't move the circlip, you have to grind the slot in the plate larger so it clears.
```

---
## \#27 Posted by: dg798 Posted at: 2017-09-11T15:32:57.450Z Reads: 81

```
Oh ok but that didn't work either
```

---
## \#28 Posted by: Namasaki Posted at: 2017-09-11T15:41:20.055Z Reads: 81

```
How did you check them?
```

---
## \#29 Posted by: dg798 Posted at: 2017-09-11T17:18:31.208Z Reads: 82

```
No I meant I checked the circlip. I don't know how to check phase wires
```

---
## \#30 Posted by: Namasaki Posted at: 2017-09-11T17:42:49.561Z Reads: 84

```
I believe your problem is a bad connection in one of the phase wires. 
You'll need shrink tube and a hot air gun. 
Remove the shrink tube from the connectors on the Vesc wires and the motor wires. 
Then take pics of them and post so we can see
You can sometimes find the bad connection by holding each wire while twisting and pulling on the connectors. If one of them breaks loose, then you have the culprit.
```

---
## \#31 Posted by: dg798 Posted at: 2017-09-11T18:42:13.339Z Reads: 82

```
It's not my vesc because this one is brand new and it's also my second one because my first one did the same thing. When I get home I will see if I can post a pic of the motor wires
```

---
## \#32 Posted by: dg798 Posted at: 2017-09-11T18:57:01.713Z Reads: 79

```
@torqueboards
Can you help me here??
```

---
## \#33 Posted by: dg798 Posted at: 2017-09-11T18:57:26.096Z Reads: 79

```
It's the 6355 and it didn't work from the time I took out of the box
```

---
## \#34 Posted by: torqueboards Posted at: 2017-09-11T19:08:26.394Z Reads: 81

```
@dg798 I have no clue who you are. This isn't the proper channel to ask me for help. You can email me at help@ and we'll get you all sorted out.
```

---
## \#35 Posted by: dg798 Posted at: 2017-09-11T22:34:59.004Z Reads: 81

```
I was emailing someone and they stopped responding since last night
```

---
## \#36 Posted by: dg798 Posted at: 2017-09-12T00:55:26.302Z Reads: 80

```
just double checked the phase wires. Everything is good
```

---
## \#37 Posted by: racidon Posted at: 2017-09-12T03:49:31.396Z Reads: 77

```
It could also very likely be that your internal phase wires are **_close_** together before the windings

This can mean that turning by hand it isn't a big issue, but once some power is sent down the phase wires it can arc out and start jumping between phases

Another possibility is that your phase wire insulation is cut around the opening of the motor and are shorting on the casing. 

I would check this out by seeing how strong your brake is when applying a slight brake with your VESC. If it's really stiff you definitely have shorted phase wires.

If you get no braking when applying full brake then i will be a bad connection to your phase wires.
```

---
## \#38 Posted by: dg798 Posted at: 2017-09-12T13:02:30.990Z Reads: 74

```
I can't even use the brakes because the motor barely even spins
```

---
## \#39 Posted by: dg798 Posted at: 2017-09-12T15:29:40.037Z Reads: 72

```
The last vesc I had had the drv8302 error after keeping it plugged into the motor for too long. Does that mean that there's a short
```

---
## \#40 Posted by: Hummie Posted at: 2017-09-12T15:37:09.140Z Reads: 72

```
Did u simply try the bldc test on the computer.  Easiest way to see if its shorted in my experience. And it sounds like its not going to pass. Shorted.
```

---
## \#41 Posted by: dg798 Posted at: 2017-09-12T16:47:36.631Z Reads: 72

```
Ok, if it is shorted is there a way to fix it. I mean I haven't even used it yet because it didn't work since I got it
```

---
## \#42 Posted by: telnoi Posted at: 2017-09-13T16:35:56.334Z Reads: 67

```
Send it back to where it came from if it is within the warranty period. It's obviously not your Vesc/what remains is the motor. Fooling around with it will most likely not solve anything and just void your warranty.
```

---
## \#43 Posted by: dg798 Posted at: 2017-09-13T16:49:41.344Z Reads: 66

```
I'm waiting for diyelectricskateboard to get back to me. I have been waiting awhile already.
```

---
## \#44 Posted by: raven Posted at: 2017-09-25T09:02:11.678Z Reads: 60

```
Same here mate jerky motor after programming. It was still ok when first tried it
```

---
## \#45 Posted by: dg798 Posted at: 2017-09-25T16:54:15.120Z Reads: 54

```
I am buying a new one, hopefully it will work.
```

---
## \#46 Posted by: raven Posted at: 2017-09-26T14:54:53.813Z Reads: 47

```
Bad motor joints maybe and check if the esc is built for the motor.
```

---
