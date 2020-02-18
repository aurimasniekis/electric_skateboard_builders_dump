# Motor Recommendation Sealed or Unsealed?

### Replies: 24 Views: 1395

## \#1 Posted by: MyCampGround Posted at: 2018-04-12T13:52:43.890Z Reads: 266

```
i want to run a 12s4p samsung 30q, Ollin vesc + heatsink, ill be using a 37x10 inch board with caliber 2 50 degree trucks. i live in florida so i dont have any hills in my area, but i do have bridges. i am only going for a single motor setup as i don't think i would need two motors. what are your thoughts?
```

---
## \#2 Posted by: Acido Posted at: 2018-04-12T13:56:37.450Z Reads: 265

```
If its a single go 6374, Its 10$ more but its worth it.
Check the stator sizes on a thread somewhere here and see the difference
```

---
## \#3 Posted by: MyCampGround Posted at: 2018-04-12T14:02:08.569Z Reads: 255

```
i saw someone post about aps motors, would i want to or is it even possible to go bigger than 6374 motor?
```

---
## \#4 Posted by: Acido Posted at: 2018-04-12T14:04:00.880Z Reads: 247

```
there are plenty of motor sizes, why not assuming you can deliver the amps for the peak on the start
```

---
## \#5 Posted by: deucesdown Posted at: 2018-04-12T19:04:24.268Z Reads: 215

```
2 motors give you redundancy, especially important for brakes, if you should break a belt or something. This can be a huge deal.
```

---
## \#6 Posted by: Battosaii Posted at: 2018-04-12T19:12:06.631Z Reads: 204

```
I agree with him, also I'm a heavier guy and I noticed for me single motor consumes more power cause I'm always flooring it using more of my battery.

What part of Florida are you from @MyCampGround? I'm in Miami.
```

---
## \#7 Posted by: Jammm Posted at: 2018-04-12T19:12:51.999Z Reads: 198

```
Are you looking for a sensored motor ? If not i would go for the turingy 6374 192kv.
```

---
## \#8 Posted by: Bor.inc Posted at: 2018-04-12T19:13:35.256Z Reads: 199

```
I would try something like 170kv, I have heard that 12s and 190kv pushes the vesc to the limits but someone can eleborate on that
```

---
## \#9 Posted by: Jammm Posted at: 2018-04-12T19:24:59.344Z Reads: 193

```
My bad, i forgot he was going for 12s. In that case 170kv is the maximum you could go for. You're right.
```

---
## \#10 Posted by: MyCampGround Posted at: 2018-04-12T19:26:18.420Z Reads: 184

```
i am from Vero Beach , Strait east from tampa on the east coast.
```

---
## \#11 Posted by: MyCampGround Posted at: 2018-04-12T19:27:31.014Z Reads: 176

```
What is the difference in having a sensored motor?
```

---
## \#12 Posted by: Eboosted Posted at: 2018-04-12T19:30:57.359Z Reads: 173

```
Go dual, the push you will feel is balanced, the brakes are better, the look is harmonic and it'll be safer, if you ever had a vesc reboot going down a hill, you will still have brakes on the other vesc
```

---
## \#13 Posted by: E1Allen Posted at: 2018-04-12T19:32:17.703Z Reads: 171

```
190kv on 12s is within erpm limits
```

---
## \#14 Posted by: bartroosen12 Posted at: 2018-04-12T19:33:00.620Z Reads: 167

```
If you got only bridges single drive is enough, dual drive will have more friction and to much power you probably don't need.
```

---
## \#15 Posted by: MyCampGround Posted at: 2018-04-12T19:33:41.023Z Reads: 166

```
that cost of going dual is a lot more, and right now budget is tight.
```

---
## \#16 Posted by: Eboosted Posted at: 2018-04-12T19:48:48.424Z Reads: 162

```
If you have money yo but such quality parts then save a little bit more, you will thank me latter.

Money is just the mean to get what you want, if the esk8 is well made, you will forget how much you spent and soon you will realize it didn't matter, on the other hand any esk8 will bring much more happiness to your life than any amount of money, trust story!
```

---
## \#17 Posted by: MyCampGround Posted at: 2018-04-12T19:50:49.506Z Reads: 159

```
yes what i mean is i can start with single drive and in the future if i need or want could move to dual drive easily when more money comes available to be thrown at the board. i just need a good motor recommendation.
```

---
## \#18 Posted by: Jammm Posted at: 2018-04-15T12:02:12.017Z Reads: 141

```
A sensored motor will have better torque at start. It will get rid of the stuttering you can experience when starting.

For you I would sugget either this motor, unsensored : 

https://hobbyking.com/fr_fr/turnigy-aerodrive-sk3-6374-168kv-brushless-outrunner-motor.html

Or this one, sensored : 

http://alienpowersystem.com/shop/brushless-motors/aps-6374s-sensored-outrunner-brushless-motor-170kv-3200w/
```

---
## \#19 Posted by: MyCampGround Posted at: 2018-04-15T12:14:08.515Z Reads: 134

```
i was looking at these two motors, one is sealed the other is not. [( sealed )](https://buildkitboards.com/collections/motors/products/6374-190kv-motor) [( not sealed )](collections/electric-skateboard-motors/products/electric-skateboard-motor-6374-190kv) is there any other difference to these motors other than that? also what are the pros/cons to sealed/ not sealed?
```

---
## \#20 Posted by: Jammm Posted at: 2018-04-15T12:28:54.796Z Reads: 134

```
Have you heard if the erpm limit ?

Vesc's are limited to 60 000 erpm. If you go over it, you'll fry it.

Here's how to calculate it : 

Erpm = number of pair of poles * kv * max voltage of your battery

In your case, it equals to

Erpm = 7 * 190 * 50,4 = 67 032

If you choose à 190kv motor, you'll ruin your vesc. You have to use 170kv max with 12s which is just under the erpm limite (59 976)


I don't know much about the sealed or not sealed difference though
```

---
## \#21 Posted by: MyCampGround Posted at: 2018-04-15T12:58:29.183Z Reads: 127

```
cant you just limit the erpm in vesc settings?
```

---
## \#22 Posted by: Hummie Posted at: 2018-04-15T15:13:56.193Z Reads: 126

```
Yes n use any kv.
```

---
## \#23 Posted by: MyCampGround Posted at: 2018-04-16T00:02:39.995Z Reads: 116

```
Should i go with a sealed motor or a non sealed motor? was looking at BKB's or DIY's
```

---
## \#24 Posted by: DanLazer Posted at: 2019-04-07T19:24:49.318Z Reads: 45

```
The description that the BKB motor is sealed is incorrect.  There are no seals on that motor.  You can see right through the rotor to the stator coils in the pics.

I recently purchased some 6354's from BKB and was disappointed by the lack of the advertised seals.
```

---
