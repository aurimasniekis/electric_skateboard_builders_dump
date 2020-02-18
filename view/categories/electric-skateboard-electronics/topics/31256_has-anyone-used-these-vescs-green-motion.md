# Has anyone used these VESCs - Green Motion?

### Replies: 34 Views: 1760

## \#1 Posted by: rolexbene Posted at: 2017-08-22T15:04:36.006Z Reads: 239

```
Just gathering parts for my first build. Just took a bit of a impulse buy, and bought a single one of these VESCs from ebay user 'naama1485' or from 'Green motion electric vehicle solutions' based in Israel.

I just wanted to see if anyone on here could shed any light on the quality of these, are they rebranded Chinese VESC Should I avoid using them in VOC?

http://www.ebay.co.uk/itm/Twin-Pack-VESC-BLDC-Open-Source-Electric-Skateboard-ESC-/152533373148?hash=item2383b290dc:g:RyoAAOSwNRdX2smF

Will be posting a build log soon when my parts start to arrive, so we can all see the outcome.
```

---
## \#2 Posted by: rich Posted at: 2017-08-22T15:26:00.248Z Reads: 231

```
As far as I know they are rebranded maytech from china. They run in BLDC mode but don't like FOC.
```

---
## \#3 Posted by: onepunchboard Posted at: 2017-08-22T19:04:11.599Z Reads: 210

```
I used may tech before. they died now. they also have old fmw 2.18 with some bug. not recommended
```

---
## \#4 Posted by: rolexbene Posted at: 2017-08-22T20:03:10.294Z Reads: 197

```
Are the defiantly Maytech then? I was planning on updating the firmware as soon as I got them, is this not possible?
```

---
## \#5 Posted by: onepunchboard Posted at: 2017-08-22T20:38:38.222Z Reads: 183

```
not possible they tells me to buy their STlink. I told them it's buggy fmw but they deny their fault and blame vadder. i disputed in aliexpress to stop their business. long story short never buy maytech esc.
```

---
## \#6 Posted by: rolexbene Posted at: 2017-08-22T22:45:20.480Z Reads: 159

```
[quote="onepunchboard, post:5, topic:31256"]
STlink
[/quote]

That looks strange, although it seems you could buy one for cheap on ebay if this is the only way to update FW.

http://www.ebay.co.uk/itm/ST-Link-V2-New-STM32-Downloader-Programming-STM8-Unit-Emulator-Mini-HOT-/202029005922?epid=921877230&hash=item2f09ddfc62:g:mwsAAOSw5SZZktyE
```

---
## \#7 Posted by: sl33py Posted at: 2017-08-22T22:49:26.524Z Reads: 143

```
You can also push firmware via new VESC Tool without STLink - once released.  Still Beta, but i did this for two older VESC 4.7 with no problem.

Unsure on VESC Tool release... but helps those w/o bootloader (to update fw).
```

---
## \#8 Posted by: onepunchboard Posted at: 2017-08-22T23:16:24.662Z Reads: 136

```
well it's up to u to decide. I know the price is tempting.
```

---
## \#9 Posted by: rich Posted at: 2017-08-23T06:46:11.778Z Reads: 124

```
You already bought it so there is one important thing to check before using it as @onepunchboard mentioned. I have 2 maytech and both had buggy FW. You have to check your current ramp step setting in advanced tab. It should be 0.04 (mine was 40 :astonished:) Everytime you click read or write configuration this value gets multiplicated by 10. You can test this by clicking read configuration several times and watch the current ramp step value. If it stays equal at 0.04 you don't have a bug. But if so you have to set 0.004 and then write configuration (after that the value stay at 0.04 as long as you don't read configuration again). This is the reason why many people fry maytech V4.12. And don't try FOC!

As @sl33py said, you can wait for the new VESC-Tool for uploading your bootloader and firmware. I did it with both maytech's and it's super easy! If you want to do it right now with STLink you can PM me, I ordered a cheap one but won't use it.
```

---
## \#10 Posted by: telnoi Posted at: 2017-08-23T07:05:47.474Z Reads: 111

```
@rich. Thanks for the warning. Also have two maytech incoming.
```

---
## \#11 Posted by: rich Posted at: 2017-08-23T07:19:26.556Z Reads: 109

```
[quote="onepunchboard, post:5, topic:31256"]
I told them it's buggy fmw but they deny their fault and blame vadder
[/quote]

Haha, this is a shame! Also I can't believe they still deliver with faulty FW because they should know. Very funny is the fact that they say "don't use FOC" or not longer than 10 seconds :joy: but when you look at the manual FOC is an own chapter! But from my experience I know how they perform (or better not perform) in FOC, have tried it once. Now I use high quality V4.12 in FOC without problems. I bought 4 cheap V4.12 first until I realized that I lost my money because of buying cheap!
```

---
## \#12 Posted by: rolexbene Posted at: 2017-08-23T08:56:02.036Z Reads: 105

```
[quote="telnoi, post:10, topic:31256"]
incoming
[/quote]

Thanks for all the invaluable advice, will be sure to check to see if it's buggy when I get it. So FOC will still not work after a full FW update. Does anyone know the actual reason for this??

Also, if I want to get a good quality VESC that will run with FOC, which are the reputable suppliers?

Also where do I find release info on the new VESC Tool "without STLink - once released"

Is the Flier VESC from Alien Power Systems any good?
http://alienpowersystem.com/shop/esc/ev-esc/vesc/
```

---
## \#13 Posted by: telnoi Posted at: 2017-08-23T09:21:03.711Z Reads: 92

```
Are you in Europe?
```

---
## \#14 Posted by: Ishayc Posted at: 2017-08-23T09:33:04.864Z Reads: 91

```
Got Greenmotion Vesc.
had to install the bootloader using ST-Link and after that reinstalled the FW to fix the Current Ramp bug.
Running it with BLDC mode and it works just fine, didn't try FOC but heard it's not recommended.
```

---
## \#15 Posted by: rolexbene Posted at: 2017-08-23T11:40:20.245Z Reads: 88

```
Yes telnoi, I am in the UK.
```

---
## \#16 Posted by: telnoi Posted at: 2017-08-23T12:06:50.124Z Reads: 93

```
http://www.electric-skateboard.builders/t/worldwide-vesc-directory/16764

The two German resellers have stock. Alienpower only appears to have items available for backorder/who knows how long that is going to take.
```

---
## \#17 Posted by: rich Posted at: 2017-08-23T12:19:03.024Z Reads: 90

```
[quote="rolexbene, post:12, topic:31256"]
So FOC will still not work after a full FW update. Does anyone know the actual reason for this??
[/quote]

The maytech/greenmotion has minimum parts only. You need better quality with modified and upgraded parts then it will work. In europe I recommend @esk8 (esk8.de) where I bought mine. Just for info I've tried FW 2.18, 2.54 and 3.26 with maytechs in FOC (at home only), everytime hitting the brake (even with no load) the vesc cut off and show up DRV fault. 17 times braking = 17 DRV faults and no braking possible, that's bad!

[quote="rolexbene, post:12, topic:31256"]
Is the Flier VESC from Alien Power Systems any good?
[/quote]

:joy: my 2 remaining cheap V4.12 are flier, greetings from  china!
```

---
## \#18 Posted by: rich Posted at: 2017-08-23T12:21:44.493Z Reads: 90

```
[quote="rolexbene, post:12, topic:31256"]
Also where do I find release info on the new VESC Tool "without STLink - once released"
[/quote]

You don't need info, you go to bootloader tab and click upload, that's it :grin:
```

---
## \#19 Posted by: onepunchboard Posted at: 2017-08-23T12:49:19.135Z Reads: 83

```
I know, it's absolutely ridiculous. 😂
```

---
## \#20 Posted by: telnoi Posted at: 2017-08-23T13:32:23.999Z Reads: 82

```
Is the beta tool available to a select view or can anyone try it?
```

---
## \#21 Posted by: longhairedboy Posted at: 2017-08-23T13:52:08.711Z Reads: 78

```
maytech vescs are garbage. Their motors are good but the vescs are useless for anything over 10S and only do 10S for a little while before they burn.
```

---
## \#22 Posted by: evoheyax Posted at: 2017-08-23T14:05:22.190Z Reads: 76

```
Cause anyone can assemble a decent motor. Electronics though is a lot harder.
```

---
## \#23 Posted by: rolexbene Posted at: 2017-08-23T14:12:18.357Z Reads: 78

```
[quote="longhairedboy, post:21, topic:31256"]
scs are garbage. T
[/quote]

Well I am only going to be running on 8S for now, however would be nice to be able to run VOC and tryout bleeding edge stuff without fear of things going bang. Thinking  I might try and return the item and buy something of better quality.

Can anyone recommend the VESC from proto boards?
https://www.proto-boards.com/product-page/vesc-speed-controller
```

---
## \#24 Posted by: rich Posted at: 2017-08-23T14:48:12.625Z Reads: 73

```
[quote="telnoi, post:20, topic:31256, full:true"]
Is the beta tool available to a select view or can anyone try it?
[/quote]

The VESC Tool is for beta testers only right now but should be released soon :grinning:
```

---
## \#25 Posted by: longhairedboy Posted at: 2017-08-23T14:53:35.651Z Reads: 72

```
If by harder you mean they find it difficult to pay a couple cents more for higher quality components and maybe pay a little more attention to how things fail and adjust their processes accordingly, then yes. So much harder. They're doing none of that. The parts fail because of greed, not because China can't produce amazingly high quality parts. Nothing is keeping maytech parts from being Ollin or AXLE quality other than they have deliberately decided to fully maximize profits at the customer's expense. 

So yeah, its a lot harder to not make quite as much money and instead produce a higher quality product when your only mission is to maximize profits by impregnating the market with quick selling garbage that people buy after doing zero research due to the fact that they can barely contain their excitement over building a board.
```

---
## \#26 Posted by: sl33py Posted at: 2017-08-23T15:34:53.288Z Reads: 69

```
[quote="telnoi, post:20, topic:31256, full:true"]
Is the beta tool available to a select view or can anyone try it?
[/quote]


I have the question out to Frank and Ben on the VESC-Project forum.  Asking when the new VESC Tool will be released to the public.  I'll let you know what they say.

It's worth the wait folks...
```

---
## \#27 Posted by: evoheyax Posted at: 2017-08-23T16:23:56.828Z Reads: 64

```
Yes, they certainly can. But my point is there's a lot less to fuck up with a motor than with the vesc. They need to understand their lack of attention and using low quality parts are not going to work, but how can they when they don't even test their own product in the real world themselves in china?

It's either greed or ignorance, and based on your impressions, it's greed. Either way, they need to get heir shit together.
```

---
## \#28 Posted by: longhairedboy Posted at: 2017-08-23T19:28:59.887Z Reads: 65

```
[quote="evoheyax, post:27, topic:31256"]
Either way, they need to get heir shit together.
[/quote]

I couldn't agree more.
```

---
## \#29 Posted by: telnoi Posted at: 2017-08-24T04:10:58.182Z Reads: 60

```
Well, I went the expensive route after a frustrating search about what components might be best.
I must say, there is allot of conflicting information available in this forum.

1. many mention VESC is not meant to be used for mountain boards, Chinese or not
2. many mention that regular ESCs are crap in general/they burn/cannot stand up to the abuse

Conclusion. Not a single ESC/VESC is suitable for mountain boards. :rage:
Anyway, I hope the focbox type VESCs will save my bacon when going up and down hill/8 km trips.
```

---
## \#30 Posted by: rich Posted at: 2017-08-24T08:21:10.019Z Reads: 56

```
You went the right route @telnoi   :wink:
I'm using dual V4.12 from esk8.de (soon switching to 1.1 controller) and am very happy with the quality and performance. I run them on my mountainboard (and also was afraid because noone recommends it for mountainboard as you said). The performance is great (sensored FOC) for riding. I've never tried ESC but I think with ESC you get more raw power if you want to ride as crazy like @Nowind or want wheelie action. But for me the V4.12 are just fine!
```

---
## \#31 Posted by: telnoi Posted at: 2017-08-24T08:53:26.842Z Reads: 50

```
Good to hear. I ordered the 1.1 controller mainly due to the enclosure and better protection agains the elements.
```

---
## \#32 Posted by: rich Posted at: 2017-08-24T09:24:35.781Z Reads: 50

```
Additionally you get less heat problems and there are many added components and they should deliver more power, too. It's always best to buy quality stuff even when you can't afford it because in the end you buy the cheap plus the quality one.
```

---
## \#33 Posted by: rolexbene Posted at: 2017-08-30T21:42:49.262Z Reads: 39

```
So I received my VESC and I can confirm that it does have the buggy firmware. I would like to try and make it stable by updating it to Ackmaniac fireware and BLDC tool.

When I try and upload from the firmware tab, it seems to be working correctly. but when it finishes upload it crashes Ackmaniac BLDC tool, and on restart it says "the connected vesc has too old firmware..." again.

I have also tried uploading Ackmaniac firmware via the standard BLDC tool and although it does not crash and says upload complete, it does not seem to work with the same problem on restart.

I am guessing that it must be a problem with the bootloader or lack of one? It just seems strange that it goes through the process without error, and says upload complete. I have attached a video of this for example.

Can anyone confirm what is going wrong and what I need to do to fix this? Purchase a ST-Link V2?

https://www.youtube.com/watch?v=vJhH9lAK-sY
```

---
## \#34 Posted by: rich Posted at: 2017-08-30T22:47:08.325Z Reads: 39

```
[quote="rolexbene, post:33, topic:31256"]
So I received my VESC and I can confirm that it does have the buggy firmware.
[/quote]
And no bootloader that's why you can't upload FW. You can upload the bootloader with ST-Link V2 or wait for the new VESC Tool where it's just one click :grin:, should be released very soon.

If you want to use the V4.12 with buggy FW then set the current ramp step to 0.004 and then write configuration (after that the value stays at 0.04 as long as you don't read or write configuration again).
```

---
