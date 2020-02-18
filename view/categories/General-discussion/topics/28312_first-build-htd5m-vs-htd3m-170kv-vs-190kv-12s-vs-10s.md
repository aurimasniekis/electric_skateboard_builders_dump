# FIRST BUILD - HTD5M vs HTD3M &amp; 170Kv vs 190Kv &amp; 12s vs 10s

### Replies: 10 Views: 1071

## \#1 Posted by: Ket Posted at: 2017-07-22T21:51:59.046Z Reads: 175

```
Hi guys, 

So i have lurking around here for some time and i have decided its time to make my first build. I have been gathering a list of different parts e.c.t and i need to chose between the following parts. 

For the drive train i'm stuck between HTD3M 15mm wide 48t/22t and HTD5M 10mm wide 36t/16t. which one is better in terms of belt slippage and durability. I'm going to use 90mm flywheels clones was thinking of 97mm but they're a bit too big for me.

For the motor i'm going with 6374 brushless with hall sensor but not sure whether to chose 170Kv or 190Kv?

In terms of batteries i keep on going backwards and forwards between 18650s and Lipos. But i have decided to go with either 2x 5s 6000mah or 2x 6s 6000mah Lipos as they're simpler than 18650s especially because this is going to be my first build and are cheaper. Another question is that i know the VESC is rated up to 12s but i have heard that its safer to use lower than 12s batteries. 

I'm aiming for a top speed of 30mph and 10 miles of range but not too bothered about it.  

Would appreciate it a lot if you guys can help me out. 

Cheers 
Ket
```

---
## \#2 Posted by: wafflejock Posted at: 2017-07-22T22:51:01.124Z Reads: 162

```
Not to be terse but can use this to check out your build http://calc.esk8.it if you aren't already a downhill skater I'd reconsider on what you need for top speed especially if you need to do hill climbing since in the gearing you are trading torque for speed.  30mph is a lot faster than it sounds when you're standing on a wobbly stick ;). Major issues I believe with 12S with the VESC DRV chip I believe only happen above 230kv but can also artificially limit the erpm through configuration.
```

---
## \#3 Posted by: melchiorvester Posted at: 2017-07-22T23:36:13.380Z Reads: 157

```
Links to the belts you might be using? I'm interested in using HTD5M belts and pulleys
```

---
## \#4 Posted by: chuttney1 Posted at: 2017-07-23T03:59:50.126Z Reads: 144

```
Just only focusing on the belt. Not using a speed calculator because it lacks max values of power transmittance. You have to consult the belt specs from the manufacturer. I can tell you 3M belts are more prone to being destroyed by the motor if gearing ratio is chosen incorrectly. I have used a 48/18 tooth setup and the belts were destroyed and my wheels slipped.
```

---
## \#5 Posted by: Boardnamics Posted at: 2017-07-23T06:13:59.329Z Reads: 129

```
Not only are the teeth smaller on HTD3M, they're also significantly thinner. I have both and I would vouch for htd5m more. They're just generally more durable. The advantage HTD3M has is that they're quieter, smoother, and allow for a finer precision of gear ratios. 30mph is definitely fast. Most people never go that fast but if that is what you want, a higher kv motor might be a better choice. If you speed calc it, aim for somewhere top speed of about 35mph. You will never have enough torque to reach exactly 30mph in most situations.
```

---
## \#6 Posted by: Ket Posted at: 2017-07-23T14:50:05.051Z Reads: 119

```
Yeah I've used this calculator thats how i found the gearing ratio for 30mph. There no steep hills where i live i'd say a max of 10% incline at the most. but you do bring an interesting point that 30mph  is actually faster than it sound. i was thinking of first doing 16t/48t which should give me 22 mph and see how i like than and upgrade to 22t if i need the speed. In terms of batteries so i can use 12s as long as i limit the erpm in the configuration? and also what Kv should i go for or that just depends on the top speed i want/torque ? also whats your opinion on HTD5M vs HTD3M?
```

---
## \#7 Posted by: Ket Posted at: 2017-07-23T14:54:38.975Z Reads: 116

```
I've found this on ebay. The only problem i see that its 10mm wide which i think doesn't provide enough traction for single drive motor but i hope someone proves me wrong. 

http://www.ebay.co.uk/itm/Pulleys-And-Motor-Mount-DIY-Parts-For-83-90-97MM-Wheels-Electric-Skateboard-Kit/152505100375?_trksid=p2481888.c100675.m4236&_trkparms=aid%3D111001%26algo%3DREC.SEED%26ao%3D1%26asc%3D20160908105057%26meid%3D870e7ecc5cb4432193252f051c08eed5%26pid%3D100675%26rk%3D4%26rkt%3D15%26sd%3D161964844497&_trkparms=pageci%253A73a93781-6fb6-11e7-b9b9-74dbd18073c7%257Cparentrq%253A6feedc2d15d0a99be423c83cfff78991%257Ciid%253A1
```

---
## \#8 Posted by: Ket Posted at: 2017-07-23T15:02:40.665Z Reads: 112

```
wait what? shouldn't a lower Kv motor gives a higher torque? and higher Kv motor gives higher speeds with lower torque?
```

---
## \#9 Posted by: Boardnamics Posted at: 2017-07-23T18:32:15.131Z Reads: 97

```
Yes, I said a higher kv may be a better choice if ur overall goal is top speed and not hill climbing ability
```

---
## \#10 Posted by: dg798 Posted at: 2017-07-23T19:53:35.229Z Reads: 92

```
i have this motor diy-electric-skateboard-kits-parts/electric-skateboard-motor-6355-190kv/1 and im buying this esc http://www.ebay.com/itm/302332747417?var=6011693195112. can i use everything with these batteries https://hobbyking.com/en_us/turnigy-5000mah-5s-20c-lipo-pack.html1.
```

---
