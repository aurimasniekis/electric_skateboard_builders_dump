# Overheating Issue FIXED!?!? ENERTION MOTOR 6372 REPLACED

### Replies: 39 Views: 3015

## \#1 Posted by: joeadams101 Posted at: 2016-08-14T19:45:37.825Z Reads: 216

```
Hello guys, after weeks of re-searching, headeches and frustration I finally fixed the overheating on my board! If you want to read the original post : http://www.electric-skateboard.builders/t/update-not-enough-power-or-lost-of-it-enertion-build/7104/79. I asked for help many times and I got a lot of feed back but those options didn't work. I messaged @chaka because I saw he had a store and he was actively helping others. He assured me that Your VESC is overheating due to the motor pulling a lot of amps. I refused to understand because Enertion tells you that setup will work! I decided to give another expert a shot and bought @chaka's 170kv motor ( http://www.ollinboardcompany.com/product/om5065-170kv) , he was very professional even showed me a video of his motor climbing hillls with no problem. I switched out the motor and did the same 4 mile trail I could never finish with my Enertion 6372 motor due to loose of power and....BAM I was successful, not even a single mph less on every steep hill I did, I even challenged it with 5 super steep hills one after the other and nothing! Maintain a  steady speed of 16-18 mph. Again, I want to thanks @chaka for taking the time and troubleshooting me through this and for making me understand what was wrong and proving me with a solution! Thanks for everyone who gave solutions and tried to help me as much as they could ! @Jinra Thanks for everything! 

Yesterday the temperature outside was 98 F today is 101 F...


I MADE IT!


  <img src="/uploads/db1493/original/2X/4/46c8e5bfe7c830b11e12fbc469fb7a58c0515f71.jpg" width="375" height="500">

<img src="/uploads/db1493/original/2X/5/5f140976d43eeff8e606c1bcb9219044af5138a3.jpg" width="375" height="500">


Here is the Video with Ollin 170kv Motor:

https://youtu.be/BV9DU8jl0CU

Here is the Video with Enertion 6372 R Spec Motor: 

https://www.youtube.com/watch?v=4CVONzfYRjM
```

---
## \#2 Posted by: petmakris Posted at: 2016-08-14T20:21:32.198Z Reads: 199

```
[quote="joeadams101, post:1, topic:7640"]
was successful, not even a single mph less on every steep hill I did, I even challenged it with 5 super steep hills one after the other and nothing! Maintain a  steady speed of 16-18 mph. Again, I want to thanks @chaka for taking the time and troubleshooting me through this and for making me understand what was wrong and proving me with a solution! Thanks for everyone who gave solutions and tried to help me as much as they could ! @Jinra Thanks for everything!
[/quote]

I don't get it , it was the motor by itself that solved the problem? No overheating?
```

---
## \#3 Posted by: Jinra Posted at: 2016-08-14T20:22:51.553Z Reads: 189

```
Honestly, it shouldn't be overheating with the 6372 in the first place. My guess is something's wrong the motor and perhaps it's shorting out still.
```

---
## \#4 Posted by: chaka Posted at: 2016-08-14T21:00:46.427Z Reads: 182

```
I can tell you from my own personal experience with a 6372 200kv motor from maytech that it will indeed overheat the VESC on hills regardless of amp settings in a single drive configuration. I have been saying this for awhile now and I am sure we will see more proof in the future since there are many others with this single motor configuration. 

Like I said in the past, it has been long established that your motor controller should be matched to your motor. If the motor pulls too many amps it will overheat you motor controller. 

In any case it is very fortunate that the original motor was not shorting out otherwise his VESC would have been fried!
```

---
## \#5 Posted by: furryfrog Posted at: 2016-08-14T21:01:24.630Z Reads: 179

```
Glad you have it sorted out. Do you happen to have a multimeter? Have you or can you do a resistance check on your motor you were having problems with? Can you check the resistance between the 3 power leads,( 3 measurements) and each lead to the ground (case of the motor). Just wondering if these measurements would indicate a problem? Any tests a guy can do to diagnose a faulty motor like yours, without just swapping it out to see what happens?

Regards
```

---
## \#6 Posted by: furryfrog Posted at: 2016-08-14T21:05:44.027Z Reads: 167

```
Ok, so in this case it is not a faulty motor, just the wrong motor for the application?
```

---
## \#7 Posted by: Michaelinvegas Posted at: 2016-08-14T21:07:04.700Z Reads: 167

```
[quote="chaka, post:4, topic:7640"]
Like I said in the past, it has been long established that your motor controller should be matched to your motor. If the motor pulls too many amps it will overheat you motor controller.
[/quote]

This a 100% true 

Too bad we are a bunch of hacks lol

But guidelines for VECS needs help from the community ... Can't expect @chaka and the like to test every motor in the market and how it reacts to the VECS under certain circumstances.  Problem is who's gonna collect the data and maintain it?
```

---
## \#8 Posted by: Jinra Posted at: 2016-08-14T21:07:55.995Z Reads: 155

```
If this was true, shouldn't the Raptor Mono overheat as well?
```

---
## \#9 Posted by: chaka Posted at: 2016-08-14T21:12:14.794Z Reads: 150

```
I'm sure it does if you try to climb long hills.  On the flats these motors perform fine as long as you don't do a lot of repeated hard accelerations. You could probably get away with it with more gear reduction too. Figure a 20mph top speed?
```

---
## \#10 Posted by: Michaelinvegas Posted at: 2016-08-14T21:14:59.523Z Reads: 154

```
[quote="Jinra, post:8, topic:7640, full:true"]
If this was true, shouldn't the Raptor Mono overheat as well?
[/quote]

IMO we really wouldn't know unless we send @joeadams101 a Raptor to do a comparo on the same hills he's riding 

The boards need to be pushed to the same extreme...anything else would be just educated guesses
```

---
## \#11 Posted by: Jinra Posted at: 2016-08-14T21:15:41.349Z Reads: 154

```
It's really the exact same board. Enertion motor, Enertion drive train, VESC, Space Cell.. The only difference would be the VESC parameters, which seemed fine, and the quality of the build.
```

---
## \#12 Posted by: Michaelinvegas Posted at: 2016-08-14T21:16:20.716Z Reads: 150

```
And the same settings as Enertion too?
```

---
## \#13 Posted by: Michaelinvegas Posted at: 2016-08-14T21:17:35.003Z Reads: 148

```
See now VESC settings are an important factor too
```

---
## \#14 Posted by: Jinra Posted at: 2016-08-14T21:18:10.868Z Reads: 143

```
They are, which is why he went over them a TON in his main thread. None of the adjustments helped.
```

---
## \#15 Posted by: Jinra Posted at: 2016-08-14T21:19:34.896Z Reads: 145

```
chaka's probably right though, too much of a hill for too long may be building too much heat on the 63mm motor.
```

---
## \#16 Posted by: Michaelinvegas Posted at: 2016-08-14T21:19:55.097Z Reads: 144

```
But let's be honest...just because he had this experience doesn't mean this is a issue with everyone...till there is more people coming forward with this issue .... Would assume this may be an isolated issue.
```

---
## \#17 Posted by: Michaelinvegas Posted at: 2016-08-14T21:21:16.284Z Reads: 135

```
Yeah maybe...but def some more feed back from others before a label gets put on
```

---
## \#18 Posted by: whitepony Posted at: 2016-08-14T21:30:23.945Z Reads: 137

```
probably mostly a KV thing here tbh. same experience I made - 190KV overheats the vesc uphill, same hill with 168KV is just fine.

the very same effect is achieved by changing the gearing. while 190KV kept overheating the vesc with 16/36T on my daily commute hill, the same motor with 15/36T runs up that hill without an issue.

its kind of a no brainer. to get your weight up a hill, you need a certain amount of torque - a lower KV motor will achieve the same torque as a higher KV motor, but at a lower current =  less heat. same effect with the gearing - to generate the same amount of torque, the motor will turn faster with less motor torque = less current = less heat in the vesc.
```

---
## \#19 Posted by: chaka Posted at: 2016-08-14T21:50:18.811Z Reads: 140

```
Reducing kv or reducing the gear ratio produces roughly the same result but...I can take a 200kv 5065 and plow up hills that would lead to overheating if I used a 6372 200kv on the same drive ratio. Its a very simple topic really, common knowledge among the rc crowd. Running a motor too big for your motor controller will lead to problems.
```

---
## \#20 Posted by: Michaelinvegas Posted at: 2016-08-14T22:22:37.255Z Reads: 145

```
Need to super size a VESC then...no?
```

---
## \#21 Posted by: Michaelinvegas Posted at: 2016-08-14T22:23:47.520Z Reads: 147

```
[quote="whitepony, post:18, topic:7640"]
probably mostly a KV thing here tbh.
[/quote]

Yep agreed if all else the same
```

---
## \#22 Posted by: Eboostin Posted at: 2016-08-14T23:26:51.712Z Reads: 139

```
Curious as to why a 170kv was suggested on this 10s setup? Everything I keep reading regarding your motors says 200kv for 10s and 170kv for 12s.

Was this just because the OP wanted to primarily climb hills?

I ask as a potential and probable buyer. :)
```

---
## \#23 Posted by: Michaelinvegas Posted at: 2016-08-15T00:18:43.274Z Reads: 130

```
Torque is what he needed for his needs ... Prob would have close to the same issues with the 200kv version
```

---
## \#24 Posted by: sl33py Posted at: 2016-08-15T00:40:13.784Z Reads: 127

```
First off - congrats on the new setup and that it's working well for you!

The logic makes sense, but seems a bit backwards to me.  I'd think the larger motor should have more power (more magnets and surface area - especially the 72mm long one vs 55mm one), as well as more cooling surface area?!?

I'm really impressed w/ Ollin's offerings and seems like some pretty impressive service to boot.

Again - glad you got this sorted and working well for you!  It's likely in the original thread, but how heavy are you?  and do you know the grade of that hill in the videos?
```

---
## \#25 Posted by: chaka Posted at: 2016-08-15T01:04:20.042Z Reads: 122

```
@Eboostin I recommended the 170kv because a single 200kv motor might get a little hot with his current gear ratio. Speaking of the motor overheating and not the VESC. This was the easiest solution for him. 

@sl33py A smaller motor will "pull" less amps when encountering a load large enough to stall the motor. When you encounter this in larger motors the current demand can easily exceed what the VESC can dissipate resulting in an overheating event.
```

---
## \#26 Posted by: Jinra Posted at: 2016-08-15T01:07:54.591Z Reads: 119

```
[quote="chaka, post:25, topic:7640"]
a single 200kv motor might get a little hot with his current gear ratio
[/quote]

No kidding, haha
```

---
## \#27 Posted by: chaka Posted at: 2016-08-15T01:16:09.015Z Reads: 121

```
Same would happen with a single 6372 200kv motor if the VESC could handle load. My 200kv maytech got so hot the magnets came loose!
```

---
## \#28 Posted by: Jinra Posted at: 2016-08-15T01:17:20.064Z Reads: 119

```
I believe it, just crazy how hot these motors can get.
```

---
## \#29 Posted by: chaka Posted at: 2016-08-15T01:23:16.618Z Reads: 123

```
It will be interesting to see what difference ceramic bearings will make. It would be nice if we can isolate the heat to the stator and motor mount. We could then work on air cooled and eventually water cooled mounts!
```

---
## \#30 Posted by: Michaelinvegas Posted at: 2016-08-15T01:33:18.832Z Reads: 124

```
That's some tiny plumbing right there
```

---
## \#31 Posted by: Randyc1 Posted at: 2016-08-16T01:32:21.427Z Reads: 109

```
If a Single 5065 Motor can perform better on a Hill than a 6372,... what use is there for the Larger 63mm motors in E-skate.??
```

---
## \#32 Posted by: monkey32 Posted at: 2016-08-16T01:44:46.236Z Reads: 109

```
What are your specs kg/lbs that caused the 6372 to overheat?
```

---
## \#33 Posted by: chaka Posted at: 2016-08-16T01:48:09.880Z Reads: 106

```
It is actually the vesc that was overheating. When V6 is finished these big motors will work much better on hills. I still like using large motors with high end rc car esc's. Lower voltage but lots of torque!
```

---
## \#34 Posted by: Randyc1 Posted at: 2016-08-16T02:10:49.843Z Reads: 106

```
Will the new V6 have have all the advantages the RC esc's have for torque ?
```

---
## \#35 Posted by: michaelcpg Posted at: 2016-08-16T02:13:03.631Z Reads: 111

```
My VESC overheats on long steep hills with my single Enertion 6374. Wasn't really an issue on FOC but after having to get my DRV chip replaced, I'm now sticking to BLDC which obviously seems to produce more heat.
```

---
## \#36 Posted by: chaka Posted at: 2016-08-16T02:22:14.149Z Reads: 111

```
It should be capable of enough throughput to put a lot of ESC's to shame! Hopefully Vedder will be finished with the firmware changes soon and we can get it into beta production.
```

---
## \#37 Posted by: michaelcpg Posted at: 2016-08-16T02:26:59.039Z Reads: 119

```
Do you expect there will likely be much in the way of power efficiency improvements over the v4.x models? Still contemplating whether to buy another v4.x model or buy 2 v6 models when they're finally ready...
```

---
## \#38 Posted by: chaka Posted at: 2016-08-16T04:16:06.304Z Reads: 128

```
The only thing I know for certain is they will handle more throughput and should be more resilient. Don't want to speculate too much at this point.
```

---
## \#39 Posted by: b-rad Posted at: 2016-10-11T04:52:54.596Z Reads: 75

```
I actually have this exact same issue but i solved it differently. My setup was a 190 kv enertion 6355, vesc, enertion drive train (16/36), 12s lipo. I tried to tweak with the vesc settings but everytime i would go up a long steep hill i would eventually just go like 2 mph or stall out, and the same thing would happen even if i kept accelerating up and down flat streets (more than 3 times up and down a 50 yard street, accelerating normally after complete stop the vesc needed a break to cool down), i would be pressing the trigger full throttle and id be only going a quarter of the full speed. I got super annoyed and just put my TB 12S ESC on my setup and got rid of the vesc and now everything works normal again. I feel as if it wasnt the motor, it was the vesc.
```

---
