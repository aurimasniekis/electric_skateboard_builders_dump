# Am I Too Fat for E-boarding?

### Replies: 19 Views: 3073

## \#1 Posted by: stuxtruth Posted at: 2016-09-04T22:12:39.390Z Reads: 277

```
So I'm running a 6S4P Setup with two 260kV SK3 motors.

I'm running 2 6S FVT ESCs. I've already blown one. I ordered a replacement and it overheated today. The board has PLENTY OF TORQUE AND SPEED and I had a custom battery made so I'm sticking to 6S. 

My question is for a guy of my size (230lb) would VESC or TB 12S ESC suit me better? Is the only advantage VESC has over FVT the "start from a stop" capability? Also. I don't want loud brakes.

My SINGLE MOTOR TACON 160 AND EZRUN ESC PULLED ME UP HILL NO PROBLEMS. And my motor was cool afterwards. I thought switching to dual motor would give me no issues.

<img src="/uploads/db1493/original/2X/5/5a7176fa9f20cb79740bb733ccd4622d96fb851b.JPG" width="666" height="500">
```

---
## \#2 Posted by: sl33py Posted at: 2016-09-04T22:38:41.446Z Reads: 263

```
Not what you want to hear, but i think you need more voltage...  and possibly lower kv motors.

I'm a bigger guy than you, and ride single motors right now (while building a couple new dual setups).  No issues.  And by bigger i'm 265lbs in my boxers, so probably closer to 50lbs heavier.

I don't know TB's ESC as i've been using VESC as my default for the last year or so.  My GF's single motor setup moves me along fine (admittedly on the flats) - VESC 200kv 8s 83mm xx/36t.  Haven't tried hills on it, but cruising on the flats it works great.

My Marbel board is single motor and too me up hills surprisingly well last weekend on an esk8 meetup.  Don't know grade, but steeper than i expected.

Of the two i think the 12s opto that TB sells may give you more power - because the VESC will limit to around 50a vs the 120a of TB's.  Maybe someone who has ridden both can comment.  But i don't think the brakes will be as quiet as VESC, let alone FOC mode if silent is your goal.

GL!
```

---
## \#3 Posted by: Jeff Posted at: 2016-09-04T22:48:05.987Z Reads: 231

```
I am basically the same weight as you.I have a vanguard build with identical dual motors so it can be done :slight_smile:  Prior to getting VESCs, I blew out two ESCs. 

Now that I have VESCs and can set current limits I never have had any issues.

I run 10S and my gearing is set for ~33mph. The board is scary fast......
```

---
## \#4 Posted by: stuxtruth Posted at: 2016-09-04T22:50:19.662Z Reads: 219

```
I'm having a mental battle. Deciding to either just buy two VESC or to sell everything and do a single 6374 with VESC. What do you guys think?
```

---
## \#5 Posted by: Jeff Posted at: 2016-09-04T22:58:34.419Z Reads: 203

```
What is your current gear ratio? At 6S and 260 kv you can't gear it too steep or you will draw too much current.

If you can re-gear and get two VESCs it might be an easy enough change than starting all over.
```

---
## \#6 Posted by: stuxtruth Posted at: 2016-09-04T22:59:51.357Z Reads: 191

```
15/36 is my gearing.
```

---
## \#7 Posted by: sl33py Posted at: 2016-09-04T23:00:10.729Z Reads: 185

```
setup and geared correctly, the dual motors will do hills better.  But simplicity of a single setup is nice too!  You can always do single 6374 and add another dual diagonal later if needed.

I think lower kv motors on higher voltage might be the best solution...
```

---
## \#8 Posted by: TarzanHBK Posted at: 2016-09-04T23:17:46.708Z Reads: 173

```
dont just switch your escs for vescs at 6s, you´ll probably overheat them fast.
get a big single, like an 6374 under 200kv and go with a 10s and one vesc.
simple and powerfull. like the others said, if needed, add an second one and you´ll be able to go straight up a wall ;)
```

---
## \#9 Posted by: torqueboards Posted at: 2016-09-04T23:35:07.599Z Reads: 164

```
Just up the voltage. 6S is pretty lean. I honestly think the default should be 10S for each and every build. Perhaps even 8S would do just fine but the extra cost for 10S would equal more power and be a much more reliable build.

Technically, you shouldn't have any issues with that setup.

What made the setup overheat and pop?
```

---
## \#10 Posted by: stuxtruth Posted at: 2016-09-04T23:52:54.508Z Reads: 154

```
Me riding it. Braking down a hill again.
```

---
## \#11 Posted by: Photorph Posted at: 2016-09-05T02:30:53.292Z Reads: 128

```
Should we be recommending this set up if he really wants to feel the same torque and acceleration as someone who is 130 lbs would.  

12s, dual diagonal 149 kv 6374 motors, VESC, 83 mm wheels, If you want more speed you can probably change the wheels to 90mm.  Hill won't be a problem.
```

---
## \#12 Posted by: torqueboards Posted at: 2016-09-05T02:52:33.351Z Reads: 123

```
@Photorph - Yeah, I'd have to agree too.

The default standard for any build should be 10S. I was planning on offering a 6S, 8S, 10S packs but the difference in price is the difference in reliability. In the end, everyone will go for the cheaper option but that's not the entire idea/point.

Going cheaper will always in the end - end up costing more, most of the time.

While a 6S setup can work very well the added difference isn't a whole lot.. Reliability is worth the cost.
```

---
## \#13 Posted by: stuxtruth Posted at: 2016-09-05T14:56:10.401Z Reads: 104

```
So if I'm going to change to a 12S setup, I'm running 36/15t. Should I go for 149KV 6374 if I want to do a single?
```

---
## \#14 Posted by: ecuadorche Posted at: 2016-09-05T17:16:06.378Z Reads: 94

```
im at around 250 pounds and im currently using a 10s setup with vesc and 200kv motor with 36t to 16t pulley on single motor, it pulls me along fine on flats only it cannot go up a hill with me on it at all but im going with a 36t 14t dual drive setup soon
```

---
## \#15 Posted by: Photorph Posted at: 2016-09-05T17:38:44.239Z Reads: 91

```
Dual!  Anyone over 180 lbs should just use dual by default in my opinion.  I'm 140 and I still always use dual.  If you want to climb hills then you need the bigger 6374 in a dual diagonal set up.  The 149 kV will have more torque.  Get those and the widest belts you can get for more torque transfer.  I'm just recommending a set up that can easily carry you uphill and accelerate you like you aren't even there.  What max speed do you want? If you're okay with around 20-24 mph then that set up should work, decent top speed and tons of torque.
```

---
## \#16 Posted by: stuxtruth Posted at: 2016-09-05T18:17:01.277Z Reads: 92

```
Ok what about keeping my current setup and doing a 10s battery with VESCs and using @torqueboards 12T motor pulley?

<img src="/uploads/db1493/original/2X/8/80a8526fdc9c15edd21b40f2883cd0663db49148.jpg" width="306" height="449">
```

---
## \#17 Posted by: Photorph Posted at: 2016-09-05T20:38:56.581Z Reads: 85

```
Your ERPM is still too high and you have a higher chance of burning up DRV chips.  260 KV motors are just not ideal with the VESC unless you go really low voltage.  Asides from that, you want motors with more torque for your weight...for you the lower the kv value the better.  

There was a thread somewhere where chaka explained that that max motor KV should be 8600/battery voltage.  So for example, for a 12s battery (~43.4 volts), your max motor KV should be 8600/43.4 which is about 190 kv.  Same with 10s, but it comes out to be about 240kv.
```

---
## \#18 Posted by: stuxtruth Posted at: 2016-09-05T20:46:06.974Z Reads: 85

```
I honestly think the 12s opto esc may be the best bet for me
```

---
## \#19 Posted by: sl33py Posted at: 2016-09-06T19:54:29.379Z Reads: 65

```
**be cautious of 12t motor pulleys on 9mm belt.**  I did this and could not avoid skipping under hard braking and eventually (wear) hard acceleration too.  Not enough teeth in mesh and more surface area needed on a single motor (12mm or 15mm wide belt/pulleys).

as a result i don't use less than 13/14t on the motor gear just to be safe.  9/12/or 15mm.

GL!
```

---
