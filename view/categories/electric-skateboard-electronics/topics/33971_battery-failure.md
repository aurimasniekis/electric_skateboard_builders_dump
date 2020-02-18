# Battery Failure

### Replies: 18 Views: 803

## \#1 Posted by: mitchell898 Posted at: 2017-09-26T00:13:37.222Z Reads: 128

```
I built my first board about a month ago and was very pleased... but i've run into a battery issue. I'm using 2 zippy flightmax 3s batteries which I charge as one withought balance. I can now only get about 500m of useable battery life. Im not sure whether the batteries are just junk or if it's my fault. Moving forward, whats the best battery option? 18650 or similar lipos with balance charging?
```

---
## \#2 Posted by: willpark16 Posted at: 2017-09-26T00:56:59.588Z Reads: 128

```
Simple answer is 18650
```

---
## \#3 Posted by: topherbarnett Posted at: 2017-09-26T18:16:04.202Z Reads: 111

```
You should always balance your LiPo batteries or you risk blowing them up and lighting your house on fire. Do you have a multimeter to check the voltage on each cell and of each pack? If your batteries are wired in series, you could charge them as one 6S battery.

18650s would likely be less maintenance, but will be more expensive.

Either way, a BMS will help you keep your cells balanced, if you don't want to keep opening your enclosure to charge.
```

---
## \#4 Posted by: Acido Posted at: 2017-09-26T18:34:01.047Z Reads: 102

```
man a bms is like 25$ with shipping probably even less for that low cell count, you should have bought it
```

---
## \#5 Posted by: mitchell898 Posted at: 2017-09-26T19:25:07.194Z Reads: 97

```
I have an Imax B6 but since i have 2 3s batteries in series with 2 seperate balance ports I couldn't balance them simultaneously.
```

---
## \#6 Posted by: MysticalDork Posted at: 2017-09-26T19:38:26.553Z Reads: 84

```
Search online, you can get a 2x3s to 1x6s balancing adapter. Always balance your cells, either directly with a balance charger or with a BMS. Check your cell voltages, you may be extremely lucky and have a pack that can be saved. If not, you screwed up. Do better next time.
```

---
## \#7 Posted by: mitchell898 Posted at: 2017-09-26T19:52:32.974Z Reads: 78

```
Okay so decision time.... go through the hassle of building an 18650, or buy the same zippy batteries and balance them? I was pleased with the boards performance originally so im perfectly fine using the same battery setup just as long as it'll last a reasonable amount of time (Before the batteries are no longer useable). From what you guys are saying, it would be ideal to have an 18650 set up but If i balance the cheap lipos I should be fine, correct?
```

---
## \#8 Posted by: mitchell898 Posted at: 2017-09-26T20:09:44.883Z Reads: 70

```
Is there anyway I can do 2 4s batteries? In terms of charging and balancing.
```

---
## \#9 Posted by: MysticalDork Posted at: 2017-09-26T20:24:23.805Z Reads: 66

```
Your charger will handle up to 6s. That means you can charge two 3s packs in series, or charge each separately. You won't be able to charge two 4s packs in series.
```

---
## \#10 Posted by: mitchell898 Posted at: 2017-09-26T20:32:16.653Z Reads: 62

```
Yes, I mean besides my current charger.
```

---
## \#11 Posted by: mitchell898 Posted at: 2017-09-26T20:40:06.426Z Reads: 56

```
https://hobbyking.com/en_us/turnigy-accucel-8-150w-7a-balancer-charger.html?___store=en_us

I think the plan is this charger and 2 4s batteries.
```

---
## \#12 Posted by: MysticalDork Posted at: 2017-09-26T20:54:16.410Z Reads: 55

```
That will work. Just make sure your motor kv is low enough to not exceed 60k erpm with 8s.
```

---
## \#13 Posted by: florensvb Posted at: 2017-09-27T07:17:29.262Z Reads: 46

```
I have this charger

http://www.skyrc.com/image/cache/data/update/e8/720-720x480.jpg

together with 2 x this lipo

https://hobbyking.com/en_us/zippy-flightmax-8000mah-4s1p-30c.html?___store=en_us

and it works great
```

---
## \#14 Posted by: gogomrrobot Posted at: 2017-09-27T09:11:36.161Z Reads: 37

```
Ok i am pretty sure this is what battery failure looks like.....

<img src="/uploads/db1493/original/3X/9/3/93e07008c6b05d923df5c4eeb11c338f249ed712.JPG" width="666" height="500">

It happened after a hard hour of riding through trails, creeks on my Trampa (board is indestructible btw) but this one lipo Graphene 6000mAh 4s in series got this bulge and hot to the touch. Won't hold any charge- tried charging in balance mode, lipo mode, NiMH and NiCd mode... volts climb to about the 3.4v and fall back down now it just says error on the main connector. So sad $100 down the drain thought lipos would hold up better :(
```

---
## \#15 Posted by: scepterr Posted at: 2017-09-27T09:20:54.624Z Reads: 34

```
Pouch lipo are the least durable/long living. A single "bad" event can ruin a pouch lipo cell
```

---
## \#16 Posted by: hornet90 Posted at: 2017-09-27T09:44:52.195Z Reads: 31

```
Get yourself a bms from bestech it's the job all u do is plug a laptop style charger in

I might have a 8s one u can have at cost
```

---
## \#17 Posted by: gogomrrobot Posted at: 2017-09-27T09:49:45.783Z Reads: 32

```
Yeah I have to figure out what to do with this build. I got two Max6 and had those (2) 4s lipos now one is gone.  Maybe I should just build an 18650 pack -- 8s4p. I will get back to you on the BMS have to see how my enclosure fit's 18650.

BTW, How do you order from Best Tech? They have no shopping cart style checkout... is it all email and back and forth?
```

---
## \#18 Posted by: hornet90 Posted at: 2017-09-27T12:48:15.779Z Reads: 21

```
Its all email...on my 2 builds i used lipo im running 5 x 2s 5000mha in this build its super ill look and see if i still have that bms
```

---
