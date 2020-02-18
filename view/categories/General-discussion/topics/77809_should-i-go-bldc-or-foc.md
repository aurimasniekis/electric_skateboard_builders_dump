# Should i go bldc or foc?

### Replies: 11 Views: 537

## \#1 Posted by: Bjork3n Posted at: 2018-12-12T16:48:54.691Z Reads: 182

```
Hey Guys!
So im at the end of my 2nd build and im a bit torn between going bldc or foc.
On my previous build i ran bldc with ackmaniac 3.100 FW, was great and had no issue for over 1000km.
Now on my new build im a bit tempted to try FOC.. (I have those updated focboxes v1.7)
Im going to use dual 6374 190kv with 97mm wheels and 16/36 gearing 10s battery. 

My questions is the torque better in Foc compared to bldc?
Standing starts is from what i understand a lot better in foc? (im after that bananas acceleration)
What is the best FW to use to this date? Is it still the ackmaniac that is the best out there or should i stick to the 2.18fw when going FOC? 

Im going to use sensors so its either foc sensored or bldc hybrid.

Thanks in advance guys! 
// Simon (Sweden)
```

---
## \#2 Posted by: linsus Posted at: 2018-12-12T16:53:48.253Z Reads: 176

```
Never used focboxes or acks stuff. Sound is the big difference. Prob wont notice that much on the torque part. FOC is a little more efficient as well as less noisy, thats it
```

---
## \#3 Posted by: mmaner Posted at: 2018-12-12T17:09:56.660Z Reads: 167

```
FocBox's are great for FOC, the question is FOC great.

The quite is one positive aspect, and the startup from stand still can be another.  I would argue that the quiet is noce, but the sound is more useful for letting others know your there.  And its just such a waste to start up from stand still, if you do it a lot.  It takes so much power to get the board moving, not a lot to keep it moving.  

I would suggest trying FOC out, see if you like it, so it doesn't seem all mysterious and junk :slight_smile:.  But if your not just incredibly impressed or find it really useful, go to hybrid mode or back to FOC.
```

---
## \#4 Posted by: Bjork3n Posted at: 2018-12-12T17:19:26.475Z Reads: 159

```
Thanks for your reply!
Well it seems like a lot of them trying foc thinks its super nice, but ive also heard a lot of issues regarding the focmode..
Foc is making the diy board feel more polished if i understood correctly. 
Bldc is great but it can be a bit twitchy and maybe feel a bit old 2018/19?

The sound in bldc is quite useful, people tends to move out of my way when they hear the bldc sound :joy:
The speed is also a bit slower running foc  but it seems like the torque and smoothness makes up for this.

Is there anyone out there who tried foc (with no issues) and decided NOPE im going back to bldc?

These decisons....
```

---
## \#5 Posted by: briman05 Posted at: 2018-12-12T17:21:34.925Z Reads: 151

```
I have the FOC on my board with dual focbox's and it is great.  I don't think I will even go to BLDC.  Foc gets such a bad rap because it is so taxing on the mosfets but if you do conservative settings and not balls to the wall on everything FOC shouldnt be a issue.  If you have motor sensor and they dont get picked up in BLDC try FOC to see if they will register the sensors.  I had that issue with mine.
```

---
## \#6 Posted by: Bjork3n Posted at: 2018-12-12T17:26:19.262Z Reads: 145

```
So what is considerd balls to the walls settings :joy:

Im thinking of using 
Motor max: 60-70A
Battery max : 35-40A

10s4p with 30q and dual 6374. 
I think it will be quite torqy with those settings
```

---
## \#7 Posted by: briman05 Posted at: 2018-12-12T17:28:04.723Z Reads: 145

```
You should be fine with that as the Focbox was made to handle FOC mode with its upgraded components.  I was talking more about cheaper vesc that have been notoriously killed by FOC
```

---
## \#8 Posted by: Bjork3n Posted at: 2018-12-12T17:30:29.339Z Reads: 141

```
Well i also heard about bricked focboxes with FOC so im still a bit concernd. 
I have the updated boxes v1.7 that is supposed to have some better HW dont really know whats been updated more than the canbus connections.
```

---
## \#9 Posted by: thisguyhere Posted at: 2018-12-12T17:44:54.708Z Reads: 130

```
https://www.electric-skateboard.builders/t/me-this-weekend-and-discussions-about-other-things/48874?u=thisguyhere
```

---
## \#10 Posted by: Bjork3n Posted at: 2018-12-25T20:09:23.153Z Reads: 86

```
How much speed are you losing running Foc? I know it's slower but by how much? 
You guys think it's possible reaching 45-47km/h with dual 6374 190kv , 16/36 and 97mm wheels? 
Most esk8 calc is for bldc if I'm not mistaken? 

Can't wait to test Foc when spring arrives...I'm almost convinced.😂
```

---
## \#11 Posted by: Bjork3n Posted at: 2019-01-04T15:14:13.914Z Reads: 51

```
Tried foc today. 
Its Focking amazing.

Damn its smooth and predictable, and torque seems smoother and quite powerfull aswell.
Tried to detect motors in bldc but i was not able to on one of the focboxes so i decided to go FOC.

Topspeed is 40km/h with my setup. Was expecting a bit more but you cant have it all :)   (esk8 calc said 50km/H)
https://metr.at/r/vVeOc?fbclid=IwAR33AyxzZy_0j9BMAOYrAyFEkGqb4EffGPzzKJltLpb_Lr2Fx4wDFYk8Q2k
```

---
