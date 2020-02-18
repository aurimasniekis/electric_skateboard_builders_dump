# Braking downhill

### Replies: 44 Views: 876

## \#1 Posted by: DAddYE Posted at: 2018-09-14T19:39:15.330Z Reads: 279

```
Hi all!

I'm having a little issue when braking downhill. I'm using the @Ackmaniac firmware on a fsesc 6.6 and I noticed that when I go downhill I can't decrease the brake pressure. I can only release them. I don't have issues on flat surfaces.

For example, going downhill If I brake 80%, then I release them a little to 60% nothing changes it is still at 80%. If I release them to 0% then I can apply 60%.

Any idea how to fix this?

I’m on FOC, I’m using skullboard hubs 1 (65kv).

Here my specs, motor 60, brakes -40, battery 30, regen -15. I tried brakes from 20-100, and regen from -8 to -15 (it affected brakes only at max speed).

I hope I explained myself lol, it's Friday :smile:
```

---
## \#2 Posted by: Hummie Posted at: 2018-09-14T19:43:04.465Z Reads: 272

```
annoying as fuck!   I bet its your remote.  I had that a lot.  the mini trigger shows the best at not doing this in my experience.  modulation.
```

---
## \#3 Posted by: mackann Posted at: 2018-09-14T19:55:36.341Z Reads: 262

```
Have the same on my raptor 2 sometimes, dunno why
```

---
## \#4 Posted by: DAddYE Posted at: 2018-09-14T19:57:41.596Z Reads: 252

```
Do you think it's the remote? I don't recall having this issue when I was on stock FW. Admittedly I've run the stock one only for few minutes.
```

---
## \#5 Posted by: Hummie Posted at: 2018-09-14T19:58:53.825Z Reads: 244

```
supposedly the remote COULD do huge precision and you could have great control but its lost int the physical interface.  its like grand theft auto and going 200mph and controls that can move an eighth of an inch.  I'm always skidding or crashing in that game.

I think its just a quality of the remote.  try the mini trigger and see.  I think theres some adjustability on the esc but really the problem is the remote.
```

---
## \#6 Posted by: DAddYE Posted at: 2018-09-14T20:02:11.510Z Reads: 230

```
I have the mini trigger, and I don't get why happens only downhill.
```

---
## \#7 Posted by: Benjamin899 Posted at: 2018-09-14T20:27:46.761Z Reads: 212

```
i was braking down a couple of hundred meter downhill at 6% and had no problems rly, i could break harder or soften up to get more speed but no problems, i was running a focbox with a flipsky 4.12 over split ppm with that cheap 15€ mini remote.
```

---
## \#8 Posted by: DAddYE Posted at: 2018-09-14T20:31:26.885Z Reads: 207

```
Did you use the stock firmware or the ackmaniac?
```

---
## \#9 Posted by: Benjamin899 Posted at: 2018-09-14T20:33:15.765Z Reads: 197

```
ackmaniac yes, never had anything else. motor -60 and battery regen -8 each
```

---
## \#10 Posted by: Ackmaniac Posted at: 2018-09-14T20:46:53.479Z Reads: 185

```
What's your motor and battery min and max?
```

---
## \#11 Posted by: DAddYE Posted at: 2018-09-14T20:57:03.614Z Reads: 180

```
I'm on FOC, I'm using [skullboard hubs](https://www.skullboardvip.com/collections/accessories/products/dual-hub-motor-truck-kit) (65kv).

Here my specs, motor 60, brakes -40, battery 30, regen -15. I tried brakes from 20-100, and regen from -8 to -15 (it affected brakes only at max speed).

Thanks mate!
```

---
## \#12 Posted by: Benjamin899 Posted at: 2018-09-14T21:03:42.456Z Reads: 170

```
how big is your battery?
```

---
## \#13 Posted by: DAddYE Posted at: 2018-09-14T21:25:49.427Z Reads: 164

```
Sanyo 10s2p
```

---
## \#14 Posted by: Ackmaniac Posted at: 2018-09-14T21:52:25.407Z Reads: 165

```
-15 Amps for each FOCBOX results in -30A in total for the battery for your dual setup. Your battery is only recommended for 8A (i mostly recommend to set the max 50% higher for stronger brakes). But your battery is just too weak for that power. So when you brake i guess the battery overshoots already quite a lot. So the FOCBOX works then at the amp and voltage limits. And even of you reduce the throttle a bit you still overstressed the system already so that it still works on the limit. Once you release the throttle and brake again the battery has a short moment to breathe and works better then.
But that's only a guess.
Best would be you make a video with my app to see the relatime data while riding. By that we can have a very detailed look what is going on.
```

---
## \#15 Posted by: DAddYE Posted at: 2018-09-15T00:00:51.533Z Reads: 149

```
Oh I see! I’m going to try with a 12s2p Samsung 30q and see if it’s better. 

Here is my ride: https://metr.at/r/DMkl7

Thanks mate!
```

---
## \#16 Posted by: DAddYE Posted at: 2018-09-15T02:46:07.842Z Reads: 143

```
Another thing, the discharge rate for Sanyo 20700B is 15A according to the specs. 2p means I can do regen -15a on each vesc, Am I wrong?
```

---
## \#17 Posted by: telnoi Posted at: 2018-09-15T03:10:10.844Z Reads: 141

```
Discharge does not equal charge. These are different numbers.
```

---
## \#18 Posted by: DAddYE Posted at: 2018-09-15T03:21:57.085Z Reads: 141

```
[quote="DAddYE, post:16, topic:68045"]
Sanyo 20700B
[/quote]

According to this: https://liionwholesale.com/products/panasonic-sanyo-ncr20700b?variant=30186936017
They have a max Continuous Discharge Current of 15A
```

---
## \#19 Posted by: telnoi Posted at: 2018-09-15T03:37:48.570Z Reads: 134

```
It's around 2A/listed as normal charge rate.
```

---
## \#20 Posted by: dareno Posted at: 2018-09-15T05:41:25.442Z Reads: 125

```
Does it do it all the time or just on full charge downhill?  Could be over voltage.  That causes strange braking anomalies.
```

---
## \#21 Posted by: DAddYE Posted at: 2018-09-15T05:54:56.209Z Reads: 119

```
It does it all the times
```

---
## \#22 Posted by: dareno Posted at: 2018-09-15T06:18:01.588Z Reads: 112

```
Then follow @Ackmaniac advice.  Just thought I'd see if it was something simple.  Good luck with it
```

---
## \#23 Posted by: Benjamin899 Posted at: 2018-09-15T07:32:08.756Z Reads: 111

```
damn, everbody was hyping these sanyo but gotta be honest, 2a per cell recommended max charge is quite limiting, even the 30q can take 4a per cell.
```

---
## \#24 Posted by: michaelcpg Posted at: 2018-09-15T07:59:03.082Z Reads: 104

```
I had the same issue with my original Maytech remote
```

---
## \#25 Posted by: DAddYE Posted at: 2018-09-16T19:51:02.250Z Reads: 94

```
So being a 10s2p I should be at -10 or -8 on each VESC?
```

---
## \#26 Posted by: dareno Posted at: 2018-09-16T20:09:05.881Z Reads: 96

```
[quote="Benjamin899, post:23, topic:68045"]
damn, everbody was hyping these sanyo
[/quote]

They are a better option when buying the boards associated with them, meepo/wowgo etc but definitely not compared to 30q.
```

---
## \#27 Posted by: telnoi Posted at: 2018-09-17T05:51:12.244Z Reads: 86

```
P count * max charge amp : 2.

Just 2A for each vesc. 4 will probably also work, but that is twice as much as the recommended charge rate.
```

---
## \#28 Posted by: Hummie Posted at: 2018-09-17T06:01:44.871Z Reads: 86

```
I think you can put much more in for short periods as apposed to a stated continuous charge rate for all states of charge.
https://chargedevs.com/newswire/self-healing-anode-eliminates-dendrite-buildup/
```

---
## \#29 Posted by: telnoi Posted at: 2018-09-17T06:56:48.520Z Reads: 81

```
I really should get telemetry. I wonder what happens during one of my off-road downhill sessions where I am constantly on the brake. This sometimes lasts up to 5 minutes.
```

---
## \#30 Posted by: DAddYE Posted at: 2018-09-17T12:26:55.795Z Reads: 75

```
Will still have brakes at -4a each?
```

---
## \#31 Posted by: telnoi Posted at: 2018-09-17T12:32:46.225Z Reads: 76

```
Yes. I used 4 in the past. As always, test under safe conditions, but try to find a spot that would correspond to your normal road conditions. Don't go blasting down a busy city street immediately :sweat_smile:
```

---
## \#32 Posted by: boramiNYC Posted at: 2018-09-17T17:16:34.547Z Reads: 70

```
I observed the same thing with my brakes using 3.1 firmware and Akimaniacs tools, and NanoX remote. Dont know whats causing it but it seems the fw. Before, when I was on 2.14 FW and firefly remote and the brake was smooth at any speed coming down a steep hill. Now I have to release before I can change to weaker braking power.
```

---
## \#33 Posted by: DAddYE Posted at: 2018-09-17T18:29:01.305Z Reads: 68

```
Ok, I lowered it to -4A each, and I still have the same issue. I also got a DRV302 -_-, but everything seems working. Any idea why? See my metr.at here: [https://metr.at/r/xI7ah](https://metr.at/r/xI7ah)

I'm going to try the stock one this afternoon or tomorrow to compare the differences.
```

---
## \#34 Posted by: Benjamin899 Posted at: 2018-09-17T19:03:03.084Z Reads: 66

```
Here is me braking with ackmaniac Tool. I can freely increase or decrease.
https://youtu.be/eR1x8Tq3iU0
```

---
## \#35 Posted by: DAddYE Posted at: 2018-09-18T18:07:59.307Z Reads: 59

```
Seems that on my case is an issue with the @ackmaniac's firmware. I ran stock today and was working without DRV errors, a better torque, and finally, I'm able to brake downhill. I think I might have hit some kind of bug in the code because everyone usually prefers @Ackmaniac fw. 

Here my very slow/safe runs:

https://metr.at/r/tdHbR
https://metr.at/r/Sr69a
```

---
## \#36 Posted by: Benjamin899 Posted at: 2018-09-18T18:43:34.635Z Reads: 53

```
thats great to hear, but i want to know, what settings did you use with akmaniacs firmware.
```

---
## \#37 Posted by: DAddYE Posted at: 2018-09-18T19:48:15.193Z Reads: 51

```
Same sensored foc and same motor (30/-30) battery (30/-4)
```

---
## \#38 Posted by: Benjamin899 Posted at: 2018-09-18T19:50:54.553Z Reads: 52

```
how many watts?
```

---
## \#39 Posted by: DAddYE Posted at: 2018-09-18T19:55:37.717Z Reads: 54

```
With the defaults for a 10s
```

---
## \#40 Posted by: Benjamin899 Posted at: 2018-09-18T20:26:24.364Z Reads: 52

```
talking about the settings in the ackmaniac tool. for example i set my motors to max 1260 watts.
```

---
## \#41 Posted by: DAddYE Posted at: 2018-09-18T20:32:18.770Z Reads: 49

```
Sorry! I had 15000.0W which essentially disables it.
```

---
## \#42 Posted by: Benjamin899 Posted at: 2018-09-18T20:33:35.769Z Reads: 49

```
thats kinda the point of the firmware^^
```

---
## \#43 Posted by: DAddYE Posted at: 2018-09-18T21:49:18.664Z Reads: 46

```
I see... it might have issues if not set to a proper value?
```

---
## \#44 Posted by: Benjamin899 Posted at: 2018-09-19T08:16:26.622Z Reads: 36

```
Well IT actually shouldn't. But it has an effect on the Motor behaviour. It smoothes the throttle and braking over the length of the Trigger.
At the end of @ackmaniac Post He explained it Well.
```

---
