# Enertion Vesc with drv8032 fault code

### Replies: 79 Views: 4279

## \#1 Posted by: NNGG Posted at: 2016-07-25T07:10:41.665Z Reads: 204

```
When I press throttle on my vesc, it blinks red 3 times and does nothing. Has any one had this issue?
```

---
## \#2 Posted by: boards Posted at: 2016-07-25T07:16:34.123Z Reads: 198

```
fault code, hook it up to bldc tool and check the code
```

---
## \#3 Posted by: NNGG Posted at: 2016-07-25T07:17:24.266Z Reads: 195

```
How do I check the code? Is it under real time data?
```

---
## \#4 Posted by: boards Posted at: 2016-07-25T07:30:16.319Z Reads: 189

```
yeah, <img src="/uploads/db1493/original/2X/1/163caa047a73c7da4324f71956274a22575329db.png" width="380" height="500">

connect vesc, hit realtime data, check activate sampling, then press throttle.

if you have been using foc / been unlucky you'll get the drv8032 error :(
```

---
## \#5 Posted by: NNGG Posted at: 2016-07-25T07:39:49.433Z Reads: 181

```
So I got the fault code drv 8032, what now?
```

---
## \#6 Posted by: NNGG Posted at: 2016-07-25T07:40:16.314Z Reads: 182

```
Motor detection was fine and I had my limits on the default settings
```

---
## \#7 Posted by: boards Posted at: 2016-07-25T07:40:30.237Z Reads: 181

```
replace drv8302 chip
```

---
## \#8 Posted by: NNGG Posted at: 2016-07-25T07:43:22.560Z Reads: 181

```
Is it my fault? Doees enertion have this under warrenty?
```

---
## \#9 Posted by: Jinra Posted at: 2016-07-25T15:28:03.011Z Reads: 170

```
did you buy platinum? Should be covered if you did. They also warranty their electronics for two months without it IIRC. We're you using FOC?
```

---
## \#10 Posted by: NNGG Posted at: 2016-07-25T17:10:42.274Z Reads: 165

```
No I bought the vesc when there was no platinum option. I also only did motor detection on bldc on 6s and 10s. After that my vesc just quit.
```

---
## \#11 Posted by: Blasto Posted at: 2016-07-25T17:14:46.531Z Reads: 164

```
Post some close up pictures of your setup. If you lucky we may be able to help you out
```

---
## \#12 Posted by: NNGG Posted at: 2016-07-25T17:22:27.178Z Reads: 162

```
<img src="/uploads/db1493/original/2X/f/fa832fb6741f636a4fd968c0d9b9932aa86a994f.jpg" width="375" height="500">
```

---
## \#13 Posted by: NNGG Posted at: 2016-07-25T17:24:07.695Z Reads: 162

```
<img src="/uploads/db1493/original/2X/1/169c1525194e86acf5a6130cf6d35e7a5600a2a5.jpg" width="375" height="500">


This one is before I connected the vesc to bldc tool
```

---
## \#14 Posted by: NNGG Posted at: 2016-07-25T17:26:54.660Z Reads: 159

```
<img src="/uploads/db1493/original/2X/b/b575672c72e97d8db66a02f76568e6e4d462a731.jpg" width="375" height="500">


It is a vesc with one of the 50v capacitors so I only put NiMh batteries, 6s and 10s instead of my original 12s plan. Motor detection failed on 6s but worked on 10s
```

---
## \#15 Posted by: NNGG Posted at: 2016-07-25T17:27:41.547Z Reads: 158

```
<img src="/uploads/db1493/original/2X/d/dcd853abf0ec1fee7fc2008a00ddf5d25040369d.jpg" width="375" height="500">
```

---
## \#16 Posted by: Blasto Posted at: 2016-07-25T17:31:27.235Z Reads: 156

```
and your motor leads and battery connection

[quote="NNGG, post:14, topic:6584"]
NiMh batteries
[/quote]

I'm not sure nimh batteries have enough punch to drive the motor properly
```

---
## \#17 Posted by: NNGG Posted at: 2016-07-25T17:39:30.097Z Reads: 151

```
I used them the first time to check for the bldc settings
```

---
## \#18 Posted by: NNGG Posted at: 2016-07-25T17:40:01.641Z Reads: 151

```
I didn't use NiMh for batt detection
```

---
## \#19 Posted by: Blasto Posted at: 2016-07-25T17:42:41.640Z Reads: 153

```
not crazy about this:

<img src="/uploads/db1493/original/2X/f/fbcc73996785d0dc34ada74e81cfc8ef1006a313.png" width="375" height="500">

but i don't think this is the root cause of your problem, your mcu would have been roasted
```

---
## \#20 Posted by: NNGG Posted at: 2016-07-25T18:59:08.084Z Reads: 150

```
That's just the clear heat shrink
```

---
## \#21 Posted by: Blasto Posted at: 2016-07-25T19:34:41.893Z Reads: 147

```
I was refering to your red battery wire going over the bottom of your sensor connector. That has the potential to pierce the wire and have your battery voltage fry your mcu.

But i dont think this is the case now
```

---
## \#22 Posted by: NNGG Posted at: 2016-07-26T00:40:20.592Z Reads: 134

```
Any ideas on what I should do? Im confident that the default settings should have protected the vesc, and there arent any shorts. I havent even put a load on the motor when it was connected to the vesc
```

---
## \#23 Posted by: evoheyax Posted at: 2016-07-26T00:49:35.275Z Reads: 134

```
Welcome to the club. Is this the new batch made in the USA?

I had one enertion VESC arrive broken, the other broke on the second day. You will get blamed for breaking it and you will get no service. Buy your vesc's from Chaka and problem solved. I only buy chakas vesc's now becuase quality is everything with the VESC, and if anything goes wrong, you'll actually get helped instead of blamed and no service.
```

---
## \#24 Posted by: lox897 Posted at: 2016-07-26T00:58:04.779Z Reads: 129

```
Aren't these VESCs higher quality? Seems like they are breaking as much as the ones made in China.
```

---
## \#25 Posted by: Blasto Posted at: 2016-07-26T01:15:30.151Z Reads: 125

```
Well lets see those motor connections, you replaced the xt60 for some dean connectors, do you mind opening up your shrink?
```

---
## \#26 Posted by: NNGG Posted at: 2016-07-26T01:22:01.282Z Reads: 124

```
I replaced them with deans
```

---
## \#27 Posted by: NNGG Posted at: 2016-07-26T01:22:12.084Z Reads: 128

```
it is the new batch, The vescs have a 60 day limited manufacturing warrenty. So I'll contact support
```

---
## \#28 Posted by: NNGG Posted at: 2016-07-26T01:25:32.537Z Reads: 123

```
[Uploading...]()


No way for a short to happen<img src="/uploads/db1493/original/2X/0/0ec96f7c86f285e7e91d6d2de9715d8f170db063.jpg" width="666" height="500">
```

---
## \#29 Posted by: NNGG Posted at: 2016-07-26T01:26:39.908Z Reads: 125

```
that is heat shrink with electrical tape and more heat shrink, my theory is maybe capacitors are shit or bldc tool bugs
```

---
## \#30 Posted by: onloop Posted at: 2016-07-26T01:28:50.301Z Reads: 129

```
[quote="evoheyax, post:23, topic:6584"]
You will get blamed for breaking it and you will get no service.
[/quote]

We offer a VESC-PLATINUM with a 12 month no questions asked replacement warranty, did you buy that one?, its the same price as OllinVESC.... if so you get a new one sent to your door for any fault, If you didn't & took the cheaper option you get less service.
```

---
## \#31 Posted by: NNGG Posted at: 2016-07-26T01:29:24.420Z Reads: 129

```
there wasnt that option when I bought it, but do you have any ideas? I am curious as to the reason is the chip has a fault code. Could I do anything on the bldc tool to double check?
```

---
## \#32 Posted by: onloop Posted at: 2016-07-26T01:33:21.380Z Reads: 129

```
[quote="NNGG, post:31, topic:6584"]
there wasnt that option when I bought it,
[/quote]

it's available as a separate purchase, if you buy it now ill send you a new VESC.

http://www.enertionboards.com/electric-skateboard-parts/1yr-vesc-replacement-warranty/

otherwise return the VESC to the manufacturer and they can investigate it, but not guarantee we can get it fixed.
```

---
## \#33 Posted by: NNGG Posted at: 2016-07-26T01:33:42.007Z Reads: 127

```
[quote="onloop, post:30, topic:6584, full:true"]

We offer a VESC-PLATINUM with a 12 month no questions asked replacement warranty,
[/quote]

Seems kinda easy to fake a fault code and pretend to have a broken esc and get two vesc for $160
```

---
## \#34 Posted by: NNGG Posted at: 2016-07-26T01:34:39.793Z Reads: 123

```
Thank you for the offer, can I email enertion support, and ask them any questions? Will that do anything?
```

---
## \#35 Posted by: onloop Posted at: 2016-07-26T01:36:38.179Z Reads: 124

```
[quote="lox897, post:24, topic:6584, full:true"]
Aren't these VESCs higher quality? Seems like they are breaking as much as the ones made in China.
[/quote]

why do you insist on making uninformed broad sweeping statements like this? 

we just shipped 1000 vesc in the last 4 weeks... how many have you seen being reported as faulty?
```

---
## \#36 Posted by: NNGG Posted at: 2016-07-26T01:38:49.314Z Reads: 122

```
Why do people get different capacitors? some get  63v and some get 50v (myself included)
```

---
## \#37 Posted by: Blasto Posted at: 2016-07-26T01:46:55.811Z Reads: 123

```
[quote="NNGG, post:33, topic:6584"]
Seems kinda easy to fake a fault code and pretend to have a broken esc and get two vesc for $16
[/quote]

I'm sure you need to send the broken one in anyways
```

---
## \#38 Posted by: NNGG Posted at: 2016-07-26T01:49:01.234Z Reads: 122

```
I hope so.
```

---
## \#39 Posted by: evoheyax Posted at: 2016-07-26T02:18:41.306Z Reads: 139

```
Your assumption is people are using them immediately. The reality is, a lot of people get them and they sit on desks for a few months. Look at hummies hubs. He's shipped to dozens of people over the last 8 months or so, and in the last month since you made that video, your finally seeing people use them. I bought two vesc's from you, and I didn't use them for 3 or 4 months until I could figure out a) how to use them and b) what I was going to use them with. It's too early to know right now of the quality. I know chakas are of high quality, they've been out in the field for quite some time. These vesc's are new, and barely tested. I would expect due to the manufacturing changes that they are better, but it's like, why go to an untested source when there's a tried and tested one?
```

---
## \#41 Posted by: onloop Posted at: 2016-07-26T02:36:01.637Z Reads: 131

```
[quote="NNGG, post:36, topic:6584, full:true"]
Why do people get different capacitors? some get  63v and some get 50v (myself included)
[/quote]

About 100 people got a 50v cap. Has been tested and works well with 10S. If you are using 12s I'll buy you some caps.
```

---
## \#42 Posted by: onloop Posted at: 2016-07-26T02:41:17.761Z Reads: 129

```
What questions do you want to ask? 

If it's somthing that can be answered here on the forum you should avoid emailing us. 

Otherwise feel free to email us.
```

---
## \#43 Posted by: lox897 Posted at: 2016-07-26T02:52:42.476Z Reads: 128

```
I am just interested to know why Chaka's VESCs are less prone to breaking if you use the same high quality components? I have seen 4 reports of VESCs breaking in one day, and how many have actually been delivered? No hate, just interested to know. I'm sure your VESCs wont have any issues soon.
```

---
## \#44 Posted by: NNGG Posted at: 2016-07-26T02:55:55.057Z Reads: 126

```
Is the drv chip fixable, or is it only replaceable? 
Where are the schematics for the drv chip?
```

---
## \#46 Posted by: onloop Posted at: 2016-07-26T04:15:31.986Z Reads: 121

```
[quote="lox897, post:43, topic:6584"]
I am just interested to know why Chaka's VESCs are less prone to breaking
[/quote]

what makes you think his VESC don't fail?

.... if his VESC never failed how did he get a reputation for offering great after sales service & repair on VESC?? 

the reason you hear about enertion VESC problems more often is because there are more enertion customers on this website & we sell more VESC units. 

So far we have shipped 1000 VESC from our new American factory, we are the only VESC supplier who are assembling VESC to IPC-A-610 Class 2 standards, initial feedback is that failure rates are very low & we also have the best warranty to ensure anyone with a faulty VESC gets a brand new one sent to them.

AS of the 5th of August, VESC will ship same day they are ordered.
```

---
## \#47 Posted by: whitepony Posted at: 2016-07-26T04:26:27.780Z Reads: 122

```
one of my 2 march 2016 vescs came with a drv8302 fault - hooked it up, first testspinup with notebook up & downarrow -> blinking LED right away. didnt even run motor detection nor did I change any settings at that point (hooked up to 6355 rspec).

when I hooked up the 2nd vesc in the exact same hardware environment, it worked right away.

I broke a few german vescs, but these were always my fault - this time I dont feel like I should assume responsibility, especially not after vesc no2 works flawless int he exact same environment. mailed enertion support, but no reply yet and reading through this thread I got a feeling Ill just be sitting there with a broken vesc that never ran once.

not sure whats that platinum vesc thing - when I ordered my vesc in the first march week, there were just vescs and nothing else. ontop of that it was written on the enertion page, that the vescs will ship from europe. I then specifically mailed you that question again to be sure and you said 

_"Yes, you have heard correctly and we are setting up an EU warehouse as we speak! it should be up and running for your VESC shipment."_

ok, "should be" leaves room for interpretation - if I knew I had to pay import taxes, I never wouldve ordered these vescs. basically now I bought 2 for the price of nearly 3 and all I got was 1. :joy:
```

---
## \#48 Posted by: onloop Posted at: 2016-07-26T05:02:26.615Z Reads: 115

```
@whitepony

Sorry to hear of your problems. As you are In EU it makes it harder for me to fix your problems.

However here are your options.
1. Buy the vesc warranty & I'll send you a new one, maybe you will be charged tax I can't guarantee you won't.. (This is a special option only for people who didn't get that option due to ordering before it existed)

2. Return the vesc to our American manufacturer and we will get it repaired. Once again maybe you will get tax bill.


Regarding the EU distributor
I am sorry to say the timing for this didn't work out. I suppose we could have waited longer but there was so many people becoming impaitent. We couldn't delay any longer. However it looks like we now have the option. All future VESC should be able to be shipped from Belgium. We will send them to Belgium with duty prepaid. So soon we can offer EU customer VESC shipments, without import tax and super fast same day shipping.
```

---
## \#49 Posted by: NNGG Posted at: 2016-07-26T05:20:01.993Z Reads: 112

```
is there any way for me to send my vesc to the us supplier to change the drv chip?
```

---
## \#50 Posted by: lox897 Posted at: 2016-07-26T05:27:57.607Z Reads: 110

```
I've seen one report of a broken VESC from Ollin and I think it was from user error.
```

---
## \#51 Posted by: NNGG Posted at: 2016-07-26T05:36:21.986Z Reads: 112

```
I feel that is where ollin usually gets screwed over with user error.
```

---
## \#52 Posted by: lox897 Posted at: 2016-07-26T05:40:59.299Z Reads: 112

```
I'm quite sure @chaka tests his VESC throughly before shipment.
```

---
## \#53 Posted by: onloop Posted at: 2016-07-26T05:47:36.505Z Reads: 112

```
[quote="lox897, post:52, topic:6584, full:true"]
I'm quite sure @chaka tests his VESC throughly before shipment.
[/quote]

we built a custom made test rig, all VESC are tested before shipping.

https://www.youtube.com/watch?v=N9kbYnCEkjw
```

---
## \#54 Posted by: lox897 Posted at: 2016-07-26T05:51:18.650Z Reads: 111

```
What problems does testing eliminate exactly? Does it just upload firmware or does it make sure they don't have problems?
```

---
## \#55 Posted by: whitepony Posted at: 2016-07-26T06:09:24.631Z Reads: 112

```
[quote="onloop, post:53, topic:6584"]
we built a custom made test rig, all VESC are tested before shipping.
[/quote]


my repaired vesc was tested too - with 10V and superlow current. first time I connected it to 40V and spun up the motor once it showed drv8302 error. when I returned it to the repair guy, he just resoldered the drv chip and everything worked fine afterwards. so, even with testing, you can still get a vesc that will fail under some load without any user error really!

[quote="onloop, post:48, topic:6584"]
1. Buy the vesc warranty & I'll send you a new one, maybe you will be charged tax I can't guarantee you won't.. (This is a special option only for people who didn't get that option due to ordering before it existed)

2. Return the vesc to our American manufacturer and we will get it repaired. Once again maybe you will get tax bill.
[/quote]

before I send something off to the US, i can just get it repaired for 60€ by our german vesc support.

about option 1: does it require me to return the broken vesc, or is a video, closeup and faults error log sufficient? with 50€ platinum and customs, its a very close call of doing that, or "buying a hot air soldering station" or "letting the german vesc repair guy fix it for 60€".

either way, it was "false economy" for me.
```

---
## \#56 Posted by: NNGG Posted at: 2016-07-26T06:15:23.513Z Reads: 100

```
Strange, my motor wouldnt spin on 14V, 22 volts or 40 volts, on motor detection. i just got a detection error
```

---
## \#59 Posted by: evoheyax Posted at: 2016-07-26T06:50:03.945Z Reads: 109

```
Talking to Chaka, he has told me he has only had a hand full of customers tell them they have had any issues. You'll probably say the same thing. The difference is, he advertises he'll fix it free of charge. Since you don't, many probably never say anything to you. Some will think they broke it themselves, some will assume nothing will be done since no real warranty is stated. So to assume everyone whose VESC breaks will contact you is a bad assumption. With Chaka, it makes no sense not to contact him, as you know he will fix it. So one is less likely to say nothing due to his warranty. I have always said, I would bet your vesc's fail rate is much higher than you think.

I know this latest batch has higher expectations. I wish every one worked flawlessly, but if the fail rate is as low as you state it is, then it shouldn't cut too much into your profit margins to sell them at the $130 ish USD price and offer a free replace if breaks warranty without any extra charges. I'm sure it costs you less per VESC completed than what chakas paying per VESC in parts unbuilt. Money is usually, but not always, a good indicator of quality. And In this case, I think it speaks loudly.

He started in a similar way that hummie did also, barely profiting if at all for a while, selling them basically at cost like hummie.

Also, I think you under estimate how many vesc's he makes. It's less than you, but it's a lot still. My understanding is he actually does some tests on them besides just powering them on and seeing if there's any fault codes, correct me if I'm wrong @chaka. If the one sent to me from China had been plugged in, and you tried to connect a receiver, you would of noticed it doesn't turn on. Then you would of noticed the ppm positive lead is only outputing 3.2 volts instead of 5 volts. And it never would have been shipped to me in the first place. Connect a motor, connect a receiver, config the motor, and see if it works. A test that simple is much needed.
```

---
## \#60 Posted by: onloop Posted at: 2016-07-26T07:15:13.398Z Reads: 112

```
[quote="whitepony, post:55, topic:6584"]
my repaired vesc was tested too - with 10V and superlow current. first time I connected it to 40V and spun up the motor once it showed drv8302 error.
[/quote]

The simple truth is the DRV8302 chip are a weak link in this application, it can error for many reasons. Many people don't realize it but the DRV8302 can have many different faults, they are not always resulting in permanent hardware failure, in some cases it is possible to simply re-boot and start the VESC again without errors, it really depends on the error & the cause. Also the BLDC tool doesn't distinguish between these different errors, it simply reports a generic fault code. Sometimes a DRV error can be displayed due to a bad motor detection and/or any other less obvious set of circumstances.

[Here is a summary of faults.](http://www.ti.com/product/DRV8302/datasheet/detailed_description?search=fault,code#SLES2676321)

<img src="/uploads/db1493/original/2X/b/be588b8a662cd4b945135d101abe870fd57ef643.png" width="444" height="500">


**The sensitivity of this chip is the reason why Vedder has stopped using it on the VESC 6.0**

As a seller of VESC the best i can do is ship out VESC that work during our thorough bench test, if they fail after that we are left guessing what the problem was, as we cannot see the detailed report, we only know of the generic error message which could be caused by many variables. Some of those instances will be due to user error.

In summary, maybe user error is to blame, maybe not... what is well established is, no matter what the cause is, the end user in the ESK8 market will shame the vendor into accepting responsibility & more often than not they will do this by attributing the DRV fault to inferior assembly quality. The DRV faults, more often than not, has nothing to do with the assembly process and therefore is rarely the responsibility of the VESC vendor. 

Based on this trend of shaming vendors into accepting responsibility & other market research we decided to offer the VESC-PLATINUM product which has the 12 months replacement warranty.

**Here are the best options for purchasing VESC & Having your problems solved if they arise**

**(a) [Enertion VESC-PLATINUM](http://www.enertionboards.com/electric-skateboard-parts/vesc-platinum-1yr-replacement-warranty/)** - inc 12 months instant replacement warranty $165USD (inc free worldwide shipping) 

**(b) Ollin VESC** - no warranty conditions noted - does repair faults when they occur $165USD (+ shipping)

**(c) Esk8.de** - 2 years warranty as per EU law, doesn't cover firmware changes or FOC use $185USD (tax/vat inc for EU customers + Shipping)
```

---
## \#61 Posted by: lox897 Posted at: 2016-07-26T07:25:02.668Z Reads: 107

```
So how come Ollin VESCs don't have as many errors?
```

---
## \#62 Posted by: Maxid Posted at: 2016-07-26T07:27:15.339Z Reads: 110

```
[quote="onloop, post:60, topic:6584, full:true"]
**(c) Esk8.de** - 2 years warranty as per EU law, doesn't cover firmware changes or FOC use $185USD (tax/vat inc for EU customers + Shipping)
[/quote]

So you are saying that FOC use is encouraged on your VESC?
```

---
## \#63 Posted by: onloop Posted at: 2016-07-26T07:37:18.460Z Reads: 112

```
I am saying the Enertion VESC-PLATINUM has a 12 months replacement warranty, do what you want with it, if it fails for any reason you get a new one.
```

---
## \#64 Posted by: evoheyax Posted at: 2016-07-26T07:38:51.794Z Reads: 112

```
I don't think so, not even Chaka is really encouraging FOC. It does seem to cause more problems, I haven't had issues with FOC on chakas vesc's.

It's true also that Chaka doesn't really have any terms stated, but from talking to him, you will understand that at worst case, you pay a bit for shipping and replacement parts if you were a flaming idiot, which he has said he hasn't had to do yet.
```

---
## \#65 Posted by: Maxid Posted at: 2016-07-26T07:38:54.106Z Reads: 113

```
Wow ok - just let me know when the EU warehouse is set up ;)
```

---
## \#66 Posted by: onloop Posted at: 2016-07-26T07:46:43.845Z Reads: 112

```
[quote="lox897, post:61, topic:6584, full:true"]
So how come Ollin VESCs don't have as many errors?
[/quote]

Lachlan, please stop. you have no idea what you are saying & nothing to back it up.

unless you have hacked into ollin systems & are reading all his customer emails you are simply spitting out random chunks of nonsense. 

So please STOP
```

---
## \#67 Posted by: NNGG Posted at: 2016-07-26T07:49:14.728Z Reads: 107

```
The drv chip is a driver for the large mosfets, how does that translate to it being fragile?
```

---
## \#68 Posted by: onloop Posted at: 2016-07-26T07:50:11.085Z Reads: 99

```
[quote="NNGG, post:67, topic:6584"]
how does that translate to it being fragile?
[/quote]

due to the number of people saying so
```

---
## \#69 Posted by: NNGG Posted at: 2016-07-26T07:50:30.972Z Reads: 99

```
Ollin vescs (probably) have the same fail rate, but chaka manually tests the and people directly contact him if they have a problem and it gets fixed quietly and no one hears about it as much
```

---
## \#70 Posted by: lox897 Posted at: 2016-07-26T07:55:20.247Z Reads: 98

```
Jason, I have nothing against Enertion. I love your mounts, drive trains, trucks, wheels, motors also look nice even though I haven't tried them. You are an inspiration for growing your company %1400 in the last year. I am very appreciative of being a moderator here, even though I probably don't deserve it. I even say to my parents how cool your designs are. My parents are a bit sick of me talking about esk8 though... Anyway, I was just interested what you think is the cause of the DRV8302 on your VESCs blowing up.

This is probably the longest reply I have ever done so I am going to stop now. Keep doing what you love to do mate. Peace.
```

---
## \#71 Posted by: onloop Posted at: 2016-07-26T08:10:38.159Z Reads: 99

```
_Finally, someone who is making some sense...._




----------


----------


The fact of the matter is, I am the owner of this forum, I directly refer my customers onto the forum to publicly describe their faults & problems, I promote this forum on my youtube videos, I have links from my website & I also have a shortcut to the forum inside my "automated response emails" when someone submits a support ticket with us. None of the other vendors do this. There is a chance that customers who purchase from my competitors don't use this forum or know about it.

Personally, I think it benefits the community if all the "dirty laundry" is hung up for everyone to see.. I have nothing to hide and i think it is only fair that the general public be given a snapshot of the "real world" - This concept is not shared by my competitors & in most cases they like to hide their faults away from the public.

What forum readers must be careful of is the fact that cases of faults on here are just a "snapshot". It cannot be used as a source of data for your statistical analysis. For accurate information, we need to conduct a large survey of forum users (and ideally all vendors customers) to get any meaningful data... Which i do plan on be doing in the near future. 

the truth of the matter is, There are plenty of vendors who happily use this forum to promote their business but are very careful to ensure their customers never use it to talk down their products.

It's a double edge sword, i love the community because it helps me improve my products & gives me invaluable feedback about my mistakes. I can then use this knowledge to better my competitors... But it also means that my mistakes are all visible for the world to see....

anyway... such is life!
```

---
## \#72 Posted by: onloop Posted at: 2016-07-26T08:21:51.939Z Reads: 93

```
Lachlan, you just need to make sure you are being objective & being careful not to make statements that are written as facts when in fact they are simply your own subjective opinions based on a small dataset. 

_It's like me saying everyone who is under 15 years of age is bad at soldering electric skateboards, because i have viewed pictures on this forum showing that your soldering sucks & you are also under 15._
```

---
## \#73 Posted by: onloop Posted at: 2016-07-26T08:22:32.901Z Reads: 93

```
[quote="Maxid, post:65, topic:6584"]
just let me know when the EU warehouse is set up
[/quote]

they will be getting the first batch by middle of august,.
```

---
## \#74 Posted by: lox897 Posted at: 2016-07-26T08:25:08.975Z Reads: 87

```
[quote="onloop, post:72, topic:6584"]
because i have viewed pictures on this forum showing that your soldering sucks & you are also under 15.
[/quote]

That is a fact though. Haha. I get your point. I need to consider what I am saying before I say it.
```

---
## \#75 Posted by: onloop Posted at: 2016-07-26T08:29:47.552Z Reads: 88

```
[quote="lox897, post:74, topic:6584"]
That is a fact though. Haha
[/quote]

Only if i am talking about your results specifically, If there are 3 other 15-year-olds in the same room I shouldn't assume their soldering quality is going to equal, better or worse than yours simply based on the snapshot of observable results.
```

---
## \#40 Posted by: onloop Posted at: 2016-07-26T08:53:50.157Z Reads: 102

```
4 posts were merged into an existing topic: [Should ESK8 Vendors Make a PROFIT? or NOTHING?](/t/should-esk8-vendors-make-a-profit-or-nothing/6623)
```

---
## \#76 Posted by: lox897 Posted at: 2016-07-26T08:54:59.265Z Reads: 87

```
I am talking about myself. It was humour
```

---
## \#77 Posted by: JohnnyMeduse Posted at: 2016-07-26T14:33:38.663Z Reads: 89

```
[quote="NNGG, post:67, topic:6584, full:true"]
The drv chip is a driver for the large mosfets, how does that translate to it being fragile?
[/quote]


It communication protocol between the DRV and the MCU, for use we have in Esk8, that make the DRV fragile. Also Wrong setting and bad setup are a big part of the famous DRV Failure. (the cause problem with other component that can affect directly the DRV)... AND don't forget the VESC is still some kind of Prototype.
```

---
## \#78 Posted by: NNGG Posted at: 2016-07-26T16:11:31.139Z Reads: 78

```
Thanks for the response
```

---
## \#79 Posted by: Camwar0616 Posted at: 2016-08-19T23:48:58.302Z Reads: 72

```
Hey, I'm not sure if this is the right place for this, can't seem to find a way to PM you so I thought your latest post would work. I am currently trying to build the best board I can for the lowest amount of money, I already have a completed board(not e board) so there's a way to save already. Anyways, while browsing the forums, I stumbled on one of your comments stating this is the best budget build:
"Torqueboards for mounts (unless you are welding) and hobbyking for outrunner motors and lipo batteries. Space cell should be good, but its overpriced and you can make it yourself for half the cost. Buy a good charger (genuine IMAX). I would get a 192kv 6374 motor from HK and run it on 6S. with a vesc. Thats what I would do if I could redo my build again. 
VESC- $100
2* 3S Lipos at 20C- $45
HK outrunner- 90$ ($60-80 is you go for a higher KV)
Motor mount kit from Torqueboards- $75
Separately purchased drive kit- $60 for a 12-15mm belt setup
OR buy torqueboards drive kit which is $120 includes motor mount and belt/pulleys at 9mm
And a charger- 30$ 
Total is gonna round up to $400 with shipping and extra belts and metal bolts plus $100 labor if you time costs money. 
PS you can save: 
$40 on the esc with a 1/8 car esc 
$80 by making your own motor mount 
$20 on the charger buy buying a 3S charger 
$20 on the motor with going for like 230-295kv
Hope I helped."
Just wanted to know if you still stand behind this setup or if new products have emerged or something like that. It would be amazing if you could get back to me, thanks!
```

---
## \#80 Posted by: NNGG Posted at: 2016-08-20T00:13:00.252Z Reads: 75

```
If you want to go cheap,
 buy a 6364 SK3 245kv and run it on 6S on a 150 amp car esc with a programming card and build a li-ion pack. I now see the benifits of them over lipos unless you want a stealth build. 

Buy TQ's motor mount. Hes a great guy and local for me. If your international then maybe elsewhere.

If you want all out buy a reliable 12S esc (ollin/Maytech/TQ) with a 168-192kv motor. I would gear lower just because I want sub 20mph speeds but thats up to you. 

There is a false economy, but its not in the motors, its in the esc and batteries.
```

---
## \#81 Posted by: Camwar0616 Posted at: 2016-08-20T00:34:16.974Z Reads: 78

```
Wow awesome man thanks for responding so quick, a few questions:
The two motors you mentioned are within $10 of each other price wise, so should I just go for the 192kv?
Also I'm totally willing to DIY and build the bat pack, do you have any links to a good forum post or something?
With the vesc vs car esc, is there a notable difference in performance, braking? speed? also how can I rig the car esc?
With the speeds, I have no problem with going over 20, is there something I need to buy to reach those speeds.
Do you have a list or a recommended truck to use, or could I use the ones that came with my board.
Well, that's it, I hate to ask so many questions but I'm new to the scene and extremely interested.
thanks for the help man!
```

---
## \#82 Posted by: NNGG Posted at: 2016-08-20T04:31:57.071Z Reads: 73

```
Well..
Regarding the battery pack, I am not educated on the process of soldering together Li-ion cells, so you are going to need to look at some forum posts.

The 192kv is perfect for 12S and so Is the 168kv, both are 6374 and could benifit from high Amp escs. The 245kv is smaller 6364 and will go faster. It is good for a vesc.its up to you if you want to go fast/slow.

 Calculator here: http://toddy616.blogspot.com/2013/07/electric-skateboard-calculator.html

the car esc is less flexible but simple. Buy a expensive vesc and learn the basic setup guide and you should be fine and you will have customization. As with speed, I dont know much as i havent gone over ~17mph. Buy calipers since thats the only one available. Buy one truck form TQ.
```

---
