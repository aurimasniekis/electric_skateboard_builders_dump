# Third enertion vesc failure

### Replies: 80 Views: 4991

## \#1 Posted by: kingbing Posted at: 2016-08-20T05:06:33.438Z Reads: 364

```
I am going to start of this post by addressing those who are contemplating on getting Enertion's VESCs.... DO NOT BUY THEM. 

Let me explain:

I ordered two enertion vesc back in December and got them in February. Plugged one of them to my laptop and did a motor detection, got it running and ready to plug it to my board. Finally the next day I got my board ready and connected all the components. Got the board running for  about 45 min. I was riding at a relatively low speed (around 15km/h) considering it was my first time on a Esk8. All of a sudden my bord stops aggressively and i go flying. Came back home with some bruises but nothing too serious. Messaged Onloop and posted on this forum about what happened. I got told to check for possible errors on the bldc tool and i did so. I then discovered i had a Drv chip failure. Asked onloop if i can get a refund but unfortunately he said no as it wasnt covered under their guarantee and claimed that it could of  been the users fault and not theirs. As a newbie I thought he might be right and i might of accidentally did something wrong. I naively did nothing afterwards. 

Now onto the second Vesc from December. Did the same procedure (pluged it to Bldc and did motor detection) with extra care. Plugged it to my board and lasted me for about a week. Keep in mind that that VESC well protected with no possibility of shorts happening. And again the same god damn drv failure.

NOW... what brings me to write this post. 
Even with these two vesc failure i decided to buy another two vesc from enertion as i wasnt entirely sure if these failures were caused by the manufacturer or the user. So went ahead and order two vesc in May and guess what... got them 4 months later in August. Thats fine, i dont mind waiting but every single time enertion kept pushing the shipping date... WTF. 
Anyway got them finally. Plugged one vesc to the bldc tool and couldnt get the motor to spin right. I later realized (with peoples help on this forum) that i had the wrong bldc version. So i then downgraded the bldc tool and got my vesc to work fine. Plugged it to my board and everything was fine. I decided to put some heatsinks on three of the mosfets just for precaution. Rode the board for exactly 8 days with medium use. Everything was fine until tonight when i decided to go for a night ride. Pluged everything, went outside and rode the board for a minute until i started to notice that the board was jerking. At first i thought it was my transmitter that was causing that due to signal interruption but a few seconds later the board wouldnt move even with the transmitter and receiver signal very strong. Got home, inspected everything only to see three red blinking light. At that point  i knew for sure it was an drv failure.

Now before anyone asks me about my set up for all of the VESCs, i was using 10 cells 5000mah batteries (2 turnigy nanothech), a 6374 sk3 149kv motor and a hobbyking gt2b transmitter.

Now i am not in anyway trying to bash or insult onloop as i am fully aware of his contribution in this community. His ESK8 Hardware seem to be of good quality even though i have never bought a motor mount or a pulley but see good reviews on them.
HOWEVER i am going to say that enertions customer service is the absolute worst customer service i have ever come across and their vescs are extremely bad quality. I had to wait 4 months and pay over 450$ that i will never get back on a product that fails every single time. And i dont mind if he is in his garage trying to get his company to grow but do not tell your customers that you will ship their product on date x but end up shipping it 4 months later. Now i get it that you might run into some complication along the way but you are fully aware of those complications and instead of giving a shipping date, at least give your customers a heads up by saying that they might not get the product by x date.

And people...Keep in mind that  I have never given a bad review on anything i ever bought. Its fair to say that i have been patient with enertion by not blaming them about the first two vesc failures but instead made sure that i wasnt the cause of the problem first before writing anything negative about their product.

I am sure some people who bought enertion vescs can agree with my statements.
I am trying to save people's time and money here. And i am speaking from experience.
```

---
## \#2 Posted by: Photorph Posted at: 2016-08-20T05:10:08.510Z Reads: 328

```
This does sound extremely frustrating.  I feel like you should get a refund at the very least.
```

---
## \#3 Posted by: Blasto Posted at: 2016-08-20T05:14:50.524Z Reads: 328

```
Show us your settings and setup, so you don't go through your 4th one

I can understand your frustration, went through 3 vesc in one night once... I was pissed, then i found the bad setting i had, no problems since
```

---
## \#4 Posted by: c4Lvin Posted at: 2016-08-20T05:16:03.669Z Reads: 325

```
I was really frustrated with VESCs myself and I think you have a motor short somewhere. My first VESC did the same exact thing. Replaced the DRV and got riding again but I felt sudden brakes. Read through some threads here and fiddled around with the motor phase wires and all that junk. It does not seem to do it anymore but I've since been running a new SK3 6364 190kv which is flawless. Please change out your motor for another one (still cheaper than buying any new ESCs) and repair the VESC. I'm sure you will be not have any further damaged VESCs and hopefully no more injuries. Take care.
```

---
## \#5 Posted by: kingbing Posted at: 2016-08-20T05:18:20.970Z Reads: 322

```
I will do that first thing in the morning. Its 1h17 am here and gotta wake up early tomorrow. But expect those pictures tomorrow.
```

---
## \#6 Posted by: kingbing Posted at: 2016-08-20T05:21:53.595Z Reads: 316

```
Trust me i did everything. I bought 2 motors from hobby king thinking i would do a dual setup but ended up using the first motor for the frst two vescs.
As soon as i got the other two vescs the first thing i did was change the motor to a brand new one. I would not have written this post if i wasnt sure it was the manufacturers fault. Thank you for the suggestion.
```

---
## \#7 Posted by: itsmikeholland Posted at: 2016-08-20T06:08:17.388Z Reads: 310

```
ollinboard vesc or bust. I've had 0 issues with mine, the one user error I had was fixed the day it arrived at their P.O. box and I had a tracking number that night.

edit: I should mention I run 12s 149kv single chaka vesc, though I HIGHLY recommend you get cell checkers for each of your batteries, despite whatever low-voltage monitoring the vesc claims to have. I have 3x 4s (vesc isn't specifically designed for this), one of the batteries was draining unevenly and took a cell all the way to 0, and another one down below 2 volts.
```

---
## \#8 Posted by: Pablo_702 Posted at: 2016-08-20T06:24:55.434Z Reads: 302

```
Man if i was you i would buy a vesc from @chaka and maybe send those 3 broken vesc for a proper repair, just type ollin vesc and you will see how many happy customers there is, and on top of top notch quality, fast shipping like 2 weeks instead of 4 months and by far one of the best customer service, imo ollin and diy are the 2 best esk8 suppliers, i dealt with enertion once and thats it no mo for me
```

---
## \#9 Posted by: petmakris Posted at: 2016-08-20T07:38:21.794Z Reads: 294

```
Guys I burned a couple of vesc myself but is it really a supplier issue? chaka vs onloop? vedder himself had many failures and fried drvs , so this is an open hw/sw project and it's highly possible that you would burn chaka's vesc as well 

and then you will realize how difficult it is creatr such a controller
```

---
## \#10 Posted by: dogeatgod Posted at: 2016-08-20T08:06:36.217Z Reads: 293

```
I think this is more a consumer issue.
'A product should be fit for purpose and last a reasonable amount of time'
If something purchased fails for whatever reason when used within scope of purpose sold then consumers expect a level of service from seller such as replacement or repair.
In my opinion VESC went to market too early in development - It should still be sold in BETA test phase for those willing to accept risk of failure - not as an off the shelf product. What will happen if (God forbid) a serious accident occurs when brakes fail due to overcharge or whatever - it's reasonable to believe an electronic speed controller should not fail under braking but many have - original poster crashed when VESC shut off/failed.
It does not matter how difficult something is to design or build, if sold to Joe public it should work without issue - regardless of price or profit
```

---
## \#11 Posted by: onloop Posted at: 2016-08-20T09:30:59.645Z Reads: 291

```
[quote="kingbing, post:1, topic:7956"]
I am sure some people who bought enertion vescs can agree with my statements.I am trying to save people's time and money here. And i am speaking from experience.
[/quote]

I can understand your frustration, we have all blown up vescs before. But this forum is not designed for you to complain & blame so keep it off the forum.

Just remember enertion vesc are all tested before shipping. Each one is powered up, firmware loaded & motor is spun up. So your vesc definitely was working before you got it.

We also offer 12 months instant replacement warranty on the vesc. No other vender offers that. Did you buy vesc that has the warranty? If not you can buy it now and get an instant replacement sent.

If there is a manufacturing fault. Or user error fault you are covered with our warranty. No questions asked.

We build 20 - 30 raptors each month with the same vesc and they are all working great. Rarley will there be any faulty units and if it does happen is normally our fault. We also test ride the raptors before shipping. Pure manufacturing Problems are very rare.

We also ship about 300 vesc each month at the moment. If there was some quality issue where are the other 300 complaining customers?

Is there a chance you could have done something wrong?
```

---
## \#12 Posted by: Hummie Posted at: 2016-08-20T09:33:21.084Z Reads: 286

```
Is the vesc inherently prone to failure though?  Who's lasted the longest?  i think it could be because of the extreme conditions of a skateboard.  If it's made robustly its solid state electronics and should last and last right?  Once I had one on FOC I was hooked so all I can do is hope for the best and so far I've been pleased.  I do still have good potting resin and think potting it is likely much safer concidering the vibrations and stuff
```

---
## \#13 Posted by: onloop Posted at: 2016-08-20T09:49:21.564Z Reads: 288

```
[quote="dogeatgod, post:10, topic:7956"]
my opinion VESC went to market too early in development - It should still be sold in BETA test phase for those willing to accept risk of failure
[/quote]

I'll admit. It took us a long time & lots of trial an error to get an optimised drive train. We also sent motors to the vesc designer for testing and feedback. We tried many settings to get a well tuned system.....   we sell motors and vesc & batteries.... they are all designed to work together reliably..  if people buy other stuff they need to expect some failures... 

VESC work very reliably when used correctly....  people who connect random motors and batteries and have unknown and untested configurations with little preavious knowledge of vesc and how to configure it tend to have the most problems.... this is why we offer the best warranty in the market. Instant replacement for any faulty vesc...

People should consider buying the vesc with the best warranty if they are experimenting with untested motor and battery configurations.
```

---
## \#14 Posted by: Svenska Posted at: 2016-08-20T12:11:45.319Z Reads: 274

```
That sounds a lot like the multiplication bug I found.
Make sure to only use firmware that is form the source directly as well as only the BLDC tool from the source.
```

---
## \#15 Posted by: dogeatgod Posted at: 2016-08-20T12:58:20.350Z Reads: 276

```
[quote="onloop, post:13, topic:7956"]
I'll admit. It took us a long time & lots of trial an error to get an optimised drive train. We also sent motors to the vesc designer for testing and feedback. We tried many settings to get a well tuned system.....   we sell motors and vesc & batteries.... they are all designed to work together reliably..  if people buy other stuff they need to expect some failures...
[/quote]



Exactly - when sold as part of a package designed, tested, optimised and set up to work it will perform - You have done the ground work and are confident to supply.

Average Joe consumer has not gone through the trial and error process for their set up and can't become a VESC expert overnight - they've purchased an Electronic Speed Controller and will expect it to work. In time it is likely that the VESC will become a simple plug and play electronic item but it's not at that stage yet and users need be made aware of risk at time of purchase.
```

---
## \#16 Posted by: onloop Posted at: 2016-08-20T13:27:38.795Z Reads: 268

```
[quote="dogeatgod, post:15, topic:7956"]
users need be made aware of risk at time of purchase
[/quote]

If people don't read about it and buy it anyway it's not in our controll... we have tried hard to educate but it's ultimately the buyer decision. 

We also pre install settings for our motors to make it easy...

I have personally written nearly every vesc article on this forum. I also encourage my customers to write about there problems openly on the forums as I know it helps others diagnose issues..


So Why no other VESC vendors writing help articles? Why doesn't chacka contribute his immense vesc knowledge to write articles to help others? He has openly said he only helps his customers in private? Seems a bit unfair... I have openly shared all my vesc knowledge (vesc faq) and made available to all users..

http://www.electric-skateboard.builders/search?context=topic&context_id=7956&q=Vesc%20faq&skip_context=true

When drivers crash their cars do they blame the manufacturer?
```

---
## \#17 Posted by: dogeatgod Posted at: 2016-08-20T13:51:07.029Z Reads: 256

```
[quote="onloop, post:16, topic:7956"]
If people don't read about it and buy it anyway it's not in our controll... we have tried hard to educate but it's ultimately the buyer decision.
[/quote]

I agree with you - it is the buyers decision - if you underline this at time of purchasing a $99 VESC in BIG HIGHLIGHTED WORDS that buyer accepts risk of possible failures when used with other set ups or changes to firmware/settings (not hidden in terms and conditions of sale blerb) then you can simply quote this when problems arise and start the help/solution conversation without a buyers expectation of immediate satisfaction and a free VESC,

The fact that there is plenty of information available on a forum does not mean that people will read/understand it.

Many 1st posts are people venting frustration following a problem that has not been resolved the way they wish - that's human nature. A standard reply to these would then be possible "purchaser accepted the risk and we are trying to help"

[quote="onloop, post:16, topic:7956"]
When drivers crash their cars do they blame the manufacturer?
[/quote]

If they can yes
```

---
## \#18 Posted by: devin Posted at: 2016-08-20T13:58:51.000Z Reads: 243

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#19 Posted by: onloop Posted at: 2016-08-20T14:10:20.821Z Reads: 242

```

This article I wrote talks about how to change the motor current...

I am not sure Measuring with a watt meter helps. I suggest trial an error approach... slowly change the setting until they feel best. Normally default settings are 95% good. it's just the remaining 5% that can perfect your ride.

http://www.electric-skateboard.builders/t/vesc-faq-regen-braking-configuration-bldc-tool-brake-force/353
```

---
## \#20 Posted by: devin Posted at: 2016-08-20T14:12:21.958Z Reads: 242

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#21 Posted by: onloop Posted at: 2016-08-20T14:14:16.363Z Reads: 227

```
It depends on the motors and the drive train setup...

My settings are probably in that screen grab..
```

---
## \#23 Posted by: onloop Posted at: 2016-08-20T14:27:17.721Z Reads: 225

```
[quote="dogeatgod, post:17, topic:7956"]
$99 VESC in BIG HIGHLIGHTED WORDS that buyer accepts risk of possible failures when used with other set ups or changes to firmware/settings (not hidden in terms and conditions of sale blerb) then you can simply quote this when problems arise and start the help/solution conversation without a buyers expectation of immediate satisfaction and a free VESC,
[/quote]

Good advice.... sometimes I forget to spell shit out like that...

I assumed it was obvious... my mistake.
```

---
## \#25 Posted by: onloop Posted at: 2016-08-20T14:38:37.358Z Reads: 217

```
I flagged the post because it's off topic.... create a new post with your thought experiment and if I have time I'll answer the questions.
```

---
## \#26 Posted by: devin Posted at: 2016-08-20T14:39:38.573Z Reads: 217

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#27 Posted by: JLabs Posted at: 2016-08-20T15:55:22.837Z Reads: 212

```
@onloop I was just was on your website, why is it cheaper to buy a standard vesc and then the warranty, compared to the vesc with warranty?
```

---
## \#28 Posted by: kingbing Posted at: 2016-08-20T16:02:27.205Z Reads: 221

```
Look people, I have had 3 VESC from enertion. When the first two failed i did not blame enertion one bit. I calmly tried to figure out what the problem was and who it came from. But after the third vesc failure, I do not see where i could be at fault especially that i had more than half a year to research the settings and to read as much as i could on this forum. 
Now the reason i believe enertion does not write in HIGHLIGHTED WORDS that buyer accepts the risk of possible failure is because it is very bad for business... that is common sense.

[quote="onloop, post:13, topic:7956"]
VESC work very reliably when used correctly....  people who connect random motors and batteries and have unknown and untested configurations with little previous knowledge of vesc and how to configure it tend to have the most problems
[/quote]

My set up was as followed: SK3 6374 149 KV, 16/36 gearing ratio with kegel wheels, and 2x5 cells in series for a total of 5000mah 10 cell, and finally a gt2b from hobby king. These are NOT random motors and batteries... these parts are the most used in the esk8 diy community and are mostly always connected to vescs.

[quote="onloop, post:13, topic:7956"]
this is why we offer the best warranty in the market
[/quote]

Sorry i am not going to spend almost the cost of another vesc just to get mine replaced especially when i am certain it is going to fail me again. 

[quote="onloop, post:11, topic:7956"]
But this forum is not designed for you to complain & blame so keep it off the forum.
[/quote]

The purpose of this post was not mainly to complain but to warn anyone of possible enertion vesc failure. And as long as this(post) is intended to help (and it really much is) i have the right to post on this forum.[quote="onloop, post:11, topic:7956"]
Just remember enertion vesc are all tested before shipping. Each one is powered up, firmware loaded & motor is spun up.
[/quote]

Do you really call that a test? You spin the motor under no load for a couple of seconds but when it comes to the raptors you test them with actual load... okayy...

[quote="onloop, post:11, topic:7956"]
We also ship about 300 vesc each month at the moment. If there was some quality issue where are the other 300 complaining customers?
[/quote]

They are not complaining because, like i thought when my first 2 vesc failed, they think:
1. its their fault but really in most cases its not
2. they buy your vescs and do not use them immediately
3. Or they do not even bother to ask or post about their vesc failure

[quote="Hummie, post:12, topic:7956"]
Once I had one on FOC I was hooked so all I can do is hope for the best
[/quote]

Trust me you do not want HOPE for the best especially when you life is literally at risk. I dont want to scare anyone but that is the truth.

And one last time i am not trying to pick a fight. I am just giving true facts and my honest opinions.
This will be my last reply and if you are aware of enertion vesc failure and still want to purchase them PLEASE DO SO.
I will post pictures of my set up and all three VESCs for anyone who is still doubting me. And people please do not fight here. This forum's purpose is to help one another. @onloop do not get me wrong you have immensely contributed to this amazing community and i dont want to take that away from you in any way. But when i see a problem somewhere or something i do not agree with i have to speak up.  
Anyway guys keep this community alive and i hope the best for everyone.
Cheers
```

---
## \#29 Posted by: devin Posted at: 2016-08-20T16:07:24.305Z Reads: 206

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#30 Posted by: ra.rend Posted at: 2016-08-20T16:19:49.389Z Reads: 201

```
This might have caused the problem. http://www.electric-skateboard.builders/t/psa-remember-to-reset-your-max-current-ramp-step-when-programming-your-vesc/6262?u=ra.rend
```

---
## \#31 Posted by: Svenska Posted at: 2016-08-20T16:21:10.928Z Reads: 203

```
@kingbing

Could you please do a quick test with your blown VESC?
Goes like this: 
Hook the VESC up to your computer. Start BLDCTool, connect. Then go to the advanced tab and multiple times !without changing any value! Read your settings, then write them again. Do it 5 times for good measure.
Heres the important part:
There is a value called "current ramp per hertz" (not sure on the precise name) watch what happens to this value. 
Does it magically change? If yes, that is your problem and the only reason you blew up VESC. There was a bug in the firmware that caused this.
If you are interested I can explain what that value does and where the bug came from.
```

---
## \#32 Posted by: Hummie Posted at: 2016-08-20T16:27:48.685Z Reads: 198

```
With this forum there's so much info available but tragically it's missing much on the one part most unknow. This last info is a gem which 99% of us don't know.  Wish there was a a decent tutorial on everything.  Vedder's stuff is a start but how bout someone else who knows all that and more can do a guide/tutorial.  If I were you Jason I'd even pay someone a couple hundred or a board to do it and then you can at least tell people where to go and people won't be as able to complain..and surely a lot less will blow
```

---
## \#33 Posted by: Svenska Posted at: 2016-08-20T16:33:09.632Z Reads: 199

```
@Hummie are you telling me that bug is not known here?
If so, can you create a sticky to warn people to not use any firmware before the date me and my buddys pull request with the fix got accepted into master?
```

---
## \#34 Posted by: flatsp0t Posted at: 2016-08-20T16:35:34.411Z Reads: 195

```
It was known, There even was a e-mail warning about it.
```

---
## \#35 Posted by: devin Posted at: 2016-08-20T16:35:42.579Z Reads: 191

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#36 Posted by: flatsp0t Posted at: 2016-08-20T16:38:26.599Z Reads: 197

```
Seems to be already fixed:
https://github.com/vedderb/bldc/commit/fbfc442b432e88825d1c1999cf726256303c81aa
```

---
## \#37 Posted by: Svenska Posted at: 2016-08-20T16:40:28.995Z Reads: 194

```
Yep, it is fixed. That is the fix my friend submitted...

@devin No, there was a bug in the firmware. Look at the link above 10^5 instead of 10^6
```

---
## \#38 Posted by: Hummie Posted at: 2016-08-20T16:43:49.240Z Reads: 193

```
I'd read something about it in passing but next time I get a vesc I won't know where to look.  A dedicated thread that explained as much as is known.  That's what I'd like at least and think others would too
```

---
## \#39 Posted by: devin Posted at: 2016-08-20T16:46:21.446Z Reads: 192

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#40 Posted by: Svenska Posted at: 2016-08-20T16:50:13.715Z Reads: 202

```
Just keep up with the source on Git as well as the VESC forum and only compile your firmware from this source.
If there is a bug reported change to the latest version.
Thats at least how I do it.

On a more involved level one could setup a server that checks for changes and auto compiles the latest firmware and offers it for download?
```

---
## \#41 Posted by: kingbing Posted at: 2016-08-20T16:53:11.615Z Reads: 189

```
HI Svenska, 
I tried that and the value of "Max curent ramp step (at 1kHz)" does not change. Dis it six times for good measure but the value stays the same.
```

---
## \#42 Posted by: devin Posted at: 2016-08-20T16:56:09.324Z Reads: 197

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#43 Posted by: kingbing Posted at: 2016-08-20T16:59:58.585Z Reads: 199

```
Here are my setting on the BLDC tool:
<img src="/uploads/db1493/original/2X/2/2b39576735210c8e03075099fa51354cfde63886.png" width="690" height="388">
```

---
## \#44 Posted by: kingbing Posted at: 2016-08-20T17:19:02.862Z Reads: 204

```
And as promised here are all the pictures:

<img src="/uploads/db1493/original/2X/e/ef404d504451949c5394a95b339734097505908b.jpg" width="666" height="500">
From left to right: The first two vescs are from february and the last two are from august. The third one failed yesterday and the last one has not been used yet.

<img src="/uploads/db1493/original/2X/d/d63f8700842a7988f626dacb789aa38e0014f7ea.jpg" width="562" height="500">
Same image from the other side.

<img src="/uploads/db1493/original/2X/0/0d3577efb9205bd07039db23fbb2d6758c1a9edc.jpg" width="240" height="500"><img src="/uploads/db1493/original/2X/5/5d91577c2e8ab9b76b0664652525b19449080e2e.jpg" width="196" height="500"><img src="/uploads/db1493/original/2X/a/a09a23f26e80e68f080a0faecafeaa238e55a4b2.jpg" width="145" height="500"><img src="/uploads/db1493/original/2X/e/e26cbd9d936385c639d5774d7e1d60cfaa8bc6fb.jpg" width="148" height="500">
These are close ups of all four of them.

<img src="/uploads/db1493/original/2X/f/f335330ccf9ec48f42d68b277380429feeeeed5b.jpg" width="481" height="500">
Both motors. The one attached to the axle is the newest one.only a week of use.

<img src="/uploads/db1493/original/2X/a/a7b20bea946444a0cc2dff1aa0dc2d32e6d6dc47.jpg" width="690" height="394">
As you can see i protected my batteries to the max.

<img src="/uploads/db1493/original/2X/3/3ec1eb51cc54740fa9cbc404c3694db2d62a75cd.jpg" width="649" height="500"><img src="/uploads/db1493/original/2X/f/f71c21ca75bb14a35e6c303448d439a99d9d44d5.jpg" width="375" height="500">
And this the hard plastic case i use for all my vescs> It protects them while still allowing air to go through it.
```

---
## \#45 Posted by: Hummie Posted at: 2016-08-20T17:45:30.461Z Reads: 191

```
Maybe add padding?
```

---
## \#46 Posted by: kingbing Posted at: 2016-08-20T17:52:56.518Z Reads: 192

```
There was bubble wrap on the bottom of the inside.
```

---
## \#47 Posted by: RogerD Posted at: 2016-08-20T17:57:17.328Z Reads: 194

```
Each time I read these threads I remember why I dabbled in them and then reverted to car ESCS. They are just too damn unreliable. Lots and lots of money, hassle, PC settings, firmware confusions for what? The ablity to start your board without kicking off. I just can't see it's worth it unless you are a high voltage user left with few other choices.
```

---
## \#48 Posted by: kingbing Posted at: 2016-08-20T18:11:22.992Z Reads: 193

```
What ESC do you use and what is your configuration. I might have to make the switch like you did because i am tired of all these issue popping out of nowhere.
```

---
## \#49 Posted by: Michaelinvegas Posted at: 2016-08-20T18:15:03.848Z Reads: 193

```
Just 12s @torqueboards esc
```

---
## \#50 Posted by: c4Lvin Posted at: 2016-08-20T18:24:13.480Z Reads: 191

```
or @barajabali 12S at a great price.
```

---
## \#51 Posted by: RogerD Posted at: 2016-08-20T18:29:44.977Z Reads: 190

```
EZRun pro 150amp car esc, 6S (I've kept clear of high voltage due to high battery and esc costs)
```

---
## \#52 Posted by: kingbing Posted at: 2016-08-20T18:34:50.262Z Reads: 191

```
What motor do you use and does it have enough torque with 6s? That was my main concern when i thought of switching to a low voltage set up.
```

---
## \#53 Posted by: c4Lvin Posted at: 2016-08-20T18:44:44.075Z Reads: 186

```
Personally started off with 10S, can't go backwards.
```

---
## \#54 Posted by: kingbing Posted at: 2016-08-20T18:48:15.240Z Reads: 185

```
what is his VESC called? Will look into it.
```

---
## \#55 Posted by: c4Lvin Posted at: 2016-08-20T18:55:05.557Z Reads: 185

```
It's not a VESC. It's a airplane or boat high voltage speed control with skateboard firmware loaded onto it. You need only a program card to do settings. Simple and robust.
```

---
## \#56 Posted by: kingbing Posted at: 2016-08-20T18:58:10.917Z Reads: 186

```
HAHAHA Sorry i meant what ESC. I have been typing the word vesc so much that its automatic now. And where can i get one.
```

---
## \#57 Posted by: Jinra Posted at: 2016-08-20T19:21:07.596Z Reads: 184

```
diy-electric-skateboard-kits-parts/torqueboards-12s-120a-car-esc-opto-hv/
```

---
## \#58 Posted by: onloop Posted at: 2016-08-20T23:28:12.474Z Reads: 191

```
[quote="kingbing, post:28, topic:7956"]
Sorry i am not going to spend almost the cost of another vesc just to get mine replaced
[/quote]

Lol... And this is the problem folks.... you want me to spend the money to fix it? But your not willing too.

Everyone wants the cheapest stuff, no one takes any responsibility for faults that occur and everyone thinks its perfectly acceptable for vendors to take a loss to fix problems.... 

I have sent r-spec motors & batteries to vedder for testing & I program the vesc to work with our products... if you use other stuff and change the settings expect a fault.

I have a warranty. Buy it. Problem solved....
```

---
## \#59 Posted by: kingbing Posted at: 2016-08-20T23:45:18.542Z Reads: 191

```
[quote="kingbing, post:28, topic:7956"]
Sorry i am not going to spend almost the cost of another vesc just to get mine replaced especially when i am certain it is going to fail me again.
[/quote]

Lol.. You didnt quote the whole sentence. Here is my sentence: 
Sorry i am not going to spend almost the cost of another vesc just to get mine replaced especially when i am certain it is going to fail me again.
```

---
## \#60 Posted by: whitepony Posted at: 2016-08-21T08:17:21.331Z Reads: 191

```
sounds weird that you killed 3 vescs in a row on the exact same setup - I would start to think there is something funky with the rest of your gear. maybe very long/thin battery wires? possibility for motor wires to short under extreme circumstances? connectors coming loose and shorting? excessive motor current settings, maybe a very high kv motor that pulls a lot of current for quite a long time?

in which moments did the vescs usually die?
```

---
## \#61 Posted by: Namasaki Posted at: 2016-08-21T09:28:29.677Z Reads: 192

```
Maybe this could be your problem?

http://www.electric-skateboard.builders/t/vesc-faq-negative-squared-cross-mark-warning-negative-squared-cross-mark-risk-of-short/6805
```

---
## \#62 Posted by: Nordle Posted at: 2016-08-21T09:48:57.384Z Reads: 189

```
No :older_man:
```

---
## \#63 Posted by: RogerD Posted at: 2016-08-21T09:55:06.773Z Reads: 199

```
Turnigy SK 6354 motor (245 Kv) - I can go up hills that cyclists get off their bikes to go up, and I'm 90Kg,
```

---
## \#64 Posted by: RogerD Posted at: 2016-08-21T10:07:04.155Z Reads: 201

```
Not so weird in my experience. My mate (GodeatDog - on here) is on his third Esc I believe. I set the 1st one up for him (and electronics is my thing). Worked ok until a firmware update and then dead when performing the motor sensing test. Second one blew the DRV chip after a month or two for no apparent reason. He's on his third now I think.

All wires correct gauge, good soldering, nowhere near over current. 10S, SK 6 series motor. Cooling fan on ESC. His would have high temp cut out kick in without a fan. I've the distinct impression the VESC in it's current form is not up to hauling grown adults around. It's just too delicate. At the very least , it should be robust. I'm on year three with the same car esc I started with. Same motor, same weight, same board, same wiring, but 6s instead of 10.
```

---
## \#65 Posted by: Namasaki Posted at: 2016-08-21T17:41:56.816Z Reads: 195

```
[quote="RogerD, post:64, topic:7956"]
Worked ok until a firmware update and then dead when performing the motor sensing test.
[/quote]
There was a bug in the first edition of the latest firmware that caused the current ramp setting to multiply during write and was blowing DRV chips.
That bug was just recently fixed.
```

---
## \#66 Posted by: chuttney1 Posted at: 2016-08-21T18:31:20.554Z Reads: 195

```
TL;DR  Summary from reading
kingbing buys 3 VESC. Each one fails. Bug found in firmware causing current ramp setting to blow DRV chips, fixed.


Not to high jack thread. From my knowledge and following the VESC's movements. The open source VESC is not a plug and play device yet as of today as one user mentioned in comments above. Partly requires some knowledge. It's is still being improve by Vedder. Next iteration changes board design to separate layout into a high and low power sides with no DRV blowouts. This is an increase in reliability of device. Currently no ETA on when next iteration will be release.
```

---
## \#67 Posted by: kingbing Posted at: 2016-08-21T20:09:00.317Z Reads: 190

```
The battery wires are the original wires, i always duck-tape the motor (on top of teh heat shrink) and esc connectors as much as i can and my motor has the lowest kv for a sk3 which is 149KV. The VESCs always fail me during the ride, that being said I always connect the battery and the VESC correctly and if there was a short I wouldnt be able to ride for a bit before the VESC failure.
```

---
## \#68 Posted by: kingbing Posted at: 2016-08-21T20:14:27.611Z Reads: 189

```
I havent protected the positive wire coming from the capacitor board for the first two VESCs but after a close inspection, the wires are not pierced and there arent any burned marks. However for extra protection I trimmed the pins with nail clippers on the third and fourth VESC, added a dab of hot glue and even with that i had a failure.
```

---
## \#69 Posted by: Namasaki Posted at: 2016-08-21T20:44:47.007Z Reads: 187

```
Ok, gotta be something else then
```

---
## \#70 Posted by: Skitzor Posted at: 2016-08-23T19:40:15.864Z Reads: 176

```
@Jinra has made a topic for that parameter error firmware bug.

Is it actually dangerous ? I don't really know. When I saw the topic and checked mine, both VESC's had these on 50 since I've played a lot with my settings to try and fix my battery cutoffs.
It could be related to the cutoffs though...
```

---
## \#71 Posted by: Jinra Posted at: 2016-08-23T19:46:42.116Z Reads: 172

```
if you flash newest firmware it fixes the bug. Not sure how dangerous it is but I've seen a couple blown drvs with high max current ramp steps. I think it dictates how to ramp up current when throttling.
```

---
## \#72 Posted by: Lizardking0069 Posted at: 2016-08-23T19:49:19.488Z Reads: 172

```
Whats the latest version?
```

---
## \#73 Posted by: Jinra Posted at: 2016-08-23T19:50:26.952Z Reads: 172

```
still 2.18 but with bug fixes. get it at VESC.net.au
```

---
## \#74 Posted by: sl33py Posted at: 2016-08-23T19:58:25.670Z Reads: 172

```
I have my original hw4.7 VESC on my GF's Vanguard build - going strong now since July 2015.

Still running fw 1.13 (if it ain't broke...) - and BLDC not FOC, on 6 or 8s.
```

---
## \#75 Posted by: Hummie Posted at: 2016-08-24T02:10:10.080Z Reads: 174

```
do I hear longer? going once. going twice....  but does she really ride much.
```

---
## \#76 Posted by: sl33py Posted at: 2016-08-24T04:20:16.602Z Reads: 178

```
She rides when i ride, and i've ridden it when she's not able to.  If i go out w/ friends or visiting guests i ride hers and they ride my Marbel.  (friendly mode for beginners is nice)

Not a huge # of miles, but gets ridden pretty regularly still.
```

---
## \#77 Posted by: Svenska Posted at: 2016-08-24T06:07:10.030Z Reads: 181

```
I'm very surprised that yours are still alive! That parameter is responsible to limit the power that hits the components. Aka, we ramp it up soft and don't hit it in the face with a sledgehammer.
If I recall right it is increase in amp per hertz. 50A is huge!
```

---
## \#78 Posted by: Skitzor Posted at: 2016-08-24T14:26:51.019Z Reads: 192

```
I agree, but that makes me wonder if it was just a visual bug, not actually being set until you hit the apply button in the advanced tab. (model-view-controller programming logic)
```

---
## \#79 Posted by: Jebe Posted at: 2016-10-01T09:47:04.668Z Reads: 117

```
2 enertion vescs - no issues. BLDC motor detect, slight adjustment on brakes. FTR
```

---
## \#80 Posted by: Ackmaniac Posted at: 2016-10-01T10:35:37.260Z Reads: 113

```
I checked your settings and your max battery setting is very high. Try it with 25 at the beginning. When you test the motor on the bench then use the current to spin the motor and not the rpm. Also your battery cutoff start and end is too low. When you have a 10s battery then set it at least to 32v start and 30v end. 
Maybe the vesc gets killed when those numbers are too low because it can't shut down the vesc when you shut off the power (caps still have some power left) . But that is a very wild guess. 

And please post a Screenshot of the motor advanced tab and the application tabs.
```

---
## \#81 Posted by: spottyjohn Posted at: 2016-10-02T15:21:07.513Z Reads: 97

```
I'd say that probably 2 items having the same failure could conceivably be a coincidence but 3? No, something's either wrong with the set up or something's shorting somewhere.
Imo 😀
```

---
## \#82 Posted by: SORRENTINO Posted at: 2016-10-02T17:36:12.603Z Reads: 92

```
Wire length to the esc from battery has also been a issue known to blow drvs. You want it short as possible. The longer it is the more it is prone to voltage spikes that blow the drv.
http://www.rcgroups.com/forums/showthread.php?t=952523
```

---
