# Single hubs in diagonal drive?

### Replies: 12 Views: 887

## \#1 Posted by: Bazingazunga Posted at: 2017-09-13T13:43:55.582Z Reads: 138

```
Hello,

Some of you may have seen my post regarding acquiring cheap Mini Fiik's in the UK. These are Single 75kv hub boards, presumably with some weak ass battery and a basic chinese ESC. 

https://www.fiik.com/mini-fiik

I have absolutely zero experience with hubs, so I'm trying to decipher how they work. 
Now I had the idea last night to get two, and just for the giggles rig it into a dual hub board. Im assuming the hub is connected to the truck in some way shape or form, and as such i'd have to put them in a diagonal drive? 

I'd obviously need to replace the ESC's with two vesc's too, and have them using one receiver. 
Is this even remotely possible? What would the maximum(ish) amps these hubs would be able to handle? I'm really struggling to find any specifications about these boards whatsoever, so I'm not too sure on them.

Any insight on the mechanics of this would be great, as im tempted to even just replace the battery and/or esc to speed things up a bit.

A bit of a shits and giggles project, hopefully! :grin:
```

---
## \#2 Posted by: JdogAwesome Posted at: 2017-09-13T14:05:36.645Z Reads: 122

```
I dont see any reason why diagonal hubs wouldn't work, never seen it before though people do diagonal geared builds so I think it would work fine. Not sure what size wheels those are so I cant say much but with my 90mm Maytech Hubs I have max amps at 50 and they usually steady out to about 15A and only spike that high when accelerating.
```

---
## \#3 Posted by: Bazingazunga Posted at: 2017-09-13T14:23:29.553Z Reads: 112

```
You got a link to where you got the maytechs from? Also what sorta speed to you get to/what kv are they? 
Nice one :)
```

---
## \#4 Posted by: Idle Posted at: 2017-09-13T14:30:08.230Z Reads: 105

```
Why not do two meepos to make a all-wheel-driv!
```

---
## \#5 Posted by: BigBoyToys Posted at: 2017-09-13T14:35:15.216Z Reads: 99

```
I built a dual diagnal Carvon V2 hub board. Worst handling board Ive ever made. The board got dissassembled within a week and converted to a dual rear. The only way I can imagine this would be ok is if the board is very underpowered. Otherwise the torquesteer/truck walk is unbearable and puts you into a speed wobble when going from acceleration to braking
```

---
## \#6 Posted by: Bazingazunga Posted at: 2017-09-13T14:47:53.608Z Reads: 94

```
Ah okay, interesting. Pardon my ignorance, but am i able to simply have two single hubs, pop one off and pop it onto the one truck to make it a dual drive? Didn't think that would be possible
```

---
## \#7 Posted by: JdogAwesome Posted at: 2017-09-13T15:16:31.334Z Reads: 85

```
Check out my review of them [HERE](https://www.electric-skateboard.builders/t/maytech-hub-motor-vesc-and-truck-review/31413) and to purchase them, I emailed them though you can get them on AliExpress as well. $90 a hub and you need a special type of truck to fit them as well which is $25 as well. So far there great hubs though problem is that at 6S I'm only getting upto 20mph max which sucks compared to the 32mph on my single Carvon V2. Though I think 10 or 12S you'd definitely get more speed.

I'm not sure about the changing the hubs out for different truck but you may be able to. Try taking them apart and see how far you can get.
```

---
## \#8 Posted by: themegak Posted at: 2017-09-13T16:18:17.332Z Reads: 75

```
If you don't mind me asking, how much do you weigh ?
```

---
## \#9 Posted by: NickTheDude Posted at: 2017-09-13T16:38:57.432Z Reads: 64

```
Check out this site. It seems like they sell many of the commonly used Chinese parts as kits or individually. Incredibly cheap too, they say they're selling directly from the factory. http://www.diyeboard.com/diy-electric-skateboard-kits-c-533.html
```

---
## \#10 Posted by: JdogAwesome Posted at: 2017-09-13T17:10:24.350Z Reads: 58

```
I weigh about 130lbs and the dual Maytechs in sensorsed get me going really fast.
```

---
## \#11 Posted by: composites_r_awesome Posted at: 2018-08-25T17:46:23.526Z Reads: 23

```
Is that for both hubs? I'm wondering if the cooling of stators wouldn't be a problem, could I set the VESC amp rating to higher than 22A per hub? 65kv 90mm ones at 10s with FOC
```

---
## \#12 Posted by: JdogAwesome Posted at: 2018-08-27T13:41:04.222Z Reads: 18

```
I believe the Ackmaniac firmware does total your current draw for each VESC when you tell it you have two VESC's, which I did, so I believe yes that is total current draw. While my motors did get warm they stayed under 60c from what I remember which is totally acceptable, so I don't think throttling to 22A max is necessary or wanted because it will diminishe your acceleration.
```

---
