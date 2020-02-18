# Having an issue with my TB vesc

### Replies: 71 Views: 1687

## \#1 Posted by: coleg411 Posted at: 2017-12-11T03:45:57.119Z Reads: 186

```
warning to those on a low budget, do not buy the torque boards VESC. Although the price point seems attractive, they do not last.
```

---
## \#2 Posted by: GrecoMan Posted at: 2017-12-11T03:48:14.731Z Reads: 187

```
this is wildly untrue. i guarantee you it blew because of user error. I will stand behind the TB vescs until I blow one from something other than user error.

@moderators, time to delete this thread, I could just do it if I was a mod 😉
```

---
## \#3 Posted by: coleg411 Posted at: 2017-12-11T03:49:19.225Z Reads: 182

```
I really am not sure what I did wrong then, I followed all their setups perfectly
```

---
## \#4 Posted by: kyletrainy Posted at: 2017-12-11T03:50:57.557Z Reads: 181

```
What were your settings for the vesc at?
```

---
## \#5 Posted by: lasplaner Posted at: 2017-12-11T03:51:09.080Z Reads: 178

```
They're good for what they're used for; lower voltage applications at lower current settings.

While it's true that they aren't the highest quality VESC out there, they are definetly worth the low price tag. I run 6S FOC Hybrid mode, and never have I burned out the VESC/DRV chip.

You just need to find what VESC suits you best, if you're going for a 12S high amperage FOC Hybrid setup, then naturally the TB VESC wouldn't be your best shot. Maybe a FOCBOX, or even VESC 6 is more suitable. Other than that, TB VESC is great for most ESK8 applications, espeically considering its low price point.
```

---
## \#6 Posted by: willpark16 Posted at: 2017-12-11T03:51:48.871Z Reads: 169

```
Tb vescs aren't known for being the best vesc, if you look at where most of the issues are coming from vesc wise most are usually a tb vesc
```

---
## \#7 Posted by: lasplaner Posted at: 2017-12-11T03:52:11.724Z Reads: 166

```
Could you enter "faults" into the BLDC Tool Terminal?
```

---
## \#8 Posted by: ARetardedPillow Posted at: 2017-12-11T03:52:25.960Z Reads: 164

```
What were you vesc settings? And did you tape your phase wires?
Did you short your phase wires?
```

---
## \#9 Posted by: GrecoMan Posted at: 2017-12-11T03:52:35.901Z Reads: 161

```
i am fully aware that they are not the best, imo @chaka’s vescs are the best. but they do not just blow out of nowhere.
```

---
## \#10 Posted by: coleg411 Posted at: 2017-12-11T03:53:12.948Z Reads: 160

```
<img src="/uploads/db1493/original/3X/3/a/3a0e04e21912f0bc33417d07ce291a099606ef41.png" width="690" height="389"> these are my settings
```

---
## \#11 Posted by: ARetardedPillow Posted at: 2017-12-11T03:53:38.040Z Reads: 156

```
Ive fried over 6 tb vescs lol. They sure arent the best
```

---
## \#12 Posted by: willpark16 Posted at: 2017-12-11T03:53:54.012Z Reads: 153

```
I understand your issue as a new builder many have been in a similar predicament, but change the post to addressing what could. Have gone wrong because we don't allow bashing on the forum. Many of his products have had issues and his customer service is not the best yet it is possible that you may have made a mistake or you might be correct and it was just a bad vesc either way just keep it civil
```

---
## \#13 Posted by: coleg411 Posted at: 2017-12-11T03:54:05.844Z Reads: 150

```
yeah I heat shrunk them
```

---
## \#14 Posted by: coleg411 Posted at: 2017-12-11T03:55:23.296Z Reads: 147

```
changed the name, sorry for seeming aggressive. Is this name better?
```

---
## \#15 Posted by: coleg411 Posted at: 2017-12-11T03:56:04.072Z Reads: 145

```
I did, ended up with a DRV error on both
```

---
## \#16 Posted by: willpark16 Posted at: 2017-12-11T03:56:19.016Z Reads: 146

```
Excellent bro shoot us some photos of your settings and tell us how u set it up
```

---
## \#17 Posted by: lasplaner Posted at: 2017-12-11T03:57:57.831Z Reads: 145

```
Is this instantaneous, after motor detection, assuming you did the motor detection correctly, or did it spaz out before throwing the error? Was this on bench or in a real test scenario?
```

---
## \#18 Posted by: coleg411 Posted at: 2017-12-11T03:59:32.287Z Reads: 150

```
<img src="/uploads/db1493/original/3X/3/a/3a0e04e21912f0bc33417d07ce291a099606ef41.png" width="690" height="389"> I was using a 12s LIFEPo4 battery, (10s equivillant). Erpm was limited to 60k, I have very reasonable amps setting too
```

---
## \#19 Posted by: willpark16 Posted at: 2017-12-11T04:00:56.820Z Reads: 143

```
Motor kv? Huh
```

---
## \#20 Posted by: coleg411 Posted at: 2017-12-11T04:01:04.688Z Reads: 143

```
Yeah the second one died after about two-three days of use, I was moving along uphill (not steep just a slight grade) when the motor cut out. The pushed home and got yet another drv error.
```

---
## \#21 Posted by: coleg411 Posted at: 2017-12-11T04:01:23.037Z Reads: 139

```
245kv sk3 motor, however I was not going extremely fast and had my erpm limited
```

---
## \#22 Posted by: lasplaner Posted at: 2017-12-11T04:03:42.824Z Reads: 140

```
What about the first one? Could you show us the BLDC Motor Config as well as the App Config?
```

---
## \#23 Posted by: mmaner Posted at: 2017-12-11T04:05:45.499Z Reads: 140

```
[quote="willpark16, post:6, topic:40642, full:true"]
Tb vescs aren't known for being the best vesc, if you look at where most of the issues are coming from vesc wise most are usually a tb vesc
[/quote]

It's likely that you see more TB VESC issues because they sell a ton of VESC's. I've got 4 running right now, 2 of them for well over a year. The only one I ever had an issue with was because of foc and @torqueboards  replaced it. 

Just a numbers game. You sell 10,000 and you see a larger number of issues not a larger percentage.
```

---
## \#24 Posted by: coleg411 Posted at: 2017-12-11T04:06:18.437Z Reads: 133

```
I do not have my board on me right now, but I will update you asap with those settings. The first one had the same settings and blew after only one day of testing at low speeds.
```

---
## \#25 Posted by: willpark16 Posted at: 2017-12-11T04:08:43.860Z Reads: 129

```
It's not just his products but also customer service, I believe he picks and chooses members he wants to take care of but that's just my opinion I can only speak to the reoccurring amount of people complaining about his products
```

---
## \#26 Posted by: willpark16 Posted at: 2017-12-11T04:09:34.907Z Reads: 122

```
I have to look this up but I think that a higher kv can still lead to more problems even when limited
```

---
## \#27 Posted by: GrecoMan Posted at: 2017-12-11T04:09:50.326Z Reads: 121

```
i do have to agree with you there...

I emailed his customer support back in AUGUST about changing my order, got a reply at the end of NOVEMBER...
```

---
## \#28 Posted by: coleg411 Posted at: 2017-12-11T04:10:36.940Z Reads: 122

```
Ok, are there better quality vesc that limit the erpm more reliably?
```

---
## \#29 Posted by: willpark16 Posted at: 2017-12-11T04:13:21.689Z Reads: 118

```
I can say the focbox handles heat very well but the warranty by @chaka is unparalleled
```

---
## \#30 Posted by: willpark16 Posted at: 2017-12-11T04:14:51.097Z Reads: 122

```
Exactly I just personally think his service is terrible and if the service isn't good then why would I buy the product
```

---
## \#31 Posted by: ARetardedPillow Posted at: 2017-12-11T04:16:58.549Z Reads: 121

```
@chaka 's vesc for sure, I had tb vescs, focboxes, and the only one thats standing and usable right now is the ollin vesc, literally bulletproof
```

---
## \#32 Posted by: ThermalM16 Posted at: 2017-12-11T04:42:32.324Z Reads: 119

```
I can take a look at your VESC and find out why it't not working. I'm actually about to launch my repair service at https://theboardtech.com/
```

---
## \#33 Posted by: Eboosted Posted at: 2017-12-11T05:25:46.012Z Reads: 106

```
@coleg411

User error Nr. 1: You were running 245kv on 12s Lifepo4 it's 43.2V it's more than a 10s equivalent which is 42V.

User error Nr. 2: You chose to use 245kv motor, with 43.2V you will have 65359erpm, the vesc might limit the motor speed but only during acceleration, if you were going downhill it could fry. 

I've been runing TB vesc on my 10S vanguard for more than a year with 190kv motors and still working perfect. 

You shouldn't beware people about Torqueboards but beware people to avoid these mistakes, that'll be fair
```

---
## \#34 Posted by: DEEIF Posted at: 2017-12-11T06:24:05.132Z Reads: 107

```
Lol I’m like the god of 
They reply to my emails within 12 hours for me
I always on the live chat get a technician who helps build the stuff 
And they upgraded my battery from 12s2p to 12s4p as a surprise upgrade for free
```

---
## \#35 Posted by: PXSS Posted at: 2017-12-11T11:31:50.145Z Reads: 108

```
[quote="Eboosted, post:33, topic:40642"]
User error Nr. 1: You were running 245kv on 12s Lifepo4 it's 43.2V it's more than a 10s equivalent which is 42V.
[/quote]

Batteries sag. Realistically, even in lab conditions, he will never see that voltage under power, let alone full throttle. Unless he's spinning no load conditions. 

[quote="Eboosted, post:33, topic:40642"]
User error Nr. 2: You chose to use 245kv motor, with 43.2V you will have 65359erpm, the vesc might limit the motor speed but only during acceleration, if you were going downhill it could fry.
[/quote]

Negative ghost rider, look at his settings. He enabled the negative torque if erpm limit is reached. This would mean that his board brakes as he reaches that speed. It could induce a lot of heat issues but not what you described
```

---
## \#36 Posted by: Kug3lis Posted at: 2017-12-11T11:45:36.108Z Reads: 99

```
Still its too high kV rating for the ESC, not because of settings but because of magnetic specs inside motor
```

---
## \#37 Posted by: coleg411 Posted at: 2017-12-12T05:17:08.932Z Reads: 94

```
So my question is, If I buy a high quality vesc from ollin and limit the erpm to 50-60k, will that be enough to prevent blowing one of his VESC as well? Im not on an unlimited budget and would prefer not to have to replace my motor,
```

---
## \#38 Posted by: coleg411 Posted at: 2017-12-12T05:18:03.168Z Reads: 95

```
Even the focbox died?
```

---
## \#39 Posted by: ARetardedPillow Posted at: 2017-12-12T05:20:09.924Z Reads: 95

```
Yep, I had both ollin and focbox in a parallel connector, and there was a cold joint where the batteries are connected and killed my focbox completely, no blown drv but the entire vesc.

Ollinvesc is still going strong though, using it as my daily commute
```

---
## \#40 Posted by: coleg411 Posted at: 2017-12-12T05:25:39.379Z Reads: 93

```
I was thinking of running a 10s on a 245kv motor with an ollin vesc. based on your experience, do things like the erpm limit work well?
```

---
## \#41 Posted by: Blasto Posted at: 2017-12-12T05:33:01.378Z Reads: 91

```
[quote="ARetardedPillow, post:39, topic:40642"]
there was a cold joint where the batteries are connected and killed my focbox completely
[/quote]

Your CAN transceiver blew, remove U401 and-or replace it
```

---
## \#42 Posted by: ARetardedPillow Posted at: 2017-12-12T06:05:08.363Z Reads: 89

```
@scepterr has the focbox now, seems like the pcb died. Im waiting for enertion to ship out some new ones
```

---
## \#43 Posted by: scepterr Posted at: 2017-12-12T06:05:57.452Z Reads: 89

```
Lol yeah that one was a doozy, blown up fets, shunt, burned traces
```

---
## \#44 Posted by: coleg411 Posted at: 2017-12-12T06:25:34.489Z Reads: 84

```
did it come like that?
```

---
## \#45 Posted by: ARetardedPillow Posted at: 2017-12-12T06:27:42.984Z Reads: 87

```
Naw it came working perfectly, put many miles on it and then boom! Bad soldering skills
```

---
## \#46 Posted by: saul Posted at: 2017-12-12T09:55:02.749Z Reads: 83

```
[quote="GrecoMan, post:2, topic:40642"]
this is wildly untrue. i guarantee you it blew because of user error. I will stand behind the TB vescs until I blow one from something other than user error.
[/quote]

Actually The one vesc that i've had fail was from tb. and it was not user error. it was cold solder... 
still gotta fix that paper weight....
```

---
## \#47 Posted by: saul Posted at: 2017-12-12T09:56:07.091Z Reads: 83

```
[quote="coleg411, post:40, topic:40642, full:true"]
I was thinking of running a 10s on a 245kv motor with an ollin vesc. based on your experience, do things like the erpm limit work well?
[/quote]

i've done this for a bit, but 200kv is nicer on 10s. ;)
```

---
## \#48 Posted by: coleg411 Posted at: 2017-12-12T18:01:31.297Z Reads: 80

```
Did it work?
```

---
## \#49 Posted by: saul Posted at: 2017-12-13T00:04:44.599Z Reads: 77

```
yes ti works, but i never went full speed with that setup. the top end is where the problems would happen...
either way its not needed. the speed can be had with other more reliable setups.
```

---
## \#50 Posted by: Deckoz Posted at: 2017-12-13T00:08:06.619Z Reads: 73

```
Lol... Hmm I've heard this story before...
```

---
## \#51 Posted by: willpark16 Posted at: 2017-12-13T01:21:55.032Z Reads: 72

```
I've had multiple foc boxes and Olin vesc on 10s and 12s for 245, 110, 149, 190, and 170kv no problems
```

---
## \#52 Posted by: Hariboisawesome Posted at: 2017-12-13T02:32:06.456Z Reads: 70

```
I completely disagree. The Vesc work perfect and the price is right if you are on a budget. I’ve bought 5 vesc all from @torqueboards and the only issue I’ve run into was because I didn’t set up FOC properly
```

---
## \#53 Posted by: coleg411 Posted at: 2017-12-13T03:13:28.428Z Reads: 68

```
for 245kv did you limit the erpm or the top speed some how?
```

---
## \#54 Posted by: willpark16 Posted at: 2017-12-13T03:15:11.930Z Reads: 70

```
I actually never limited the Erpm I'm just super light and never went fast
```

---
## \#55 Posted by: coleg411 Posted at: 2017-12-13T03:28:32.331Z Reads: 69

```
Ok, but do you think that If I use an Ollin Vesc, and limit the erpm to 55k, I should be safe? I doubt that I will be going over the erpm anyway because that is over 30mph for me. Are there other ways to limit top speed?
```

---
## \#56 Posted by: willpark16 Posted at: 2017-12-13T03:30:59.684Z Reads: 71

```
I think that will be fine just don't try racing the board, I would say if you want to never have to worry get a 190kv motor
```

---
## \#57 Posted by: coleg411 Posted at: 2017-12-13T03:35:23.208Z Reads: 69

```
Ok, because I am on a limited budget, what inexpensive 190kv motor would you recommend. what could I do with my old SK3? Its in very good condition with limited riding on it.
What about this one that I found https://hobbyking.com/en_us/kd-53-30-high-voltage-brushless-outrunner-190kv.html?wrh_pdp=3&___store=en_us
```

---
## \#58 Posted by: willpark16 Posted at: 2017-12-13T03:38:28.094Z Reads: 66

```
That one works
```

---
## \#59 Posted by: coleg411 Posted at: 2017-12-13T03:42:58.809Z Reads: 64

```
Is there a reason the I should beware of because of the lower price than the SK3?
```

---
## \#60 Posted by: willpark16 Posted at: 2017-12-13T03:44:41.749Z Reads: 64

```
Nah just look up the motor in the search function u aren't the first to use it
```

---
## \#61 Posted by: coleg411 Posted at: 2017-12-13T04:06:17.327Z Reads: 64

```
If I were to sell my old SK3, in very good condition, do you think anybody would buy it?
```

---
## \#62 Posted by: willpark16 Posted at: 2017-12-13T04:07:30.543Z Reads: 66

```
Don't see why not just sell it at the cost of what you need to buy your new motor
```

---
## \#63 Posted by: coleg411 Posted at: 2017-12-13T04:10:27.994Z Reads: 64

```
I could sell it for $50 maybe, or just run the risk using the erpm limiter for my current motor
```

---
## \#64 Posted by: willpark16 Posted at: 2017-12-13T04:15:38.419Z Reads: 63

```
Up to you man
```

---
## \#65 Posted by: Acido Posted at: 2017-12-13T09:53:13.473Z Reads: 62

```
They are good for lower voltages, if you go 10 or 12s theres a pretty good chance of blowing it
```

---
## \#66 Posted by: Hariboisawesome Posted at: 2017-12-13T15:01:24.186Z Reads: 58

```
Thanks for the tip man! I didn’t realize that 10s could possibly cause issues as well
```

---
## \#67 Posted by: GrecoMan Posted at: 2017-12-13T15:06:25.745Z Reads: 58

```
ive never had an issue with 10s on the TB vesc. it just doesn’t do FOC well
```

---
## \#68 Posted by: Hariboisawesome Posted at: 2017-12-13T15:09:35.702Z Reads: 58

```
Yea I found this out the hard way. Lol.
```

---
## \#69 Posted by: mmaner Posted at: 2017-12-13T16:09:49.440Z Reads: 56

```
[quote="GrecoMan, post:67, topic:40642, full:true"]
ive never had an issue with 10s on the TB vesc. it just doesn’t do FOC well
[/quote]

The older versions didnt, the ones Ive bought in the last 6 to 8 months have had no issue.  I've got a spud running a single 190kv 6355 motor on 10s in FOC and have had no issues.  Ive got around 300 miles on it.
```

---
## \#70 Posted by: coleg411 Posted at: 2017-12-13T18:16:15.630Z Reads: 54

```
Hmm, I wonder what makes mine keep dying then?
```

---
## \#71 Posted by: TarzanHBK Posted at: 2017-12-14T09:00:14.567Z Reads: 54

```
like said before, the higher you go on motor kV, the more likely you fry your DRV.
If you wanna go safe on foc, get an improved one with upgraded components and use a motor with less kV then recommended. For example 10s with 140 kV, maybe 170 kV should be more than bulletproof.
```

---
