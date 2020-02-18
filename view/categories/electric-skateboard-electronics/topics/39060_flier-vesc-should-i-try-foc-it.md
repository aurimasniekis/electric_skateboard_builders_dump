# Flier VESC - should I try FOC it?

### Replies: 22 Views: 1216

## \#1 Posted by: Tomer Posted at: 2017-11-23T09:04:15.631Z Reads: 171

```
I just received a Flier VESC that was for sale on 11.11. Got it with an anti-spark switch, great deal.
It comes with v2.54 firmware installed over, and a bootloader. I'll update it soon to v3.32.

Flier states that this VESC is FOC compatible, although I have my doubts.
As I don't want to fry it, does anyone know if this VESC will pass FOC without any issue?
Did a search and Flier VESCs don't seem to be very popular in this forum.

It even comes with a heat sink which is nice.

<img src="/uploads/db1493/original/3X/1/d/1de90ecd8d1c670980be5386cb7f32334ea35647.png" width="525" height="341">
```

---
## \#2 Posted by: TarzanHBK Posted at: 2017-11-23T09:15:24.851Z Reads: 165

```
Don´t use FOC on that vesc.
Like other cheap ones, these are made with the standard BOM without any modifications to properly run FOC.

If you really want to use FOC, you have to get one of the upgraded, more expensive ones.

With vescs it´s most of the time "you get what you pay for".
```

---
## \#3 Posted by: pennyboard Posted at: 2017-11-23T09:17:20.954Z Reads: 165

```
^^^ What he said. Basically the only vescs you'd want to run FOC on are ollin boards, FOCbox, axle vesc, and maybe esk8.de vesc
```

---
## \#4 Posted by: Tomer Posted at: 2017-11-23T09:19:38.906Z Reads: 157

```
Well, $128.00 is not that cheap for a VESC.
```

---
## \#5 Posted by: TarzanHBK Posted at: 2017-11-23T09:21:47.012Z Reads: 154

```
well that´s a pretty bad deal for that vesc unfortunately...
80 - 90 bucks, maybe 100 with heatsink is ok for that.
```

---
## \#6 Posted by: Tomer Posted at: 2017-11-23T09:26:00.486Z Reads: 152

```
Yes, it's a pretty bad deal.
I got it for $128.00 and anti-spark switch with free shipping so I don't feel that bad.

Thing is that Maytech are well known for non FOC support, they even strongly declare not to use it.
Flier states by themselves that their VESC can do FOC. I also contacted them to double check it, they 
claim that it can run FOC and had no issues whatsoever with any customer.

Comes to think about it, I think I'm their only customer.
```

---
## \#7 Posted by: TarzanHBK Posted at: 2017-11-23T14:41:52.032Z Reads: 129

```
Yah Maytech are a bit better with their marketing like:
We are better then Flier Vescs and deliver an good standard Vesc without any upgrades.
And it´s true, their Vescs are really ok for about 90 bucks! But like i said before, don´t use a standard Vesc in Foc mode.. your vesc will blow up sooner or later!

There was a time a few months ago where you could get a Flier Vesc for about 60-70 bucks, because everyone wanted to get rid of these..
```

---
## \#8 Posted by: Yecrtz Posted at: 2017-11-23T14:52:51.143Z Reads: 121

```
I ran FOC on mine since I had it, without problems.. (vesc from DIY). 10s with 192kv. That's for over a year now.
```

---
## \#9 Posted by: Tomer Posted at: 2017-11-24T15:35:17.293Z Reads: 110

```
Guys, this must be a joke.
Before I placed my order for this VESC I asked Flier if their VESCs are FOC compatible. 
Here's the answer I received:
<img src="/uploads/db1493/original/3X/8/e/8e0ab95e5aa3f637e75fb78c8990c86f800a4acd.png" width="690" height="223">

After I got my VESC, this is what they're replying me back.
<img src="/uploads/db1493/original/3X/e/d/ed13b9cf83b22a5775ab091336ce59a9ba0378a1.png" width="690" height="238">

In addtion, this is what they write under them item description. 
<img src="/uploads/db1493/original/3X/d/9/d9874758fd153b74f1e6e80e8b69dca523c1d704.png" width="690" height="14">

**Are you kidding me???**

Do you think I'll be able to open a dispute and get my money back?
This is totally scamming their buyers.
```

---
## \#10 Posted by: pennyboard Posted at: 2017-11-24T16:02:14.853Z Reads: 103

```
To be fair, several people told you that it wasn’t a good idea to run Foc on that, let alone buy one. You could still get a focbox for $100 for Black Friday Which can run FOC. 
At this point, file a dispute, you have good evidence. And try to return it. Otherwise I say just try FOC and if it blows up, claim it blew up running bldc (by sure to reprogram before you send it back) and demand they repair it under warranty
```

---
## \#11 Posted by: Tomer Posted at: 2017-11-24T16:07:51.741Z Reads: 99

```
I'm going to get a FOCBOX, price is too good with Monday Cyber sale.

I asked here after I received them, I was too impulsive upon purchasing them. I learned my lesson.

I didn't try to run FOC on them. I'll keep them in BLDC as for now.
```

---
## \#12 Posted by: Tomer Posted at: 2017-11-25T16:25:47.131Z Reads: 94

```
What do you think guys?

<img src="/uploads/db1493/original/3X/c/5/c5f76bc5120d630456a001f727072537c72f1f71.jpg" width="281" height="499">

<img src="/uploads/db1493/original/3X/c/8/c8ab92430aacadcbb5ab71a3ec79db5b6b01d81d.jpg" width="281" height="499">
```

---
## \#13 Posted by: Tomer Posted at: 2017-11-27T20:52:23.507Z Reads: 82

```
I need your help here guys.

What would you do if you were me? I honestly don't know what should I do next.
It's either I try FOC and hope for the best, if something will happen Flier will fix it under warranty.
I have the feeling that something will happen (if not at the beginning, then at some point) and then 
I'll not be able to ask for a refund. Or maybe will I...? 

On the other hand, how can they be so confident about their VESC and FOC? Are they completely
 lying to me?
```

---
## \#14 Posted by: Mattmccrary8 Posted at: 2017-11-27T20:55:26.861Z Reads: 80

```
Don’t try FOC. I got a DRV failure on my TB one a month ago.
```

---
## \#15 Posted by: b264 Posted at: 2017-11-27T21:24:24.258Z Reads: 79

```
I think you have 2 options -- the best one is to return/dispute that since they lied in the advertising and get a focbox or two TODAY from enertion while they are $97usd

The other option is to run 7S5P or 7S6P (7S max voltage) because it'd be **significantly** harder to break something if you turned down the voltage and current and didn't "push it" to the max
```

---
## \#16 Posted by: Tomer Posted at: 2017-11-27T23:24:46.659Z Reads: 70

```
I already purchased x6 FOCBOXs today :sweat_smile:

I'll contact the seller tomorrow and will ask to return it and demand them to pay the shipping costs.
If not, I'll open a dispute. However, I'm not able to open a dispute yet because you can only do it after
10 days since the day of placing an order. I received the VESC after two days from China :open_mouth:
```

---
## \#17 Posted by: b264 Posted at: 2017-11-27T23:34:50.068Z Reads: 68

```
[quote="Tomer, post:16, topic:39060"]
I already purchased x6 FOCBOXs today
[/quote]

Begin the celebrations! :-D  I got 4 myself
```

---
## \#18 Posted by: pennyboard Posted at: 2017-11-28T04:53:59.041Z Reads: 64

```
It's basically only a matter of time before it fries if you FOC it. Honestly the best thing to do is probably dispute it and return it and get your money back. And then have fun with your 6 FOCBoxes
```

---
## \#19 Posted by: Tomer Posted at: 2017-11-28T09:21:57.198Z Reads: 64

```
This is getting too funny.

There's a lot of hype from the Chinese vendors (Flier, Maytech) since the new v3.3 firmware.
Suddenly, all of their VESCs can run FOC, at least that's how they are advertising it.
But when you ask them if there's a chance that a VESC will get fried, they don't know the answer. 
They claim this without even do proper QA on their products.

<img src="/uploads/db1493/original/3X/d/0/d00785fdeb740e14fbb495c47d4376057066a074.png" width="690" height="325">
```

---
## \#20 Posted by: rich Posted at: 2017-11-28T11:14:52.220Z Reads: 60

```
Man, they are really joking! I can confirm Maytech don't work in FOC no matter which FW. It's an own chapter in the manual but if you ask them they say don't run FOC longer than 10 seconds. This is just ridicolous :expressionless:

I'm sure they even don't know what FOC is :joy:
```

---
## \#21 Posted by: ramon Posted at: 2017-11-29T16:50:50.241Z Reads: 50

```
I've also bought the same vesc for 93€ the 11.11 and now that the FOCBOX is 81,89€ I'm so annoyed :sob:
Nevertheless, with shipping and taxes a FOCBOX would cost me arround 100€ and I would still have to pay custom office taxes which were arround 25€ for the last enertion vesc I bought. Thats my only consolation :joy:
```

---
## \#22 Posted by: Tomer Posted at: 2017-12-06T07:23:44.129Z Reads: 39

```
I guess I'm a beta-tester now.

<img src="/uploads/db1493/original/3X/a/c/ac107601b27dedf059dbeec57568019279eb2299.png" width="690" height="301">
```

---
