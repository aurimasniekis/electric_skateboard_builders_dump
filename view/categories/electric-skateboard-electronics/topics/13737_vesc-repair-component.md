# Vesc repair component

### Replies: 54 Views: 3315

## \#1 Posted by: ralphy Posted at: 2016-11-27T03:01:27.072Z Reads: 205

```
Does anyone know what this little square electronic device that fried on my vsec is called? 

Im not sure what happened and id like to repair it so i dont have to get a new one. <img src="/uploads/db1493/original/3X/c/c/ccd900609fffb056c0dcd2b29797dc1de43c1376.jpg" width="375" height="500">
```

---
## \#2 Posted by: JohnnyMeduse Posted at: 2016-11-27T03:04:02.248Z Reads: 193

```
It's a capacitor
```

---
## \#3 Posted by: Blasto Posted at: 2016-11-27T03:07:12.656Z Reads: 191

```
It's 10uf 1206 50v cap... but that's not the point here, your vesc's are missing the 15uf caps also.... and bulk caps...
```

---
## \#4 Posted by: wmj259 Posted at: 2016-11-27T03:07:35.281Z Reads: 190

```
The 3 square pieces at the upper half of the board? or the 2 cylindrical pieces attached with the red and black wires (These are the capacitors).

Edit: OOOOOOO now I see that orange arrow :slight_smile:
```

---
## \#5 Posted by: JohnnyMeduse Posted at: 2016-11-27T03:09:45.041Z Reads: 184

```
Capacitor are all shape and form... for more info you can look on vedder web site vedder.se or use VESC Faq as search keyword
```

---
## \#6 Posted by: ralphy Posted at: 2016-11-27T03:21:37.253Z Reads: 186

```
The big capacitors are the bulk caps? They have fallen out with vibration. 

The one that got fried is that little sqaure one with the arrow. Is this a common failure?<img src="/uploads/db1493/original/3X/7/f/7f1c767510ccd96292c2752c285dabcdd180081f.jpg" width="375" height="500">

See it better now
```

---
## \#7 Posted by: Blasto Posted at: 2016-11-27T03:26:49.256Z Reads: 179

```
(Sorry for the crappy edit picture)

Your vendor never populated the 15uf caps. I woudn't be surprised if you drv is roast also from over voltage.

<img src="/uploads/db1493/original/3X/4/3/431c4e380bfb8c3e1766983d02a3c973cae4bbe9.PNG" width="374" height="500">
```

---
## \#8 Posted by: Namasaki Posted at: 2016-11-27T03:34:11.340Z Reads: 173

```
Just curious, where did you buy these Vesc's?
```

---
## \#9 Posted by: zmoney Posted at: 2016-11-27T03:35:15.605Z Reads: 169

```
http://www.electric-skateboard.builders/t/chakas-vesc-repair-log/1151/28?u=zmoney

Didn't realize that there was a separate thread for this. My bad.
```

---
## \#10 Posted by: Blasto Posted at: 2016-11-27T03:37:07.544Z Reads: 168

```
Holy crap man.... guess this reel didn't make it to the pcik and place

<img src="/uploads/db1493/original/3X/0/0/003f8314f56ec281cb9e94e2422dad5eecd07b00.PNG" width="374" height="500">
```

---
## \#11 Posted by: zmoney Posted at: 2016-11-27T03:38:49.130Z Reads: 158

```
I was about to say! Who was your vendor?
```

---
## \#12 Posted by: ralphy Posted at: 2016-11-27T03:42:36.619Z Reads: 160

```
I got these with some brushless motors from Alibaba. 

So i got slightly screwed ? 

Is everything circled missing? One still works great
```

---
## \#13 Posted by: zmoney Posted at: 2016-11-27T03:44:39.625Z Reads: 161

```
Yeah man. Everything he circled is missing and should be there. Your other VESC might work for now, but brake too hard or accelerate too fast and you might find yourself in some trouble.
```

---
## \#14 Posted by: Blasto Posted at: 2016-11-27T03:45:05.346Z Reads: 159

```
[quote="ralphy, post:12, topic:13737"]
Is everything circled missing? One still works great
[/quote]

Yes missing, don't want to be pessismistic, it's a question time before something blows. Your missing so many caps and we didnt even see the other side of the pcb
```

---
## \#15 Posted by: ralphy Posted at: 2016-11-27T03:47:50.858Z Reads: 159

```
<img src="/uploads/db1493/original/3X/3/f/3fb0bc513cab750d09e7675d45e3e35904264f51.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/2/5/254a3501590f7b5f65ad130871b47bd66f0604f7.jpg" width="375" height="500">
```

---
## \#16 Posted by: ralphy Posted at: 2016-11-27T04:36:24.292Z Reads: 152

```
Found another issue the positive leads insulation gets cut with the little studs poking through. Short circuit for sure.<img src="/uploads/db1493/original/3X/1/2/12c6a9995f205dd279780c171a62ab689d3d846d.jpg" width="375" height="500">
```

---
## \#17 Posted by: wmj259 Posted at: 2016-11-27T05:06:32.252Z Reads: 145

```
Where did you get your vescs so you can warn others not to get it from.
```

---
## \#18 Posted by: Namasaki Posted at: 2016-11-27T12:39:13.694Z Reads: 136

```
He said he got them from Alibaba. 
This just proves that Vendors matter.
```

---
## \#19 Posted by: ralphy Posted at: 2016-11-27T14:07:30.358Z Reads: 136

```
Guys so how do I go about getting this resolved . Should I add in the missing components on the functional one? 

Who can provide a quality vesc or repair job to get me up and running again?
```

---
## \#20 Posted by: wmj259 Posted at: 2016-11-27T16:55:27.374Z Reads: 130

```
@chaka, I believe
```

---
## \#21 Posted by: Blasto Posted at: 2016-11-27T16:57:59.401Z Reads: 122

```
Pretty sure chaka won't touch this with a 10 foot pole. Seeing the power cable scewered, you got battery voltage on the 3.3v rail... most of the ic's are probably blown
```

---
## \#22 Posted by: Maxid Posted at: 2016-11-27T17:32:04.640Z Reads: 119

```
[quote="ralphy, post:19, topic:13737, full:true"]
Guys so how do I go about getting this resolved . 
[/quote]

Not at all. Throw away and buy new quality ones.
```

---
## \#23 Posted by: zmoney Posted at: 2016-11-27T20:23:26.530Z Reads: 114

```
Yeah... Repairing it can be costly and almost impossible.
```

---
## \#24 Posted by: ralphy Posted at: 2016-11-27T22:19:46.143Z Reads: 110

```
What exactly differs in a quality one? I paid $150 total for both of these and buyer protection goes for 6 months so i could get my hands on replacments. I can easily keep the battery lead silicone from getting damaged if thats the issue.
```

---
## \#25 Posted by: Maxid Posted at: 2016-11-27T22:30:45.881Z Reads: 106

```
You have missing components on a part that is actually crucial for your survival and think that just getting a replacement from the same vendor is a good idea? I would get the replacements if they are free and fully inspect them before riding. However I'd always feel uneasy knowing that something could happen while riding.
```

---
## \#26 Posted by: ralphy Posted at: 2016-11-27T22:35:50.673Z Reads: 107

```
I see, i just wonder if for some reason it is actually designed purposly with those components missing. I  found a thread that talks about the ones i bought but it doesnt seem anyone has tried them. 

http://www.electric-skateboard.builders/t/new-vesc-from-china-seems-like-not-only-maytech-is-making-vescs-now/5207/55
```

---
## \#27 Posted by: Maxid Posted at: 2016-11-27T22:38:31.132Z Reads: 104

```
You bought from Vanda? I thought their VESC looked quite good on the pictures they showed. But in the end it might all habe been just marketing. You should contact @Karen_Vanda and ask what is going on. Let us know so we can all benefit from the experience.
```

---
## \#28 Posted by: ralphy Posted at: 2016-11-27T23:04:44.952Z Reads: 106

```
These are not from her these are from FREERCHOBBY.

I dont think she is associated with them. Hers are also purple these are green
```

---
## \#29 Posted by: wmj259 Posted at: 2016-11-27T23:04:46.619Z Reads: 110

```
I know alibaba has a 30/60 day money back guarentee also with very good buyer protection. Make a dispute about this. Don't let $150 slide away.
```

---
## \#30 Posted by: Maxid Posted at: 2016-11-27T23:06:14.587Z Reads: 111

```
The post you linked was about the Vanda VESCs.
```

---
## \#31 Posted by: ralphy Posted at: 2016-11-27T23:10:04.454Z Reads: 111

```
Its been more than 60 days, ive had good luck with motors from them ive even gotten some free stuff in the past. I hope they come through with a resonable solution. From past experience they value feedback on product improvement greatly so others dont struggle with the same issue. Ill let you know how it plays out.
```

---
## \#32 Posted by: wmj259 Posted at: 2016-11-27T23:12:50.485Z Reads: 111

```
It should probably not be a big deal about it being more than 60 days, since it was missing components since day 1. You have a valid case here. Go fight them.:muscle:
```

---
## \#33 Posted by: wmj259 Posted at: 2016-11-28T04:45:44.992Z Reads: 113

```
On a closer look and great zoom of 500% on google chrome for your pics and to compare to ollinboards 4.12 vesc, I dont see any chips actually missing?

Yours:
[http://www.electric-skateboard.builders/uploads/db1493/optimized/3X/3/f/3fb0bc513cab750d09e7675d45e3e35904264f51_1_375x500.jpg](http://www.electric-skateboard.builders/uploads/db1493/optimized/3X/3/f/3fb0bc513cab750d09e7675d45e3e35904264f51_1_375x500.jpg)

@Blasto, Ollins seems to be "missing?" the same pieces?  

Ollin:
[https://images.bigcartel.com/product_images/185259495/20160913_115537.jpg?auto=format&fit=max&h=1000&w=1000](https://images.bigcartel.com/product_images/185259495/20160913_115537.jpg?auto=format&fit=max&h=1000&w=1000)

EDIT: I just noticed what you meant. 
-C31
-C14
-C24
-C26
-The box above C20? (wow thats really a bad bad miss of their part)
-C4

WOWOWOWOW :astonished:
```

---
## \#34 Posted by: Blasto Posted at: 2016-11-28T04:53:07.493Z Reads: 109

```
Ollin is missing R6, but is not part of vedder's bom, it's can be a 0ohm resistor for the 5V USB (input not protected not recommended to use)

So no one has R6

[quote="wmj259, post:33, topic:13737"]
WOWOWOWOW :astonished:
[/quote]

haha I think you got it now
```

---
## \#35 Posted by: JohnnyMeduse Posted at: 2016-11-28T04:54:07.720Z Reads: 109

```
The red one are missing and the yellow ones are not looking the same <img src="/uploads/db1493/original/3X/2/2/22a5da6e0e9116d09ab4a3ecfb7a79b004ce18c7.jpg" width="600" height="499">

EDIT: love that game.... :heart_eyes:
```

---
## \#36 Posted by: wmj259 Posted at: 2016-11-28T05:06:47.970Z Reads: 108

```
Now we just gotta find waldo
```

---
## \#37 Posted by: lox897 Posted at: 2016-11-28T05:42:59.072Z Reads: 108

```
Find Wally, he has a brown top and two bits of solder on the side. Haha
```

---
## \#38 Posted by: TarzanHBK Posted at: 2016-11-28T11:13:33.167Z Reads: 105

```
throw that shit away for safety and trouble avoiding reasons. If someone tries to repair it you´ll find yourself with a much higher bill than with buying a new one
```

---
## \#39 Posted by: JohnnyMeduse Posted at: 2016-11-28T13:52:09.959Z Reads: 102

```
[quote="wmj259, post:36, topic:13737"]
find waldo
[/quote]


I think he got off and stole all the parts.
```

---
## \#40 Posted by: 2-alex-2 Posted at: 2016-11-28T14:08:01.503Z Reads: 101

```
If was me would email the seller point out all the missing parts and explain a local specialist has stated that the missing items has caused the vesc to fail and that you want to receive two new ones. Then if they send some inspect them and if there are some missing parts get them added before you got further and then hope for the best that they are ok.
```

---
## \#41 Posted by: ralphy Posted at: 2016-11-28T14:13:45.707Z Reads: 96

```
I can't imagine they are purposely doing this . Obviously since I had no prior experience I didn't know any better. 

I should have definitely inspected it before using. 

Let's see what they say I wouldn't be surprised if they did t know the parts were missing too.
```

---
## \#42 Posted by: JohnnyMeduse Posted at: 2016-11-28T14:15:52.746Z Reads: 95

```
[quote="ralphy, post:41, topic:13737"]
I can't imagine they are purposely doing this
[/quote]


yes the are doing on purpose, for a cost reduction, the big capacitor are around a 2 to 3 dollar each and the other one around 1 dollars... So it is cost reduction, and they really don't care about your safety.
```

---
## \#43 Posted by: 2-alex-2 Posted at: 2016-11-28T14:19:09.437Z Reads: 96

```
Yea I hope they replace for your sake but they may not but seeing as the product was supplied with missing components then I think you have some rights defiantly. How did you pay ? PayPal ?
```

---
## \#44 Posted by: ralphy Posted at: 2016-11-28T14:35:24.422Z Reads: 100

```
So they reduce production cost to stay competitive in the market and when it fails and they get a charge back and a bad rep online what happens .

Sometimes it makes me laugh on some of these strategies to do business overseas.
```

---
## \#45 Posted by: Karen_Vanda Posted at: 2016-11-29T12:25:33.728Z Reads: 96

```
Hello all, PCBA quality is critical because it's a heart of products. We as a manufacturer we know every little detail matter when we produce products from components, tools, solder quality, temperature and environment cleanness. All those combine together, you can see the difference from the photos below. 



<img src="/uploads/db1493/original/3X/0/0/00b9dedef8975869493fcd136f1d42a3abe91b4f.jpg" width="690" height="387">

<img src="/uploads/db1493/original/3X/4/f/4f7ec165738677f7163e8d7012c6225537c3ece1.jpg" width="690" height="390">

In addition, we were aware of the positive leads insulation may get cut through the little studs. Therefore, we cut the studs and put silicon glue over the studs. We want to make sure our users have a safe, fast and fun ride. 

<img src="/uploads/db1493/original/3X/f/e/fed0b03e15c775f79cb0d93ac860b015fab93074.jpg" width="286" height="500">
```

---
## \#46 Posted by: TarzanHBK Posted at: 2016-11-29T14:39:10.390Z Reads: 88

```
nice to see these insights frome a vendor!
```

---
## \#47 Posted by: Okami Posted at: 2016-11-30T09:20:39.272Z Reads: 85

```
[quote="ralphy, post:31, topic:13737, full:true"]
Its been more than 60 days, ive had good luck with motors from them ive even gotten some free stuff in the past. I hope they come through with a resonable solution. From past experience they value feedback on product improvement greatly so others dont struggle with the same issue. Ill let you know how it plays out.
[/quote]

If the warranty / return thing fails.. and you dont get a resolution.. I think there was someone who was willing to get broken vesc.. Just not sure who was this person and in which thread it was mentioned.. 

Though, it would be better if it was not shorted.. but maybe a few componenets that went bad.. if the chip is burnt then that's probably too much work already to repair it
```

---
## \#48 Posted by: ralphy Posted at: 2016-11-30T20:43:46.301Z Reads: 83

```
Its all sent back for their review and repair. They said production has improved and the latest ones are much better. I got the first batch apparently. Tis the season !
```

---
## \#49 Posted by: wmj259 Posted at: 2016-12-28T14:40:11.212Z Reads: 79

```
Any updates?
```

---
## \#50 Posted by: ralphy Posted at: 2016-12-28T16:20:02.752Z Reads: 76

```
Yes 2 new replacements were shipped out through regular post so hopefully they will arrive early next year. I will post pics
```

---
## \#52 Posted by: ralphy Posted at: 2016-12-28T16:23:21.434Z Reads: 77

```
well no i returned a defective one and a good one and im getting two new ones
```

---
## \#53 Posted by: ralphy Posted at: 2017-01-09T04:35:33.427Z Reads: 74

```
Got the new ones two days ago, seems like they fixed the production issue of the missing components and im back on the road! 

I report back if there are any issues and thanks for everyone expertise and advice.
```

---
## \#54 Posted by: wmj259 Posted at: 2017-01-09T19:45:11.063Z Reads: 74

```
Do a check on the soldering and any small connections, look for neatness.
```

---
## \#55 Posted by: bigben Posted at: 2017-05-08T09:52:21.478Z Reads: 53

```
How did this turn out in the end? Did they keep working?
```

---
