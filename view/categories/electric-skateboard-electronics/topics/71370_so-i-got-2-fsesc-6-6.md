# So I got 2 fsesc 6.6

### Replies: 58 Views: 1248

## \#1 Posted by: Holyman92 Posted at: 2018-10-16T04:28:02.313Z Reads: 299

```
I know this isnt normal, which is why I'm posting this. I do t even want to plug this guy in to my battery...

So I bought 2 fsesc and opened them, still factory sealed mind you... 1st thing I always do with Chinese ANYTHING is visually inspect for bad solder joints, cold solder, or something out of the ordinary as I don't like blowing my self up. 

Any who, one of the 2 I got looks BAD 

![15396637958691430392650|375x500](upload://ku2YHfSDoCe5HBFDBoKbqooSQq8.jpeg) 

The weird thing tho, no bad smell usually associated with burned electronics...

Side by side of the 2

![1539663938218626441199|666x500](upload://l9eBSWcCSFMcFWxTWeZBZjB8ckL.jpeg) 

The other 1 I'm about to wire up and set up, but I just sent Flipsky an email to find out what to do... 

@thisguyhere check this out lol
```

---
## \#2 Posted by: thisguyhere Posted at: 2018-10-16T04:32:14.660Z Reads: 285

```
wth, so you took the heatsink off, and underneath the heat sink pad looks burned?

hm...i wonder if anyone else has this, i haven't taken the heatsink off mine to check.

possibly they QA them in house and thermal paste they use is garbage and burns?

looks like soot but i don't see any obvious burned out components...
```

---
## \#3 Posted by: Holyman92 Posted at: 2018-10-16T04:32:28.796Z Reads: 279

```
Oh yea, @thisguyhere the battery issue was the charger... one of the pots inside needed to be adjusted
```

---
## \#4 Posted by: Holyman92 Posted at: 2018-10-16T04:34:37.765Z Reads: 274

```
Yes, I removed the heatsink and there was that burn mark... on the thermal pad. The other pad is perfectly fine
```

---
## \#5 Posted by: thisguyhere Posted at: 2018-10-16T04:35:00.493Z Reads: 269

```
let's see what they have to say about it.
```

---
## \#6 Posted by: Holyman92 Posted at: 2018-10-16T04:35:47.901Z Reads: 273

```
we'll find out tomorrow most likely... it looks like the pads are blown off w/e components those black things are

![15396645572231135437616|375x500](upload://7McywIY3MZEcu61O6fTtYvRBYCi.jpeg)
```

---
## \#7 Posted by: thisguyhere Posted at: 2018-10-16T04:54:07.550Z Reads: 262

```
those are the fets, they're the components that need to be heatsinked
```

---
## \#8 Posted by: Holyman92 Posted at: 2018-10-16T04:55:29.470Z Reads: 261

```
Yea the pads on the top right 2, look like the pads are gone...
```

---
## \#9 Posted by: kalebludlow Posted at: 2018-10-16T06:02:32.674Z Reads: 253

```
The black shit doesn't simply wipe off? If not then I wouldn't power up
```

---
## \#10 Posted by: Holyman92 Posted at: 2018-10-16T08:14:11.937Z Reads: 248

```
it does wipe off but the pads were the fets are supposed to be soldered to are gone, like burnt off... i dont think this unit was ever supposed to leave the factory lol
```

---
## \#11 Posted by: dareno Posted at: 2018-10-16T08:20:47.753Z Reads: 242

```
Yet another victim to Chinese Quality Assurance.  Least with flipsky you will get a result with your complaint.  Blown fets out of the box.  Nice.
```

---
## \#12 Posted by: kalebludlow Posted at: 2018-10-16T08:22:33.471Z Reads: 240

```
Can we get a close up of the FETs of both side by side?
```

---
## \#13 Posted by: Holyman92 Posted at: 2018-10-16T08:22:56.149Z Reads: 239

```
yea, i mean the 2nd esc seems to work perfectly... I've never ran FOC because i was always on 4.12 HW and holy crap is it a noticeable difference in sound and take off... its nice
```

---
## \#14 Posted by: Holyman92 Posted at: 2018-10-16T08:23:59.234Z Reads: 232

```
when i get home from work tomorrow i will take SBS pics again... but its 3am and i have class in the AM followed by work, so ima crash
```

---
## \#15 Posted by: kalebludlow Posted at: 2018-10-16T08:25:38.904Z Reads: 226

```
Of course man no stress
```

---
## \#16 Posted by: Holyman92 Posted at: 2018-10-16T08:26:50.969Z Reads: 236

```
Ignore the screws on the motor can, those are for the enclosure

![15396782867411020753260|375x500](upload://p8zZLJnc9kaV5CgHtumI10iUACj.jpeg) 

![15396783454282004055685|375x500](upload://9Yj1Nsa7u9tVGP3jaHQAeUmB3EY.jpeg) 

![15396796897411320387965|375x500](upload://jvTNEHrCGbpHl9ygCeGd7JiKvOy.jpeg)
```

---
## \#17 Posted by: Holyman92 Posted at: 2018-10-17T21:33:50.428Z Reads: 205

```
**UPDATE**:

So I plugged it in (as per their request for wanting the configuration it's in) It SEEMS to work fine, green light and everything, no fault codes, but when going through the motor setup wizard, it won't spin the motor for detection or even make it do that God awful sound. It's been about 36 hrs since their last reply...
```

---
## \#18 Posted by: Battosaii Posted at: 2018-10-17T21:44:34.646Z Reads: 203

```
Yeah if you blow a fet on a Vesc it will still power on and communicate with your Computer but you won't be able to spin a motor or do detection it's def blown.
```

---
## \#19 Posted by: Holyman92 Posted at: 2018-10-17T21:47:20.862Z Reads: 199

```
never blown a fet before lol... i didnt even want to plug in this ESC so i used an old pack from an Ownboard
```

---
## \#20 Posted by: Battosaii Posted at: 2018-10-17T21:50:37.092Z Reads: 197

```
Yeah super weird how they let that through that obviously would not pass testing let alone physical inspection. It has to be powerd on to blow like that so it probably blew during the QC testing process and they still passed it...
```

---
## \#21 Posted by: Holyman92 Posted at: 2018-10-17T21:52:09.582Z Reads: 189

```
thats what im thinking... u cant see the burn marks unless u take off the heatsink
```

---
## \#22 Posted by: Holyman92 Posted at: 2018-10-18T03:16:48.841Z Reads: 188

```
**UPDATE**: Okay so I had a very nice chat with their fb rep after my friend said that she helped him. Here's the convo thus far, click it to see the whole thing

![Screenshot_20181017-220845|42x500](upload://qrYTOOdpOSVCZMsP4ErMHJHU368.jpeg)
```

---
## \#23 Posted by: AreaKruzer Posted at: 2018-10-18T04:26:53.809Z Reads: 182

```
@BarbaraZ is on this forum as well.
```

---
## \#24 Posted by: Blix Posted at: 2018-10-21T12:09:28.384Z Reads: 175

```
Pictures are glitched atm I think, what was the outcome of the chat?
```

---
## \#25 Posted by: Holyman92 Posted at: 2018-10-21T17:58:57.574Z Reads: 169

```
Don't know they haven't gotten back to me, giving them til Monday their time and I'm gonna message them again
```

---
## \#26 Posted by: Holyman92 Posted at: 2018-10-24T14:47:09.437Z Reads: 163

```
Update: rather than RMA the esc she's asking me to take 50% of the blame for their shotty QC >_>

![Screenshot_20181024-094357|281x500](upload://94dBldRGhevizAxKirq93RiI108.png)
```

---
## \#27 Posted by: moon Posted at: 2018-10-24T14:49:02.209Z Reads: 157

```
Did you pay with PayPal?
```

---
## \#28 Posted by: Holyman92 Posted at: 2018-10-24T14:55:09.524Z Reads: 155

```
Got it from thisguyhere who got them in the group buy I believe, but yes I did, just don't wanna file a claim with PayPal since it wasn't thisguyhere's fault this was just a DOA part
```

---
## \#29 Posted by: moon Posted at: 2018-10-24T15:00:46.536Z Reads: 155

```
Oh right ok.. I don't know why they can't take full blame.

It's clear that their prices are too low to cover stuff like this
```

---
## \#30 Posted by: Komamtb Posted at: 2018-10-24T15:09:13.891Z Reads: 153

```
I had the same issue with the "we give 50% off" this seems to be common warranty procedure with them. @BarbaraZ what the...?
```

---
## \#31 Posted by: Holyman92 Posted at: 2018-10-24T15:10:02.700Z Reads: 152

```
Pretty sure that's who I'm talking to on Facebook lol ^^
```

---
## \#32 Posted by: thisguyhere Posted at: 2018-10-24T15:13:02.811Z Reads: 151

```
good of ya.

i can kick back some monies though, this is kind of f'd up.
```

---
## \#33 Posted by: Holyman92 Posted at: 2018-10-24T15:14:21.294Z Reads: 149

```
Sad part is, I'm not even unhappy with the working one, it set up with no issues and works better than I expected if I'm being honest
```

---
## \#34 Posted by: briman05 Posted at: 2018-10-24T15:32:37.484Z Reads: 147

```
@thisguyhere why dont you do a paypal charge back or @Holyman92 tell them you will do a paypal charge back to get your money back if they dont take full responsibility and send you a new one.  I keep wanting to get one of these vesc either 2 fsesc 6.6 or the dual but stuff like this keeps me from pulling the trigger.  It seems like there is no QC at all in china except in a few factories.  Hell look at enertions thermal pads had the film still on some of them when they left.  It is visually showing signs that it had blown so how did it get thrown in a bag and marked good.
```

---
## \#35 Posted by: Holyman92 Posted at: 2018-10-24T16:21:31.139Z Reads: 143

```
I think @Hummie would be the one that has to do a chargeback, basically it would be me doing a charge back, then this guy, then Hummie lol
```

---
## \#36 Posted by: brenternet Posted at: 2018-10-24T16:24:57.029Z Reads: 144

```
Let us know how this goes please because @Giga and I are In a similar situation for one that I sold to him and is non functional. They've offered him 30% off a new one though... which is frankly just straight bullshit
```

---
## \#37 Posted by: Holyman92 Posted at: 2018-10-24T16:26:38.891Z Reads: 143

```
@brenternet I update this post as they message me. Sorry to hear about y'alls situation... however I am a bit relived that it's not just me
```

---
## \#38 Posted by: chuttney1 Posted at: 2018-10-24T17:06:33.116Z Reads: 142

```
I got one of the FSECS 6.6 and did not receive those black marks on the PCB. The black markings on that thermal pad should not be there. Interesting the version you got has the capacitors with heat shrink.
```

---
## \#39 Posted by: Hummie Posted at: 2018-10-24T18:48:25.487Z Reads: 138

```
I can write n see. What u want me to do?
```

---
## \#40 Posted by: Holyman92 Posted at: 2018-10-24T19:16:26.658Z Reads: 142

```
@Hummie, I'm gonna see how this plays out, if they don't want to do an RMA and mail me a new one, then I'd say do a charge back and reimburse @thisguyhere for 1 and then ill have him reimburse me for 1 

@thisguyhere, that sound good?
```

---
## \#41 Posted by: thisguyhere Posted at: 2018-10-24T19:23:32.093Z Reads: 132

```
that's a long chain to manage but let's try it out
```

---
## \#42 Posted by: Hummie Posted at: 2018-10-24T19:49:17.510Z Reads: 133

```
They probably want a good demonstration that it’s broken.   I think ur best bet is to make a video.  Too bad the video wasn’t done when you first opened and ran it.  Thinking i should do that with everything, not that I ever have before
```

---
## \#43 Posted by: Holyman92 Posted at: 2018-10-24T20:01:07.353Z Reads: 132

```
i mean a picture of a blown fet should be adequate... no fets, no work lol...
```

---
## \#44 Posted by: briman05 Posted at: 2018-10-24T20:44:47.231Z Reads: 127

```
You do more than me I dont even take pictures before I open electronics maybe I should start.  I would think if they said to try and power it on and see what happens would mean they are at fault.
```

---
## \#45 Posted by: Holyman92 Posted at: 2018-10-24T21:53:36.976Z Reads: 123

```
i always photograph new parts when they arrive for build logs and my fb/ig page
```

---
## \#46 Posted by: Kug3lis Posted at: 2018-10-25T13:55:17.741Z Reads: 116

```
Try to remove that heatshrink from capacitors on broken one to see what is hidden maybe after some good sales they started to cheap out and replace with shitty parts like always china does :)
```

---
## \#47 Posted by: Holyman92 Posted at: 2018-10-25T14:57:26.643Z Reads: 111

```
@Kug3lis i'll dissect if they choose to not  to RMA and we have to charge back
```

---
## \#48 Posted by: Holyman92 Posted at: 2018-11-01T02:01:09.387Z Reads: 106

```
@Hummie @thisguyhere

I think i would like to proceed with a charge back. It's been a whole week with 0 response to my message where I stated if we could not come to an agreement for an RMA that I would proceed with a charge back.
```

---
## \#49 Posted by: Holyman92 Posted at: 2018-11-01T02:10:06.821Z Reads: 104

```
Just so everyone knows, this experience has left a bad taste in my mouth with their company... but the product (when it's not DOA) works great. I even bought a dual 6.6, anti-spark switch, and their Bluetooth module to test on a new build. They arrived today (befpre y'all ask, no it was not from them so I didn't take their offer for 50% off and try to charge back as well) I ordered from @hyperIon2 as I like to support local businesses as much as I can even if there is a small mark up

![received_337256966823828|666x500](upload://lUm4mcvmhgmkqghE6pQoGV9ujIf.jpeg)
```

---
## \#50 Posted by: thisguyhere Posted at: 2018-11-01T02:56:43.980Z Reads: 100

```
sure, let's do it.

tell me what to do, @Hummie can you even do a partial charge back?  doubt it.
```

---
## \#51 Posted by: Hummie Posted at: 2018-11-01T04:34:27.394Z Reads: 97

```
Can u fix it instead of being a loss? Shame to throw it when at least half goes right?  Isn’t somebody like @JohnnyMeduse capable of making it go cheap.  

What is a chargeback and what is n RMA?
```

---
## \#52 Posted by: Holyman92 Posted at: 2018-11-01T05:45:27.334Z Reads: 93

```
RMA- return merchandise authorization. 

As for repairing it, the pads for the blown FETs are gone, blown clean off, it would need an interesting fix... as well as a couple FETs. 

I might be able to take it to work and throw it under the microscope to see if there is ANY hope of fixing it. But I seriously doubt it.
```

---
## \#53 Posted by: Holyman92 Posted at: 2018-11-01T05:51:36.621Z Reads: 95

```
As for @Kug3lis's request, here's the pic of the caps unsheathed

![15410514526452047709121|375x500](upload://zh0HCGZ6yAj88hgCZJCpJrv2fKO.jpeg)
```

---
## \#54 Posted by: Holyman92 Posted at: 2018-11-05T07:10:20.272Z Reads: 82

```
@Hummie so I looked at it at work under the microscope and the pads are gone, no where to solder the FETs to, and FS stands by their offer of 50% off and not wanting to fix the issue as they seem to only be interested in $$ and not actually fixing their QC issues

![Screenshot_20181105-010439|654x500](upload://wwqMHzl2ahTRKS0lKIdzSg4Mpvi.jpeg)
```

---
## \#55 Posted by: briman05 Posted at: 2018-11-09T21:25:16.032Z Reads: 66

```
I really love the QC passed sticker on it.  It seems like overall the 6.6 work but some do have some turds in the group
```

---
## \#56 Posted by: Holyman92 Posted at: 2018-11-09T21:26:37.389Z Reads: 66

```
its been handled finally after i got really mean w/ them they finally agreed to send a replacement out for the cost of shipping
```

---
## \#57 Posted by: briman05 Posted at: 2018-11-09T21:30:05.104Z Reads: 63

```
I think you should post what you said to them to get them to send one out to you this way everyone knows what to say.  Glad they finally fixed there screw up.

Should we start a pool to see if they just look at it, throw it back in they back and send it back out.
```

---
## \#58 Posted by: Holyman92 Posted at: 2018-11-09T21:34:07.858Z Reads: 59

```
basically just threatened to do a charge back and file a claim w/ paypal and that i was pissed off
```

---
