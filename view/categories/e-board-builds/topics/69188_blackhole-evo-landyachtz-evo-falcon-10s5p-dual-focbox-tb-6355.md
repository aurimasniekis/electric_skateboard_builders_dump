# Blackhole Evo &#124; Landyachtz Evo Falcon &#124; 10s5p &#124; Dual Focbox &#124; TB 6355

### Replies: 56 Views: 2830

## \#1 Posted by: Static Posted at: 2018-09-25T20:36:28.614Z Reads: 422

```
This build has been many months in the making while accumulating parts. Hence the name "Blackhole Evo" as this has been an expensive journey. But alas, it was worth it. The final product is simply awesome. 

I started with the basics that I knew would be in the final board.

-Landyachtz Evo Falcon

-107mm Abec 11 

-Caliber II trucks

-Riptide bushings

Planning out the power system I knew that I wanted to use a newer vesc than the TB 4.12 that I already have. The breif moment I had with FOC was great, so that was going to be a criteria for this build and I needed something reliable. I had already purchased two Focboxes earlier this year from their summer sale, but didn't know if I wanted to use those or not. A short time after that another Escape GB started so I jumped on that and a GB buy for two Flipsky 6.6 as well. So in the end I had 3 three different ESCs to choose from. That was expensive, but curiosity has a way of spending my money. 

While waiting for more parts I had some time to mill a heat block for the two Focboxes. The part turned out better than I expected and I was actually curious to know if it would make a noticeable performance difference. Plus I went with a 10s5p battery so it made more sense to use them anyway.

So for the electronics:

-Dual Focboxes

-TB 6355 190kv

-10s5p 30q battery

-Nano-x remote

-HM-10 bluetooth module


![image|424x500](upload://wydRZg90PAklzOJ72Tl1rSPpXDP.jpeg) 
![image|666x500](upload://bhuMYATXkHW1PlcH9L1CZRCiOnM.jpeg) 
 
The 10s5p came from @psychotiller , a double stacked flat pack that fits the board well. Unfortunately neither of the two enclosures I got from Psychotiller would fit the deck without loads of modification (why can't I just copy what others have done). So I went with the @eboosted enclosure, not knowing if I'd be able to fit the battery. 

![image|375x500](upload://3MuwcYnmZHTlhFWy5I2PRsatQwo.jpeg) 

I'm glad I did, with a 3/8 in foam gasket the eboosted enclosure fits perfectly and looks great. On a side note, this is the only way I will assemble boards from now on. Attaching everything to the board was so much easier to get the clearance I needed. Removing the enclosure is also much easier. 

![image|690x370](upload://o0oikmDKUR7b2ICzkHwdALvjVOz.jpeg) 
![image|375x500](upload://uT8sBwvV9ZnyfFkdWtasxTSQhmG.jpeg) 

On the drive/powertain, I wasn't going to bother with forward mounted motors. I'd rather not have those space restrictions even though I really like the stealth look with FOC. So instead I'm using TB extended reverse mounts along with 18t motor pulleys and 36t wheel pulleys. Red wheel pulleys came from ebay and needed to be lathed down to 12mm.

![image|666x500](upload://yalQ5E5m8onEE9N6lRCjfImYBYg.jpeg) 
![image|666x500](upload://vLB8bBIokRdpw1ukSTXjD1cJelV.jpeg) 

Upon testing I immediately determined there was either an issue with the motor, sensor wire, or Focbox because hall detection was not working. After eliminating some variables I determined that one of my new Foxboxes was faulty, the one that came with the mangled connectors...

I really didn't want to deal with Enertion, but I had spent too much effort configuring this board for focboxes. I decided before getting too angry to open the ESC and see if anything obvious stood out... and there it was. 
![image|689x388](upload://stBImiGfQlWaLBljRod6xI5O6Yi.jpeg) very fortunate to just be a bridged connection

With the problem fixed and FOC working perfectly it was time for a test ride. 

I used these settings:

Motor max 70
motor regen -40
Batt max 40
batt min -10 (not sure what I can go up to here safely)

Despite how I feel about Enertion I really like their remote. The speed selector switch should be standard on all remotes. On full power the board is a rocket and feels just as good as my other 12s board with 6374s. Top speed is perfect too, right at 40mph thanks to the 18t wheel pulley. Feels very stable and I have no problem taking corners at speed. Couldn't be happier with the performance.

![image|666x500](upload://hCB1SDIK9Vo84V5zTJLeqsXqhfj.jpeg) 
![image|666x500](upload://sYngsnr3W2FTltM0x11gYnKmclE.jpeg) 

Couldn't get the HM-10 module to pair. I really wanted to see some actual data but the module will not pair to my android phone. It's visible as "HMsoft" in bluetooth settings, but when I attempt to connect it doesn't. Not sure if I have properly enabled PPM + UART on the ESC. I select PPM + UART but when I check the vesc tool again (App Settings> general) it shows only PPM.

If you have any insight I'd appreciate a comment.

Thanks for looking.
```

---
## \#2 Posted by: Jake2k17 Posted at: 2018-09-25T22:22:01.428Z Reads: 356

```
Damn bro, That’s a sexy looking build! How come you went with the 6355 and not 6374?
```

---
## \#3 Posted by: mixedcreation Posted at: 2018-09-25T22:28:05.015Z Reads: 354

```
Because he has caliber 2 trucks. 

Nice build! Damn everyone has an Evo..I feel left out of the club.
```

---
## \#4 Posted by: topcloud Posted at: 2018-09-25T22:43:40.166Z Reads: 354

```
![S0bcKst4Xa6x|610x403](upload://fAD1yGXX73zy1tB85xg1EwYeKMM.jpeg) 

one of my favorite builds this year.

everything you need - and nothing you don't.  

do heart!
```

---
## \#5 Posted by: Static Posted at: 2018-09-25T22:58:51.867Z Reads: 324

```
@Jake2k17 yeah what @mixedcreation said. I wanted a narrower overall profile plus 6355 motors have plenty of power.
```

---
## \#6 Posted by: mixedcreation Posted at: 2018-09-26T00:54:33.833Z Reads: 317

```
@Static did you get your 18t from Ebay? I have 2 coming from dickyho...but just wondering if you got them from another source. 

How is the torque with your setup?
```

---
## \#7 Posted by: Static Posted at: 2018-09-26T01:35:08.788Z Reads: 310

```
They came from diyelectric. The torque is excellent although I'm running near max settings for my setup.
```

---
## \#8 Posted by: mixedcreation Posted at: 2018-09-26T02:05:40.661Z Reads: 300

```
Damn dexter had 18t... I obviously missed that.  Thanks for the heads up.
```

---
## \#9 Posted by: Grozniy Posted at: 2018-09-26T08:52:12.248Z Reads: 296

```
It's possible that your phone is too new. It doesn't work on Android 8.  In my case it only works on my old phone.
```

---
## \#10 Posted by: dareno Posted at: 2018-09-26T09:59:27.309Z Reads: 284

```
Looks great man!  Just love the evo deck.  Quick question. Did you get the bolt set from Alan?  If so did you install the nut serts under the deck or through the top.  Can't tell from the pics
```

---
## \#11 Posted by: dareno Posted at: 2018-09-26T10:03:19.711Z Reads: 285

```
I know right.  Seems I'm late to the party. But there none the less  soon
```

---
## \#12 Posted by: Static Posted at: 2018-09-26T13:33:24.316Z Reads: 289

```
Well I figured out how to write the PPM+ UART setting to the vesc and I finally have the Metr module working. Still nothing on the HM-10 I think I'll try an older phone @Grozniy 

@dareno they are installed under the deck. @psychotiller made a pretty good write up [about mounting](https://www.electric-skateboard.builders/t/mounting-your-enclosure/46001)

.
```

---
## \#13 Posted by: brenternet Posted at: 2018-09-26T21:05:04.616Z Reads: 284

```
Snap :smiley:

![20180904_145226|374x500](upload://g3MIOJbgy1MAjtnEaNMRirTXzlr.jpg) ![20180906_093522|666x500](upload://qmzlZaBUzFTTVXzlpH73NBdIIVp.jpg)
```

---
## \#14 Posted by: Static Posted at: 2018-09-26T23:18:44.800Z Reads: 272

```
Ha that's nearly the same board! It's a great ride isn't it? I didn't find the need to use the idlers either.
```

---
## \#15 Posted by: brenternet Posted at: 2018-09-26T23:46:14.066Z Reads: 267

```
Honestly, might as well be the same board! 10s5p 30q, foxboxes, calibers, 107s, tb reverse.

Best feature for me is that you can stand it on the nose with perfect balance 😁
```

---
## \#16 Posted by: r18duarte Posted at: 2018-09-27T21:36:35.986Z Reads: 260

```
well i saw landyachtz and immediately clicked it. i've ridden this board but i was pushing it and was amazing. i wanted this to be my first build but 500€ for the battery is an abuse.. in europe it's hard to get these stuff without it being on the customs and paying a lot of money to get them back.

edit: found a place where i could get a 10s2p for 250$ i don't need a huge range 10 km are enough for my daily comute but still i know that they're coming from the USA and going to pay taxes as soon as they enter portugal..
```

---
## \#17 Posted by: Grozniy Posted at: 2018-09-27T22:36:16.544Z Reads: 243

```
Podes falar com @Acido ou @PWR-BOARDS sobre baterias personalizadas dentro de EU ;)
```

---
## \#18 Posted by: brenternet Posted at: 2018-09-27T22:56:39.696Z Reads: 246

```
... and eskating.eu @pjotr47 electricboardsolutions.com unikboards.com @darkkevind and the list goes on.

There's loads of placed to get a battery in europe.
```

---
## \#19 Posted by: Sender Posted at: 2018-09-27T23:23:51.636Z Reads: 240

```
Replace that coffee with a beer for a perfect setting...
```

---
## \#20 Posted by: Static Posted at: 2018-10-25T23:40:09.883Z Reads: 238

```
![1|690x460](upload://bisuK7t3vrgENe31os9f2K1ZaNZ.jpeg) ![2|690x460](upload://hjC6IvcLK8eKLWy2k1tY3kLA7UN.jpeg) ![3|323x499](upload://3NL1Xiz6i2onZqUaForHyV4ORPy.jpeg)
```

---
## \#21 Posted by: Static Posted at: 2018-10-25T23:42:10.641Z Reads: 234

```
![image|690x407](upload://flNzvGMG0emA8prqooeWHJpEi4p.jpeg) 

I designed a handle/bumper for TB rear mounts. Been using it for a few weeks without any issues, seems pretty strong even in PLA. STL available [HERE](https://www.thingiverse.com/thing:3165250)
```

---
## \#22 Posted by: brenternet Posted at: 2018-10-26T00:07:26.894Z Reads: 231

```
Amazing thank you. I'll cnc it. 

I often find myself wrapping my hand around the motors to pull it short distances. This will turn it into a bit more of a suitcase. Perfect mod
```

---
## \#23 Posted by: Static Posted at: 2018-10-26T00:11:48.098Z Reads: 227

```
CNC all the way if you can. Can't wait until I have a CNC mill available to use, sooooon.

Make sure to get the spacing right between the brackets and adjust if needed, in my case it was 127.2mm. I'd print a test fit first. :smiley:
```

---
## \#24 Posted by: Battosaii Posted at: 2018-10-26T00:15:24.870Z Reads: 230

```
Oh man id love a set of those. I have motors on the front and back and feel bit exposed.
```

---
## \#25 Posted by: murdomeek Posted at: 2018-10-26T06:08:41.161Z Reads: 221

```
slick build!
how much was the total cost if you dont mind me asking?
```

---
## \#26 Posted by: Static Posted at: 2018-10-26T14:00:25.286Z Reads: 213

```
Approx $1500-1600, I waited for sales on a few items
```

---
## \#27 Posted by: Ghost1068 Posted at: 2018-11-10T23:22:24.931Z Reads: 212

```
This is my ideal build right here. I have been wanting a Carvon Evo 4wd for a long time now but with what I have heard about the wait it just sounds like a complete nightmare and I'm not willing to lay up $3500 for something there is absolutely no definitive time frame on/ unresponsive customer service given such a high price tag. Some of the guys here in NYC have Evo diy builds; both belt drive and carvon xl/ carbon torque drives. With that said, I actually love the way the belt drives feel on this board, so stable and fast - plus the power is so smooth. I have been researching a ton and your build honestly seems to be exactly what I'm looking to do. It's honestly the nicest DIY I've EVER SEEN. Beautiful bro.

Like I said, I plan on doing almost the same thing. Diyeboards sells a "pro 3 kit" which has the TB 6374 190kv motors, 12s4p 30q battery pack, torque motor mounts, TB 218mm trucks etc. However it comes with a TB VESC and from what I understand this is not ideal? Would you use this for get the Foc Boxes? Also what kind of specs can I expect from the 6374 motors compared to your 6355s? I want a similar top speed (around 40mph). See the kit here collections/electric-skateboard-conversion-kit/products/pro3-electric-skateboard-conversion-kit

Any input here would help - thanks!!
```

---
## \#28 Posted by: Static Posted at: 2018-11-11T00:34:07.701Z Reads: 200

```
Read around the forum and other Evo builds. Do you know why a TB vesc isn't ideal? If you're gonna build one you gotta read a lot first to know what you're doing. 

That said, TB vesc's are fine. They're (currently) v4 vescs so FOC isn't perfectly stable so you're safer running in BLDC or Hybrid mode which either it does fine. Focboxes are V4 vescs as well but have upgraded components to run in FOC. 

They're bigger motors so they'll have more torque, top speed is determined by kv
```

---
## \#29 Posted by: Ghost1068 Posted at: 2018-11-13T18:34:04.476Z Reads: 196

```
I appreciate the input. I currently have a Boosted Board V2 dual plus Xr & an Ownboard W1s. However, I am looking for something with more speed and definitely want the Evo deck. I just figured that for the money this Torque Board pro 3 kit has everything I need. Do you think the Torque Boards VESC would be fine then? In other words, is it a decent VESC? Also, I completely understand what you are saying about the motors, what I was asking is where would the top speed be compared to your 6355 motors? Thanks again for the responses.

Only reason I reached out to you specifically was because of all the Evos I looked at, yours was the closest to what I want.... It's a compliment!
```

---
## \#30 Posted by: Static Posted at: 2018-11-13T18:45:07.160Z Reads: 197

```
It does have everything you need, but it's also not hard to source those parts around the forum. Personally, the wheels, bearings, battery and enclosure are all things I would change. Although, they are updating a lot of their catalog for 2019 fyi.

It's a decent vesc yes from my experience and most others. Learn what all the terms I mentioned mean and it will help you make your decision. For instance do you need a silent ride?

Top speed is determined by KV, both 6355 and 6374 are 190kv. So for the same voltage they will spin the same speed, one has more torque. [Use this](http://calc.esk8.it/#{%22batt-type-lipo%22:1,%22batt-cells%22:12,%22motor-kv%22:190,%22system-efficiency%22:85,%22motor-pulley-teeth%22:19,%22wheel-pulley-teeth%22:36,%22wheel-size%22:90}|) and read on the forum some more
```

---
## \#31 Posted by: Ghost1068 Posted at: 2018-11-13T19:06:28.782Z Reads: 191

```
I believe the battery uses Samsung 30Q cells in a 12s4p configuration. From what I've read 30q cells have the highest continuous rate of almost any cell. Are you saying you would change the configuration, the cell type, or both? 

As for doing the research, I definitely will! I just figured for the price and convenience factor the kit would be good. Obviously I would change the wheels to Abec 107s and put on zealous or Swiss bones bearings. 

Your input so far is a huge help! Thanks man.
```

---
## \#32 Posted by: Ghost1068 Posted at: 2018-11-13T19:07:08.849Z Reads: 180

```
Noise factor is not an issue. Like I said I have the boosted which is loud and the Ownboard which is silent and don't have a preference.
```

---
## \#33 Posted by: Static Posted at: 2018-11-13T20:03:28.472Z Reads: 172

```
Samsung 30Q is the current standard for most people because the price/performance ratio is good (30q is 15amp so a 12s4p can supply 60a). They're fine, id just change the layout to flat. If you want more convenience that will come from understanding the all of the parts well before you buy them. You'll save more money doing that than buying a kit.
```

---
## \#34 Posted by: Lobbie Posted at: 2018-11-24T09:13:44.536Z Reads: 163

```
Hello, you said that you couldnt be bothered with putting the motors underneath the board, but would they fit if you did and do you think it would fit with 6374 motors? Also how much ground clearance do you have. I am building a PRO3 electric skateboard conversion kit and am struggling to find a deck, thanks!
```

---
## \#35 Posted by: brenternet Posted at: 2018-11-24T13:13:13.746Z Reads: 164

```
You won't get the motors under the deck with an eboosted enclosure. If the enclosure is flat backed and doesn't follow the curve of the drop and you had some short mounts you might get them forward.

You can't get 74s on a 10" caliber 2 but on tb218s or ecalibers or basically anything longer you could. I think you would struggle getting a larger can to sit well forward in that drop on the falcon though.
```

---
## \#36 Posted by: reedbryson Posted at: 2018-11-27T16:18:54.701Z Reads: 154

```
Beautiful build!  Nice work.  I have been looking at a similar build but with a bustin boards 35" sportster deck.  I love the rear handle Idea!  Now I just need to find a 3d printer lol
```

---
## \#37 Posted by: taz Posted at: 2018-11-28T17:11:30.109Z Reads: 159

```
[quote="brenternet, post:35, topic:69188"]
You won’t get the motors under the deck with an eboosted enclosure.
[/quote]

I am pretty sure that is not the case.

https://www.electric-skateboard.builders/t/master-evo-landyachtz-abec-107-13s5p-focbox-6374-190kv-metr/44411/102?u=taz
```

---
## \#38 Posted by: Static Posted at: 2018-11-28T17:13:12.112Z Reads: 151

```
That's a different deck though. More space
```

---
## \#39 Posted by: taz Posted at: 2018-11-28T17:16:55.647Z Reads: 147

```
It is longer, however from the pictures I have seen, the transition from the middle of the deck to the rear seems the same as the falcon and the same thing looks to be the case for the enclosure.
However I do not possess a falcon to compare to the evo so I may be wrong.
```

---
## \#40 Posted by: Static Posted at: 2018-11-28T17:20:44.604Z Reads: 156

```
I have both. The falcon has less room for motors underneath. With the skate and explore deck you have more room/extension at the end.
```

---
## \#41 Posted by: taz Posted at: 2018-11-28T17:24:49.134Z Reads: 150

```
![200w|200x148](upload://4WFVZA2QLH1JJmO3dk0N5vesSFN.gif)
```

---
## \#42 Posted by: Static Posted at: 2018-11-28T17:29:02.080Z Reads: 152

```
Getting hard to find that deck too. It's the perfect esk8 deck.
```

---
## \#43 Posted by: taz Posted at: 2018-11-28T17:29:42.600Z Reads: 155

```
Are you talking about the Evo or the falcon?
```

---
## \#44 Posted by: Static Posted at: 2018-11-28T17:30:20.908Z Reads: 154

```
The 39" skate and explore evo
```

---
## \#45 Posted by: taz Posted at: 2018-11-28T17:32:07.892Z Reads: 155

```
I know. This is why I stocked up :sunglasses:

![20181001_184107|374x500](upload://grVuPMoCBOSGdFG9PJUIvpmLqzf.jpeg)
```

---
## \#46 Posted by: brenternet Posted at: 2018-11-28T17:41:51.955Z Reads: 149

```
As people have said the falcon has quite a bit less space in front of the back truck unfortunately. The enclosure doesn't really work in its current form for forward mounting.

Quite disappointing.
```

---
## \#47 Posted by: Static Posted at: 2018-11-28T17:44:08.627Z Reads: 149

```
The shorter falcon would be perfect for DD or hubs. Could really drop it low that way too.
```

---
## \#48 Posted by: brenternet Posted at: 2018-11-28T18:15:36.872Z Reads: 148

```
My falcon is on it's way to a new home now but before I let it go I did some measurements on a surfrodz tkp and with short custom mounts you would be able to forward mount 6355 size cans.

The extra space the tkp profile offers is just enough.
```

---
## \#49 Posted by: Static Posted at: 2018-12-03T16:13:11.493Z Reads: 141

```
36" vs 39" evo

![image|353x499](upload://odX1f6Xm6pWR2HmEGRroTJyxozh.jpeg)
```

---
## \#50 Posted by: mishrasubhransu Posted at: 2018-12-03T17:16:32.265Z Reads: 135

```
You should post this on the no words thread. Pretty useful thing for all the TB mount users.
```

---
## \#51 Posted by: sk8l8r Posted at: 2018-12-03T18:51:32.568Z Reads: 131

```
I managed to fit under on my falcon wasn't ideal and I dewedged, it didn't fit until I did that 

https://www.electric-skateboard.builders/t/clone-evo-landyachtz-evo-falcon-abec-107-or-boa-100-13s5p-top-mount-focbox-6374-190kv-metr-pro/57765

Edit:. Still wish I had the bigger size I find it too cramped
```

---
## \#52 Posted by: dareno Posted at: 2018-12-03T19:54:55.387Z Reads: 126

```
Transplant it mate.  That full size evo is far and away my fav esk8 deck to date.  At 6ft 2 I find it locks you in like no other deck.  I went reverse on mine so I could keep the original angles and its so solid at silly speeds.
```

---
## \#53 Posted by: Static Posted at: 2018-12-03T20:06:29.623Z Reads: 127

```
I am very tempted to transplant things. Although, the current proportions are perfect for me. The narrow profile gives it a great stance. 

The 39" was planned for TB direct drives. We'll see, I bought too much this holiday season so I'll have a lot to choose from.
```

---
## \#54 Posted by: dareno Posted at: 2018-12-03T20:22:18.067Z Reads: 133

```
Apologies my friend that reply was for @sk8l8r.  Like him I found the falcon just a bit cramped for my height and stance.  I couldn't get hold of the 39 when I originally started my build and bought a complete falcon.  Used it as a pushy and sold it on when I found a 39 on here.  A friend has it now with plans to go all out with a build but he is under 6 ft so it works beautifully for him.  I have 4 boards atm and 3 are gathering dust because of the evo.   Just love it.
```

---
## \#55 Posted by: hicklinc Posted at: 2019-12-09T17:27:32.449Z Reads: 31

```
do they mount threw the standard motor mount holes and did you need longer hardware
```

---
## \#56 Posted by: Static Posted at: 2019-12-10T14:28:19.547Z Reads: 30

```
Uses the m2.5 holes on the mounts- they are typically unused. not the motor holes

fyi this forum is dead head over to esk8 news
```

---
