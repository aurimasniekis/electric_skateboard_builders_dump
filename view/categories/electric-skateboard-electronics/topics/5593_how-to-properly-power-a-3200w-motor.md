# How to properly power a 3200W motor

### Replies: 35 Views: 2883

## \#1 Posted by: Brando Posted at: 2016-07-05T12:47:51.205Z Reads: 206

```
I am planning out my first build and was looking at buying DIY's 3200W motor. Would I be able to run this motor off a 6S battery or do I need to find a smaller motor?
```

---
## \#2 Posted by: JLabs Posted at: 2016-07-05T12:50:08.978Z Reads: 205

```
You would be able to run it on 6s with no problems. You would just be getting half the fun running 6s😁
```

---
## \#3 Posted by: Brando Posted at: 2016-07-05T13:13:47.071Z Reads: 198

```
Thanks for the quick reply, i'm so new to all of this. So would a 12S battery only give more range, or would it also increase torque and speed?
```

---
## \#4 Posted by: Nordle Posted at: 2016-07-05T13:19:52.567Z Reads: 191

```
Increase of top speed - yes.
Not more torque, but less amps for the same amount of torq (=cooler esc & battery)
as always please correct me if i'm wrong:)
```

---
## \#5 Posted by: Hillso Posted at: 2016-07-05T13:28:07.101Z Reads: 182

```
If you will use the VESC you will able to pull max 1260W continuously on 6s.
you need 125A ESC to pull 3200 on 6s
```

---
## \#6 Posted by: Brando Posted at: 2016-07-05T13:29:45.223Z Reads: 175

```
can you tell me how you calculated that?
```

---
## \#7 Posted by: Hillso Posted at: 2016-07-05T13:31:15.656Z Reads: 171

```
VESC 50A * 6s * 4.2V = 1260W
3200W / 6s * 4.2V = 126A

and 3200W will discharge space cell within 10 minutes
of course it doesn't mean you will use 3200W even if you can, only if you go 50 mph or very steep hill, depends also on the control type
```

---
## \#8 Posted by: Brando Posted at: 2016-07-05T13:33:59.940Z Reads: 164

```
ahh, ok. So I plan to start out with a 6S battery (may upgrade to 12s down the road) and Enertion's VESC. Do you have any motor recommendations? It sounds like the 3200W is overkill.
```

---
## \#9 Posted by: Hillso Posted at: 2016-07-05T13:36:59.152Z Reads: 160

```
lol I bought 2700W motor and 8s battery and I can use only 1700W. still very powerful and i weigh 55kg.

I don't know if what i'm saying is true so wait for the professionals for recommendations
```

---
## \#10 Posted by: Brando Posted at: 2016-07-05T13:39:48.554Z Reads: 155

```
Thanks so much, quick question, where did you get 4.2V from? I'm looking at two zippy 3S 5000mah 11V and I would put both in series. I believe that would be 22V
```

---
## \#11 Posted by: Hillso Posted at: 2016-07-05T13:45:18.590Z Reads: 150

```
I think I saw chaka calculate at 4.2V. It is the max V on single cell Lipo.
btw why only 6s? you can get [12s for 100$](http://www.aliexpress.com/item/14-8V-5500mAh-Floureon-4S-40C-RC-Lipo-Battery-for-RC-Helicopter-Quadcopter-Car-Hobby-Bateria/32573290438.html?spm=2114.13010608.0.57.GuuWHh). so you can get 2500W,only if you want, it is very powerful and not necessary depends on your weight and if you want to ride hills.

You can maybe buy the batteries even cheaper if you buy from them hobbyking.
```

---
## \#12 Posted by: Maxid Posted at: 2016-07-05T13:48:39.668Z Reads: 142

```
The space cell has a 40A fuse as far as i know - so you can't even use it in this case.
```

---
## \#13 Posted by: Hillso Posted at: 2016-07-05T13:51:18.875Z Reads: 142

```
you will get the max watt using the max voltage. And there is also max rpm, I think its 170kv for 12s (on v4 VESC).
```

---
## \#14 Posted by: Stevemk14ebr Posted at: 2016-07-05T15:57:22.407Z Reads: 135

```
Watts = voltage * amps

12s = 4.2v * 12 cells gives 50.2 volts
6s = 4.2v * 6 cells gives 25.2 volts

3200w = 50.2 * amps 
Amps = 63.7 amps motor draw on 12s

3200w = 25.2 * amps
Amps = 126.7amps motor draw on 6s

You will want a 150a esc at least if you run at 6s. If at 12s then you can run 80a esc or lower. If you use the vesc you need to make sure the motor kv is below ~180 if you go with 12s.

Note that the amp draw numbers i gave are theoretical max, in reality it will never be this high but you always want to overspec when you run at such high amps and volts as we do.
```

---
## \#15 Posted by: Brando Posted at: 2016-07-05T16:06:52.776Z Reads: 138

```
Is there an esc you would recomend for the 6S settup? Or should I just get a 12s settup?
```

---
## \#16 Posted by: Hillso Posted at: 2016-07-05T16:23:46.277Z Reads: 133

```
keep in mind that if you use 12s it might be harder to charge
```

---
## \#17 Posted by: chaka Posted at: 2016-07-05T16:32:30.127Z Reads: 133

```
You can use a hobbywing ezrun if you want to build a single drive with a motor this large. The vesc is not going to give you that much wattage without overheating. The Hobbywing esc's can handle a ton of throughput without overheating but the throttle is too snappy for some riders. It can be sketchy.

 If you want a plush throttle curve you can use the vesc if you are only using burst currents but any continuous watt usage that high is going to trigger the over-temp cutoff. 

You could use two of these motors and use the vesc without triggering the overheat function. You would have really high torque and excellent hill climbing but it would be expensive.
```

---
## \#18 Posted by: Hummie Posted at: 2016-07-06T05:47:26.368Z Reads: 120

```
I think you can use one big motor and two smaller controllers. What's to stop someone from splitting the motor wires to 6 and using two escs?
```

---
## \#19 Posted by: trbt555 Posted at: 2016-07-06T11:58:37.385Z Reads: 113

```
Will not work.
No sync between the controllers.
```

---
## \#20 Posted by: Hummie Posted at: 2016-07-06T17:50:25.311Z Reads: 100

```
What would they need to be in synch?i thought they could operate independently but overlapping their feeding to the motor.
```

---
## \#21 Posted by: Stevemk14ebr Posted at: 2016-07-07T03:06:09.692Z Reads: 90

```
you can use two slightly out of sync motor controllers at the same time, rc plane guys do it all the time. Just get a Y splitter on the signal wire like torqueboards uses for his dual 120a esc.
```

---
## \#22 Posted by: trbt555 Posted at: 2016-07-07T10:19:17.396Z Reads: 84

```
2 ESC's to drive one motor ? Didn't know that worked.
I still think it's a recipe for magic smoke.
```

---
## \#23 Posted by: DerBrecher Posted at: 2016-07-07T11:39:35.281Z Reads: 77

```
I agree with @trbt555 the timing of the output of an ESC must be very precise. I cant imagine that two esc can be sync this perfectly. But i could be wrong.

RC Guys use two Motors and one ESC but this is a completely differnt story.
```

---
## \#24 Posted by: GhettoFab.rictation Posted at: 2016-07-07T11:51:21.695Z Reads: 75

```
If you used one remote and used y connector at the receiver and ran the connection to both esc it would work, with enough juice from the battery that is
```

---
## \#25 Posted by: GhettoFab.rictation Posted at: 2016-07-07T11:52:04.171Z Reads: 75

```
Obviously same esc's, have to run the receiver in parallel to the escs and possibly get voltage cut off separate from bec
```

---
## \#26 Posted by: trbt555 Posted at: 2016-07-07T12:48:18.941Z Reads: 73

```
Splitting the ppm signal will not guarantee the esc's are synced.
Someone please try this and make a video.
I like fireworks :slight_smile:
```

---
## \#27 Posted by: Stevemk14ebr Posted at: 2016-07-07T13:27:31.567Z Reads: 70

```
@trbt555 just ask @torqueboards this is how he does his dual motor configs.
```

---
## \#28 Posted by: trbt555 Posted at: 2016-07-07T15:22:26.345Z Reads: 67

```
Dual motor configs with two escs per motor ? That I gotta see.
Are you sure you've been paying attention ?
```

---
## \#29 Posted by: Stevemk14ebr Posted at: 2016-07-07T15:38:35.398Z Reads: 65

```
Im talking about 2 motors, each with their own esc but the escs are slightly out of sync. Idk what u guys are talking about
```

---
## \#30 Posted by: Hummie Posted at: 2016-07-07T15:43:32.507Z Reads: 64

```
Maybe it needs the 6 leads connected to a unique wiring in the motor.  I've seen it done but think this is how they did it.  We're talki about 2 esc one motor. If u have a large motor and small escs I guess..for when you spent all ur money and they don't take returns or exchanges maybe.
```

---
## \#31 Posted by: trbt555 Posted at: 2016-07-07T16:30:43.166Z Reads: 60

```
This:
[quote="Hummie, post:18, topic:5593, full:true"]
I think you can use one big motor and two smaller controllers. What's to stop someone from splitting the motor wires to 6 and using two escs?
[/quote]

I still think it won't work. A brushless esc creates a rotational field in the windings of the motor by cyclicly modulating the phase voltages. If the phase voltages of both escs are not in prfectly in sync, you'll get currents flowing from one esc to the other instead of through the motor which will at the very least screw up your motor sync and in worst case fry one or both esc's.
```

---
## \#32 Posted by: Hummie Posted at: 2016-07-07T16:33:24.338Z Reads: 58

```
I think the wires in the motor had it so there were 6 phases and pretty much equaled the wiring of two motors inside the single motor
```

---
## \#33 Posted by: Nordle Posted at: 2016-07-07T16:34:14.589Z Reads: 60

```
Maybe you've seen a ESC which can switch also from star to delta, this would require every 2 ends of the 3 phases, wich would result into 6 leads from the motor to still one esc.
```

---
## \#34 Posted by: Hummie Posted at: 2016-07-07T16:38:33.333Z Reads: 59

```
Can u link a switching esc?  That would be a super feature for the vesc, someone surely has asked for that already
```

---
## \#35 Posted by: Nordle Posted at: 2016-07-07T16:58:01.057Z Reads: 56

```
Lol nope, i only doubt thats something possible could exist already. But looks like _(..google..)_ there's no such thing :sweat_smile:
[stupid wye-delta switch](https://www.google.it/imgres?imgurl=http%3A%2F%2Fepub1.rockwellautomation.com%2Fimages%2Fweb-proof-large%2FGL%2F1244996.jpg&imgrefurl=http%3A%2F%2Fwww.ab.com%2Fen%2Fepub%2Fcatalogs%2F12768%2F229240%2F229254%2F3170945%2F229537%2FIntroduction.html&docid=wbuSfGElLLUfVM&tbnid=wwnyTSpsvQKnKM%3A&w=302&h=289&bih=637&biw=1280&ved=0ahUKEwjpgoep5-HNAhXJVhQKHSFvD7IQMwgfKAMwAw&iact=mrc&uact=8)
only this :stuck_out_tongue_winking_eye:
```

---
