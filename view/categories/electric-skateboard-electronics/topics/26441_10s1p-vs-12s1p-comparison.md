# 10s1p vs 12s1p Comparison

### Replies: 24 Views: 2400

## \#1 Posted by: ShutterShock Posted at: 2017-06-30T14:47:51.108Z Reads: 257

```
I've been reading quite a bit in the forums and online, but I can't seem to answer the question that I currently have.

I haven't decided if I am gonna do 12s or 10s quite yet, and I currently have basically two options that I;m looking at.

1st option is doing 4x [3s1p 5000mah 20C](https://hobbyking.com/en_us/turnigy-5000mah-3s-20c-lipo-pack.html) lipo cells in series to get 12s

2nd, which is the one I have planned for since the beginning, is to do 2x [5s1p 5000mah 25C](https://hobbyking.com/en_us/zippy-compact-5000mah-5s-25c-lipo-pack.html) lipo cells in series to get 10s.

I know that with 12S I will be able to go faster, but will I get more range with that 12s setup since there are more mah's overall?

1x 190kv motor, approx 145lb rider, VESC
```

---
## \#2 Posted by: Michael319 Posted at: 2017-06-30T15:01:12.402Z Reads: 251

```
For a 12s battery you don't want a motor any higher than 170kv. It makes the ERPM over 60,000 which is bad news.
```

---
## \#3 Posted by: Eboosted Posted at: 2017-06-30T15:20:39.442Z Reads: 232

```
Against the comon forum consensus, I run 190kv on 12S and 230kv on 10S, I've never exceeded max ERPM, board runs faster and feels amazing!
```

---
## \#4 Posted by: Jinra Posted at: 2017-06-30T15:47:27.389Z Reads: 215

```
That's because 190kv on 12s and 230kv on 10s  is fine. They do not go over erpm limits in real riding scenarios (unless you're going downhill obviously).
```

---
## \#5 Posted by: ShutterShock Posted at: 2017-06-30T15:50:43.826Z Reads: 208

```
Wait so if I was going downhill with the throttle off, would I have a problem?  I don't wanna accidentally fry my electronics
```

---
## \#6 Posted by: Jinra Posted at: 2017-06-30T16:10:42.320Z Reads: 201

```
Find out what 60k eRPM translates to in speed on your setup. It should be faster than you're comfortable going on the board. I don't **believe** it'll fry your VESC as it's not supplying current to the motors when you're going downhill like that, but I definitely don't know for sure.
```

---
## \#7 Posted by: ShutterShock Posted at: 2017-06-30T16:38:22.709Z Reads: 197

```
Hm alright.  Sorry noob question but how would I find out how fast that is?  And would the 12s with the 4 5000 packs give me more range overall?
```

---
## \#8 Posted by: Jinra Posted at: 2017-06-30T16:41:33.936Z Reads: 195

```
Plug in your setup to find speed/erpm. Your range is dependent on your watt hours. Ah x voltage = watt hours. So the more the further you'll go.

http://calc.esk8.it/
```

---
## \#9 Posted by: ShutterShock Posted at: 2017-06-30T16:54:40.516Z Reads: 188

```
So basically you're saying that with the 4x 3s packs, since it is a total of 20000mah, or 20ah, 20*4.2*12 = total wh?

So for 12s, 20*44.4 = 888 wh?  

and for the 10s, 10*36 =720 ?

Any idea how many miles that translates to roughly?

The esk8 calc says my weighted speed with 12s is 30.98mph
```

---
## \#10 Posted by: Jinra Posted at: 2017-06-30T16:56:57.982Z Reads: 175

```
4x 3s packs in series = 12s 5000mah
4x 3 packs in parallel = 3s 20000mah

You don't get both by putting it in series. 12s x 5000 mah = 222wh. You can estimate 10wh per kilometer for about 22km range.
```

---
## \#11 Posted by: chaka Posted at: 2017-06-30T16:59:10.690Z Reads: 169

```
I run 12s on 200kv for my personal boards but they a geared to reach well over 40 mph so not a big chance that I will ever overrun the erpm by coasting. It is a different story for a board geared only to reach 25 to 30 mph, you need a little headroom to keep things happy.
```

---
## \#12 Posted by: ShutterShock Posted at: 2017-06-30T17:02:11.437Z Reads: 160

```
@chaka  Oh okay, what's your gearing ratio and wheel size?  I have 16-36 from the TB kit and 83mm wheels. 

You mean headroom for the VESC voltage wise?
```

---
## \#13 Posted by: ShutterShock Posted at: 2017-06-30T17:02:34.657Z Reads: 162

```
@Jinra  Ah okay that makes more sense.  Thanks!
```

---
## \#14 Posted by: Namasaki Posted at: 2017-06-30T17:08:50.178Z Reads: 157

```
You can exceed the Erpm limit on paper and not have a problem during normal operation because you won't spin the motor fast enough to top it out. 
Just remember, if you flip your board over on the bench and pull the trigger, it will top out right away
And you might fry it that way
```

---
## \#15 Posted by: ShutterShock Posted at: 2017-06-30T17:10:37.489Z Reads: 153

```
@Namasaki That seems logical, would the VESC stop increasing the speed at the 60,000 Erpm or would it just continue spinning until it blew itself up?
```

---
## \#16 Posted by: Namasaki Posted at: 2017-06-30T17:29:30.557Z Reads: 144

```
I think that depends on if you set the limit to 60k in bldc tool.
@chaka is more of an expert when it comes to Vescs 
Mayb he can give a more definitive answer.
```

---
## \#17 Posted by: ShutterShock Posted at: 2017-06-30T17:30:57.729Z Reads: 137

```
@Namasaki  And that limit is just a theoretical one or the limit of the bearings?
```

---
## \#18 Posted by: ShutterShock Posted at: 2017-06-30T17:36:20.798Z Reads: 135

```
@Namasaki  I just found chaka's post about choosing the right motor for the VESC, that explained it pretty well.  I don't want a dead VESC lol [Chaka's Post](http://www.electric-skateboard.builders/t/choosing-the-right-motor-kv-for-the-vesc/3125)
```

---
## \#19 Posted by: Namasaki Posted at: 2017-06-30T18:35:48.626Z Reads: 126

```
There is a setting in the bldc tool for max erpm.
```

---
## \#20 Posted by: sl33py Posted at: 2017-06-30T19:24:07.524Z Reads: 120

```
[quote="Jinra, post:4, topic:26441, full:true"]
That's because 190kv on 12s and 230kv on 10s  is fine. They do not go over erpm limits in real riding scenarios (unless you're going downhill obviously).
[/quote]


Good point.  Going downhill it's easy to exceed your typical speed = >60k ERPM and kapow dead DRV if unlucky.

Another *great* way to kill your DRV is on the bench - so don't full throttle and brake hard.  boom dead DRV, then you grab another VESC to re-test because we all like to confirm we're idiots and kill a second DRV...  :facepalm:
```

---
## \#21 Posted by: sl33py Posted at: 2017-06-30T19:27:12.009Z Reads: 116

```
[quote="ShutterShock, post:9, topic:26441"]
So for 12s, 20*44.4 = 888 wh?  

and for the 10s, 10*36 =720 ?

Any idea how many miles that translates to roughly?
[/quote]


The general consensus is (for street not mountainboard) is 10Wh=1km.  So 88km/54mi and 72km/44mi.  hard acceleration, hills, and weight of rider major impact.
```

---
## \#22 Posted by: Jinra Posted at: 2017-06-30T19:28:47.255Z Reads: 114

```
[quote="sl33py, post:20, topic:26441"]
Another great way to kill your DRV is on the bench - so don't full throttle and brake hard.  boom dead DRV, then you grab another VESC to re-test because we all like to confirm we're idiots and kill a second DRV...  :facepalm:
[/quote]

I think this is more of an issue on FOC. I went crazy full acceleration and braking on the bench to diagnose a separate issue and haven't had any issues on BLDC. I am using a rock solid Ollin VESC 4.12 though. I've only heard some stories on how full throttle FOC on bench has burned DRVs
```

---
## \#23 Posted by: sl33py Posted at: 2017-06-30T20:41:19.921Z Reads: 109

```
This was BLDC before @chaka let us know ERPM limit of 60k was the issue.  I was bench testing 200kv/190kv on 12s.  Just hammering hard accel/brake - not good.  Likely older hardware too like 4.8 iirc.

just cautionary - gentle on the bench is a good idea.
```

---
## \#24 Posted by: ShutterShock Posted at: 2017-07-01T06:58:43.720Z Reads: 103

```
@sl33py  Yeah that would be very unfortunate haha I

I'm gonna be using a torque boards VESC 4.12
```

---
