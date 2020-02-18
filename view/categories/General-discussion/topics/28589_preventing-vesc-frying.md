# Preventing VESC frying

### Replies: 22 Views: 1596

## \#1 Posted by: Quezacotl Posted at: 2017-07-25T13:29:39.864Z Reads: 230

```
Hello!

I just fried two VESCs with incorrect settings. Seems that there is not much info floating about how to prevent it frying.
I have used BLDC mode for a while, and now i tried FOC. It brought a DRV8302 fault, indicating broken chip. I just tested it on bench...

So any guidelines for preventing frying? Even though it is 10min to swap the chip, it is frustrating in the long run.

One thing that i read somewhere, and noticed, is that the current ramping bug still exists. I had that value around 40, a 1000 times bigger than default. But does it affect FOC mode?
```

---
## \#2 Posted by: Tuomalar Posted at: 2017-07-25T13:34:50.980Z Reads: 233

```
There is massive amount of information how not to fry your vesc. First and most known is "don't use FOC" with "older" vescs. 
What vesc did u use?
```

---
## \#3 Posted by: Quezacotl Posted at: 2017-07-25T14:04:16.871Z Reads: 231

```
Version 4.12 is what i have, and latest default vedder firmware from github.
```

---
## \#4 Posted by: Silverline Posted at: 2017-07-25T14:14:05.983Z Reads: 229

```
Yes but what brand ? A enertion focbox is also 4.12 vesc the same is a maytech vesc, but the performance quality is NOT THE SAME
```

---
## \#5 Posted by: Quezacotl Posted at: 2017-07-25T14:47:27.166Z Reads: 212

```
They are from eBay seller "softempower". It is the same hardware that is in vedder's github page.

I didn't realize that 4.12 could be understood as other than 4.12. Focbox and maytech versions are not 4.12 if they differ from the original.

Oh, and before you ask. I have 270KV motor with 10S lipos.
```

---
## \#6 Posted by: TranxFu Posted at: 2017-07-25T14:59:53.823Z Reads: 207

```
Well, 270kv on 10s is not a good combination. And even worse if you tried a maytech vesc in foc :/ ... Either get a lower kv motor or go lover on the voltage. 270kv on 36v is way above the rpm limit which the vesc can handle. Either they fried because of that or because you went FOC on a maytech vesc.
```

---
## \#7 Posted by: Quezacotl Posted at: 2017-07-25T15:09:31.892Z Reads: 204

```
Hmm.. So "maytech VESC" is considered to be the official version?

Yea i remember reading about KV limits related to batteries. Gotta find that info again.
Edit: Okay i found info, but nothing that it would hurt anything. Will be searching more...
```

---
## \#8 Posted by: Tuomalar Posted at: 2017-07-25T20:48:31.433Z Reads: 188

```
No. Maytech's vesc is just one option among the others. What comes to reliability of Maytech's vesc it isn't. However Focbox has proven to be one of the best if not the best model of vesc 4.

And limit you vesc erpm to 60 000. With 270kv motor use 6s battery or with 10s use 190Kv motor.
```

---
## \#9 Posted by: Quezacotl Posted at: 2017-07-26T06:02:03.827Z Reads: 171

```
Okay. Thanks!
```

---
## \#10 Posted by: pennyboard Posted at: 2017-07-26T06:26:16.190Z Reads: 169

```
I have a July 2016 Torqueboards VESC, I'm hoping to run FOC on it at 12s. Am I just asking to fry the VESC or is this relatively safe? I know the newer ones can handle it, but I'm wondering if anyone has an experience with the older ones like mine.
```

---
## \#11 Posted by: Quezacotl Posted at: 2017-07-26T07:46:32.552Z Reads: 153

```
I just calculated that with my setup(42V / 270KV), the max RPM would be 11340, therefore max ERPM would be 79380.
But i still don't understand where the 60000 ERPM comes from. I have just read that many agree that it is a good number to aim for.
```

---
## \#12 Posted by: Vieo Posted at: 2017-07-26T07:54:46.729Z Reads: 152

```
I _think_ it's a hardware limitation of the DRV8302 chip

(someone please correct me if i'm wrong)
```

---
## \#13 Posted by: Quezacotl Posted at: 2017-07-26T08:59:16.966Z Reads: 146

```
DRV8302 has switching frequency of 200kHz, so it can't be it.
But yea, for some reason running higher than 60000 causes more failures. But then i wonder why it isn't defaulted to that value.

But now i'm in conclusion that i don't use FOC until i get a better motor.
```

---
## \#14 Posted by: Tuomalar Posted at: 2017-07-26T09:01:38.741Z Reads: 139

```
[quote="Quezacotl, post:13, topic:28589"]
better motor.
[/quote]


Better motor doesn't help when u use crappy vescs.
```

---
## \#15 Posted by: Bazingazunga Posted at: 2017-07-26T14:56:22.896Z Reads: 124

```
There's a pretty famous couple threads on this forum from ages ago were people do the math and suggest 60,000 as your safest option. To lazy to find it but yeah, although you have a little bit of flex on that 79000 is just asking for a problem.
```

---
## \#16 Posted by: Klattrup Posted at: 2017-07-26T18:31:39.120Z Reads: 114

```
<img src="/uploads/db1493/original/3X/4/4/44d7b20eca6033b8bb62733c200bca5add54c636.jpg" width="666" height="500">

How do I spot if my VESCs are "good" or "bad" besides being from Maytech? I bought these from vesc.co.uk and they do appear to be of very nice quality. I'm just about to kick off the build of my eMTB and I plan to use these in FOC mode, but these reports scares me a bit! :)
```

---
## \#17 Posted by: longhairedboy Posted at: 2017-07-26T18:45:24.588Z Reads: 110

```
get a 4.12 from Ollin or AXLE, or get a FocBox. No sense in dicking around with mass produced crap. They cut all kinds of corners on components and production so they don't perform as Vedder intended, and don't support those dicks anyway they don't give back to the community.
```

---
## \#18 Posted by: Tuomalar Posted at: 2017-07-26T21:08:27.154Z Reads: 103

```
There are few updated components and overall good quality in production. Vesc doesn't work in eMTB because it can't handle those amps and FOC with these cheap vescs is always risk. So it's like bomb x 2. Look what LHB said.
```

---
## \#19 Posted by: bmcm Posted at: 2017-07-27T21:13:10.049Z Reads: 83

```
Please elaborate on using (or not using) a VESC for eMTB. My Ollin VESC 4.12 seemed to work "fine" (but can't confirm "great" yet) with my 8" pneumatics + 17/72 ratio + 6364 190kv + 10s in BLDC mode.
```

---
## \#20 Posted by: Tuomalar Posted at: 2017-07-27T21:29:28.055Z Reads: 81

```
I have read a lot of eMTB builds and most of them changed vescs to escs because eMTB simply draw much more amps than basic esk8 if you ride hard offroad.
```

---
## \#21 Posted by: bmcm Posted at: 2017-07-27T21:54:43.987Z Reads: 78

```
Ah, I see. Thanks for the clarification. I don't ride offroad; I just wanted the big wheels for the terrible Atlanta roads and sidewalks, and some grass/gravel. So I shouldn't be pulling more amps than my Ollin VESC can handle *crosses fingers* *knocks on wood*
```

---
## \#22 Posted by: Klattrup Posted at: 2017-07-28T07:54:35.735Z Reads: 70

```
Thanks guys, that actually helped me out aswell. :+1: I belive I'm going to use my board the same way as you do @bmcm :)
```

---
