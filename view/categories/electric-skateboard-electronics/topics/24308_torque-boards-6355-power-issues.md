# Torque Boards 6355 power issues.. =/

### Replies: 118 Views: 3513

## \#1 Posted by: trancejunkiexxl Posted at: 2017-06-01T01:06:23.777Z Reads: 247

```
Bought a new 63mm motor from , and spent a good amount of time setting it up and finally got it going! I had tons of torque and the belt was slipping like crazy, however now when applying throttle, im losing power intermittently @ approx 3/4 of the throttle i feel like im hitting some limiter or that the power is having trouble being delivered, it sux, and  Ya my soldering skills arent that good, it could be that but i double checked and looked up and down.. if anyone can help me fix id be willing 2 dontate beer.


~Tony 

<img src="/uploads/db1493/original/3X/5/8/5832719c65093cdd72c12f36f8b210900b23b398.jpg" width="281" height="500">
```

---
## \#2 Posted by: Jinra Posted at: 2017-06-01T01:16:28.059Z Reads: 228

```
First off, your motor should be turned 180 degrees. The way it's positioned now will wear down the wire and potentially break it. Likewise, your motor pulley should be flipped 180 degrees and the motor mount should be scooted a little closer to the wheel pulley to avoid unnecessary lateral pressure on the motor shaft.

A single 9mm will slip when hard braking/accelerating. You'll have to tighten it quite a bit to get it to not slip. An idler will also solve this issue. I wouldn't recommend going smaller than 12mm for a single drive.

You should post your VESC/ESC settings so we can see where you might have an issue. Are you discharging through a BMS? Do you have pictures of the internal components?
```

---
## \#3 Posted by: trancejunkiexxl Posted at: 2017-06-01T01:21:39.817Z Reads: 224

```
man, i feel really dumb could u help me with visualization of its correct position, I am pulling an internal pic now
```

---
## \#4 Posted by: Hummie Posted at: 2017-06-01T01:23:06.993Z Reads: 224

```
Does the motor still get hot even though with lame torque?  Maybe, probably, possibly internal partial short...from pulling the wires so much.
```

---
## \#5 Posted by: Jinra Posted at: 2017-06-01T01:25:02.309Z Reads: 218

```
Super tiny pic, but it works. See how the wires go backwards and loop back to the deck and goes into the enclosure, that's how it should be.

http://reviewlongboards.com/wp-content/uploads/2016/04/enertion-raptor-dual-motor.jpg
```

---
## \#6 Posted by: trancejunkiexxl Posted at: 2017-06-01T01:26:22.213Z Reads: 214

```
the motor is brand new, doesnt seem broken... 
<img src="/uploads/db1493/original/3X/d/0/d067e2dd07187aa1455ae25ef2c5dd4a914d8289.jpg" width="281" height="500">
```

---
## \#7 Posted by: Jinra Posted at: 2017-06-01T01:30:47.348Z Reads: 202

```
VESC settings would be very helpful as well. What's up with the tape wrapped around everything? Are you sure the joints aren't loose? It seems your power switch is unplugged from the antispark module as well.
```

---
## \#8 Posted by: trancejunkiexxl Posted at: 2017-06-01T01:35:10.737Z Reads: 204

```
power switch is fried left it unplugged joints are very fluxed and soldered well and thick, aviation tape was all i had around from my gliders, freaking desperate..
```

---
## \#9 Posted by: trancejunkiexxl Posted at: 2017-06-01T01:49:09.071Z Reads: 199

```
<img src="/uploads/db1493/original/3X/4/1/41b2c043d6373f9052a6fd94244ed1df282634a7.png" width="690" height="350">
```

---
## \#10 Posted by: trancejunkiexxl Posted at: 2017-06-01T01:54:55.098Z Reads: 186

```
is their a setting in mind u can think of that would be responsible. can i run motor max @ 100A or should I stay 80A
my cables are now very short... I can resolder if i must..
```

---
## \#11 Posted by: Jinra Posted at: 2017-06-01T01:57:17.615Z Reads: 184

```
Your battery cutoff is causing an issue for sure. You should have it start at 3.3v/cell at the highest.

Also post your BLDC and advanced tabs.
```

---
## \#12 Posted by: trancejunkiexxl Posted at: 2017-06-01T01:59:24.604Z Reads: 179

```
its a 12s setup does that matter, and its hooked up to bms, in case thats important...
```

---
## \#13 Posted by: Jinra Posted at: 2017-06-01T02:00:44.355Z Reads: 177

```
You're on 18650's ya? You're at 3.58v/cell which will cause problems when you're under high load. If you're discharging through BMS, it could be cutting off if it's not rated for high discharge.
```

---
## \#14 Posted by: trancejunkiexxl Posted at: 2017-06-01T02:01:39.320Z Reads: 173

```
yep 18650's, ok im trying to put this together, im not very smart so thanks for being patient. could u tell me some sample values i could try, for batt cuttoff?
```

---
## \#15 Posted by: Jinra Posted at: 2017-06-01T02:03:59.012Z Reads: 161

```
Try 39v start 36v end.  Also post the other screenshots
```

---
## \#16 Posted by: trancejunkiexxl Posted at: 2017-06-01T02:05:59.667Z Reads: 160

```
tryping and reassembling board, kicking myself for realizing why the motor cables were so long..
```

---
## \#17 Posted by: trancejunkiexxl Posted at: 2017-06-01T02:58:52.041Z Reads: 165

```
<img src="/uploads/db1493/original/3X/8/2/82e67391ef98d2679bdd6c54aa48441b62d4d23f.png" width="690" height="392">


this is before detection,
```

---
## \#18 Posted by: trancejunkiexxl Posted at: 2017-06-01T02:59:11.545Z Reads: 156

```
<img src="/uploads/db1493/original/3X/4/6/4609f00db8ef33bf5c6cd9775f1a414fe4610dec.png" width="690" height="328">
this one is after
```

---
## \#19 Posted by: trancejunkiexxl Posted at: 2017-06-01T03:02:05.985Z Reads: 151

```
<img src="/uploads/db1493/original/3X/0/e/0e76ff3431897a0044e421bfa4ce47f1f8c226d0.png" width="690" height="396">

this should be everything.. as far as motor orientation is im stuck with current setup till I can get replacement wire...
```

---
## \#20 Posted by: trancejunkiexxl Posted at: 2017-06-01T03:06:09.039Z Reads: 146

```
crossing my fingers!!
```

---
## \#21 Posted by: trancejunkiexxl Posted at: 2017-06-01T03:33:56.217Z Reads: 138

```
if you have any other ideas, they are much appreciated, ill be spending the majority of my time, trying to get things running smoothly

tomorrow i will post a video of the intermittant power loss at medium speed so you can see what I am referring to. I might make a 20min drive to buy some new connections and resolder everything.. i already had to resolder the rx cable on my vesc =/
```

---
## \#22 Posted by: Jinra Posted at: 2017-06-01T03:35:27.058Z Reads: 135

```
Settings look good. How about the app config tabs.
```

---
## \#23 Posted by: trancejunkiexxl Posted at: 2017-06-01T03:37:47.224Z Reads: 134

```
<img src="/uploads/db1493/original/3X/b/2/b248b120ec5039f2d168d4464094188114989bd5.png" width="690" height="354">
```

---
## \#24 Posted by: Jinra Posted at: 2017-06-01T03:41:17.200Z Reads: 127

```
ppm as well
```

---
## \#25 Posted by: trancejunkiexxl Posted at: 2017-06-01T03:43:31.049Z Reads: 132

```
<img src="/uploads/db1493/original/3X/d/6/d65f2114bc30e1b037d072455caf6626e1fff79d.png" width="690" height="416">
```

---
## \#26 Posted by: trancejunkiexxl Posted at: 2017-06-01T03:45:22.683Z Reads: 127

```
its crazy how just jumping up one motor size can be so difficult..
```

---
## \#27 Posted by: trancejunkiexxl Posted at: 2017-06-01T04:16:24.952Z Reads: 123

```
If there is a way to test I will try it, I have a spare vesc but there is no firmware on it and I dont have stlink
```

---
## \#28 Posted by: trancejunkiexxl Posted at: 2017-06-01T15:08:43.953Z Reads: 123

```
hey so this mornings run was pretty good!!! belt slippage is insane!! super depressed about this as i bough a whole bunch of HTD 280-5M.. if i go 12mm what is the belt size?
```

---
## \#29 Posted by: Jinra Posted at: 2017-06-01T15:22:33.614Z Reads: 122

```
You could try tightening it up a bit. Not sure what you're asking about belt. You'd use the same belt length just 3mm wider (280-5m-12)
```

---
## \#30 Posted by: mmaner Posted at: 2017-06-01T15:24:34.639Z Reads: 126

```
I usually run 265-5M-12 for dual motor setups and 265-5M-15 for single motor setups, with matching pulleys.  

http://www.vbeltsupply.com/265-5m-12-synchronous-timing-belt.html
http://www.vbeltsupply.com/265-5m-15-synchronous-timing-belt.html
```

---
## \#31 Posted by: trancejunkiexxl Posted at: 2017-06-01T16:17:58.599Z Reads: 120

```
Thanks guys, I am still experiencing power issues though. the flat portion of the ride was great! Going down hill, i had intermittant power dip, and the motor cliks and hangs under load, ejecting me from the board.. my body really hurts... =/
```

---
## \#32 Posted by: trancejunkiexxl Posted at: 2017-06-01T16:29:13.696Z Reads: 122

```
its like sometimes i apply throttle and i get a response but then sometimes i get a hang... im so confused, until i get a vesc programmer i only have one vesc. if its a power issue can i isolate the problem with a multimeter?
```

---
## \#33 Posted by: trancejunkiexxl Posted at: 2017-06-01T17:54:41.416Z Reads: 120

```
ok so i was riding just now adjusted my pulley and set screws I tried to accelerate and all i heard was "click click click", then im thrown off the board, and my foot is killing me.... feels bad.. im hoping this will go away when i go 12mm, however, im worried about when i apply throttle and it  clicks instead of drives, my last motor did that also.. could this be a problem with the vesc?
```

---
## \#34 Posted by: trancejunkiexxl Posted at: 2017-06-01T17:55:23.352Z Reads: 115

```
or hopefully some setting in bldc...
```

---
## \#35 Posted by: Jinra Posted at: 2017-06-01T18:03:08.973Z Reads: 117

```
keep in mind the remote you're using has reliability issues. You might want to consider getting a different one.
```

---
## \#36 Posted by: trancejunkiexxl Posted at: 2017-06-01T18:30:18.481Z Reads: 109

```
So ditch the nano x remote...I didnt know this could be a remote symptom
```

---
## \#37 Posted by: trancejunkiexxl Posted at: 2017-06-01T18:48:40.730Z Reads: 111

```
Isnt there a setting that will prevent brake If the remote d/c? I think I saw it somewhere in w vid but dont remember ... so applying throttle it clicks now not every time but every other time I punch it decides to hang instead of accelerate?
```

---
## \#38 Posted by: trancejunkiexxl Posted at: 2017-06-01T18:49:49.880Z Reads: 107

```
I think its related as I fall shortly after hearing it and hit the ground
```

---
## \#39 Posted by: longhairedboy Posted at: 2017-06-01T18:55:08.082Z Reads: 108

```
i thought this as well. The enamal could have worn thin from rubbing... just enough to lose power but not enough to put it in a full short.
```

---
## \#40 Posted by: trancejunkiexxl Posted at: 2017-06-01T19:01:42.657Z Reads: 111

```
Its that sensative?.. wow I mean ya I trimmed the cables and changed the connectors but It looks ok.. so earlier I soldered the rx cables back on the vesc as they are thin and connected directly to board, if the soldering isnt perfect this could mess the signal right.. I guess I will order new parts then damn that sux 90$and its broken...how come it only stalls every other time, my previous motor did that also
```

---
## \#41 Posted by: trancejunkiexxl Posted at: 2017-06-01T20:41:28.167Z Reads: 99

```
Ive examined the three cables but cant see anything wrong guess I will order another motor and vesc =(
```

---
## \#42 Posted by: Jinra Posted at: 2017-06-01T23:03:04.594Z Reads: 96

```
Oh you have the nano-x. I'm not sure about the reliability of that one, but the remote it's based off of (the winning remote) is notorious for being unreliable.
```

---
## \#43 Posted by: trancejunkiexxl Posted at: 2017-06-02T00:14:59.750Z Reads: 102

```
will signal loss immediately cause my board to stop riding? im so confused here, I just ordered another vesc im hoping to get this sorted out soon
```

---
## \#44 Posted by: trancejunkiexxl Posted at: 2017-06-02T00:32:38.151Z Reads: 103

```
<img src="/uploads/db1493/original/3X/2/4/24590d6e397b50df6979cfaa8f7724eab830948c.jpg" width="281" height="500"> i soldered them pretty good, I would like to say signal is not my issue...
```

---
## \#45 Posted by: trancejunkiexxl Posted at: 2017-06-02T01:22:36.545Z Reads: 99

```
so i guess i should order a new motor and a spare since they break so easy huh?
```

---
## \#46 Posted by: Hummie Posted at: 2017-06-02T04:25:21.253Z Reads: 95

```
What ever happened to pass the nano?


did the motor pass the vec test?

Try running it while bending the wires maybe. How hot does it get?
```

---
## \#47 Posted by: Jinra Posted at: 2017-06-02T05:19:15.936Z Reads: 93

```
@evoheyax was buying another remote from me and I was supposed to send both to him but I never got the payment. I forgot about it since it's been sitting in storage for so long. Did you want it?
```

---
## \#48 Posted by: Hummie Posted at: 2017-06-02T06:29:03.409Z Reads: 90

```
I guess u don't like it?  I thought it might be nice. I like the trigger I have but thought it might be nice
```

---
## \#49 Posted by: Jinra Posted at: 2017-06-02T06:38:43.828Z Reads: 91

```
The throttle is pretty similar to the winning which is too stiff and short for my taste. Also, if you grip it normally your thumb is not in the position to move the throttle so you have to awkwardly claw grip the controller to use it.
```

---
## \#50 Posted by: trancejunkiexxl Posted at: 2017-06-02T07:29:13.872Z Reads: 97

```
getting another bench wheel diy remote in a week.. assuming its similar to the same generic 2.4ghz tx/rx combo like
http://www.ebay.com/itm/2-4GHz-Radio-Remote-Controller-Receiver-Binding-Plug-For-Electric-Skateboard-/262779892776?hash=item3d2ee6f428:g:G2kAAOSw9GhYYjLd

I ordered another vesc, and will be ordering a motor again tomorrow.. Super frustrated, but ok I will run bldc tomorrow, and motor detection which I believe it will pass like when I first set it up.. like I said, it only hangs every other time I give it throttle, it literally clicks audibly and hangs for a sec or 2, which doesn't sound like a remote issue... but when u ride and this happens the whole board shutters and it slows down rapidly at random parts of ride, like coming through corner... this leads to crash everytime now so I don't know how I can even test it now as my foot is completely swollen...I ordered new belt setup hopefully to combat traction issue... Now the real question is how do I determine if I should throw this motor away or what real problem is?
```

---
## \#51 Posted by: trancejunkiexxl Posted at: 2017-06-02T16:33:03.404Z Reads: 94

```
Wish i had all my parts =( I am ordering extras so this doesnt happen anymore.. So i removed the faulty power button. Its too bad these things are like 60$ =/
<img src="/uploads/db1493/original/3X/b/f/bff2169425daff47f54fe60f4f0a481290ed0091.jpg" width="690" height="388">

i know its not the culprit, but I am just trying to determine which parts work and which ones dont.. OK so it passed motor detection!

https://drive.google.com/open?id=0B1KhCcXEs2BbQ2ZNdWNkQlJpTzA

-https://drive.google.com/open?id=0B1KhCcXEs2BbQ2ZNdWNkQlJpTzA

there is a drive link so you can see my progress.. cables are still a bit cramped, maybe if i shorten them so more I can fix this power issue... =/ once it passed detection, I can only wonder what to look for next....
```

---
## \#52 Posted by: Jinra Posted at: 2017-06-02T16:35:30.206Z Reads: 91

```
If it's just the button that's faulty they're only a couple bucks on amazon/ebay. If the fets are stuck on "always on" though, then you'd have to replace the whole thing.
```

---
## \#53 Posted by: trancejunkiexxl Posted at: 2017-06-02T16:36:00.042Z Reads: 89

```
ya stuck always on... bummer
```

---
## \#54 Posted by: trancejunkiexxl Posted at: 2017-06-02T16:37:02.541Z Reads: 89

```
i think the only way to resolve this is with additional parts to isolate problem, my current vesc works but I cant determine if its getting consistant power, I might need a data logger or something
```

---
## \#55 Posted by: Jinra Posted at: 2017-06-02T16:38:21.964Z Reads: 88

```
That remote is ridiculously cheap. DIYES has it for $60 and I think even the group buy for it that @Michaelinvegas organized was at least twice that price.
```

---
## \#56 Posted by: trancejunkiexxl Posted at: 2017-06-02T16:39:59.085Z Reads: 88

```
[quote="trancejunkiexxl, post:51, topic:24308"]
https://drive.google.com/open?id=0B1KhCcXEs2BbQ2ZNdWNkQlJpTzA
[/quote]

<img src="/uploads/db1493/original/3X/e/b/eb1ce9772792c5205d2d55bca9b2e1006554ce79.jpg" width="281" height="500">

that was my first remote.. it died after 3 rides..
```

---
## \#57 Posted by: Jinra Posted at: 2017-06-02T16:41:10.866Z Reads: 79

```
I have 4 of those which are all still working. How is it dead? Does the light on the receiver not turn on anymore?
```

---
## \#58 Posted by: trancejunkiexxl Posted at: 2017-06-02T16:42:29.297Z Reads: 83

```
correct sir
```

---
## \#59 Posted by: trancejunkiexxl Posted at: 2017-06-02T16:43:23.207Z Reads: 85

```
<img src="/uploads/db1493/original/3X/9/f/9faf6f46ff0a996a0c97f34ad5e4982462e02ed0.jpg" width="434" height="500">

i bought a couple of these. i really like them but not enough to keep using them and getting hurt i wont be able to ride again for at least a week i spilled so hard
```

---
## \#60 Posted by: Jinra Posted at: 2017-06-02T16:44:01.494Z Reads: 82

```
Hm weird, I wonder what killed it. It might sound stupid, but you made sure you plugged the servo into the correct 3 pins right? The 3 pins on the right side of that picture does not power on the unit, only the left 3 do.
```

---
## \#61 Posted by: trancejunkiexxl Posted at: 2017-06-02T16:45:17.851Z Reads: 81

```
ill just show you... i can recreate it!!! my phones dead give me one sec
i plugged in the rx and its doing the bad thing now..im doing a low res vid so you can see this thing. uploading now
```

---
## \#62 Posted by: trancejunkiexxl Posted at: 2017-06-02T16:52:24.149Z Reads: 79

```
-https://drive.google.com/open?id=0B1KhCcXEs2BbMXlKbjJ5LVg3ZTQ

here is a vid of the issue!

so I dont know if this is whats ejecting me from the board
but i think it could be related. something is not quite right...
```

---
## \#63 Posted by: Jinra Posted at: 2017-06-02T16:55:46.835Z Reads: 77

```
Oh you're talking about the other remote. I thought you said you had the nano-x. Anyway, you should be careful throttling like that when your motor cogs or gets stuck, you can burn out your electronics.

It sounds like the VESC's timing is out of sync, but I haven't ran into this issue before. The only thing I can say is to run detection a whole bunch of times and make sure the readings are consistent and entered correctly in BLDC tool, which, from previous posts, looks like they are.
```

---
## \#64 Posted by: trancejunkiexxl Posted at: 2017-06-02T16:59:49.225Z Reads: 78

```
Ah I think someone told me they were clones, who knows lol... they seem nice enough
ya thats very troublesome, as I can barely walk right now haha!! I will switch the vesc then I guess and see if my luck gets better.. Where are these vesc timing settings XD
```

---
## \#65 Posted by: Hummie Posted at: 2017-06-02T17:00:29.858Z Reads: 75

```
you get problems when turning you say?  I still think you likely have an internal short happening.  fiddle with the wires while powering it and see what happens.  the phase wires maybe are shorting to the motor can or sometihing.
```

---
## \#66 Posted by: trancejunkiexxl Posted at: 2017-06-02T17:02:52.330Z Reads: 71

```
it might have been a coincidence the turning thing though... maybe this is a throttle input issue, it seems I cant burst the max signal but I can go up and down easy enough...
```

---
## \#67 Posted by: trancejunkiexxl Posted at: 2017-06-02T17:06:16.020Z Reads: 70

```
ya ive been playing with the input and I need to maybe restrict the top end as long as the motor isnt dead stop I can play with throttle, I just cant gun it or it clicks and fails... this really sucks i would really like to hear more about this VESC timing you speak of, I wonder if this could this be too much signal from the controller?

-https://drive.google.com/open?id=0B1KhCcXEs2BbMXlKbjJ5LVg3ZTQ
```

---
## \#68 Posted by: Hummie Posted at: 2017-06-02T17:14:27.061Z Reads: 72

```
does the motor still get warm?  or hot?  even though you aren't putting much power in?  is it noisier?
```

---
## \#69 Posted by: trancejunkiexxl Posted at: 2017-06-02T17:18:46.880Z Reads: 74

```
ive been running it wot, its sitting on its block right now, feels cold to the touch, motor sounds good and no unusual sounds
```

---
## \#70 Posted by: trancejunkiexxl Posted at: 2017-06-02T17:19:48.151Z Reads: 71

```
its really touchy with this controller, if i use it a certain way i know i wont get spikes... so can i program the remote for this behavior? its like one second pause is necessary before max input or else it spikes
```

---
## \#71 Posted by: Jinra Posted at: 2017-06-02T17:27:05.658Z Reads: 73

```
One more thing I thought of. Since your motor's unsensored. It's probably losing timing when you blast the throttle like that. You have to kick start unsensored motors for them to work properly.
```

---
## \#72 Posted by: trancejunkiexxl Posted at: 2017-06-02T17:36:57.374Z Reads: 75

```
so then this isnt responsible for ejecting me from the board at max speed? there is a long wire that is the sensor wire i believe can i hook it up?
```

---
## \#73 Posted by: Jinra Posted at: 2017-06-02T17:43:05.482Z Reads: 69

```
The remote you're using is the new version of the winning remote. Perhaps it has the same flaws as the original winning remote. I've been ejected from my board by the original winning remote as well. 

Try turning off your remote when your board is on and seeing if it brakes by default.
```

---
## \#74 Posted by: trancejunkiexxl Posted at: 2017-06-02T17:52:50.960Z Reads: 65

```
awesome idea writing that down!! if their is anything else you can think of do let me know Im pretty much working on this full time
```

---
## \#75 Posted by: trancejunkiexxl Posted at: 2017-06-02T18:16:59.956Z Reads: 70

```
when the signal of the remote goes on and off, the remote changes so that when u let go of throttle it immediately brakes!
```

---
## \#76 Posted by: trancejunkiexxl Posted at: 2017-06-02T18:22:52.480Z Reads: 79

```
<img src="/uploads/db1493/original/3X/7/7/7759f373c53b67446d5ce9f6e8b819d576d5ec67.jpg" width="281" height="500">

so the motor has a wire like this but i dont think my vesc has a space for it
```

---
## \#77 Posted by: Jinra Posted at: 2017-06-02T18:23:34.393Z Reads: 80

```
I think you have to reset neutral position of the remote by rebinding. Follow these steps

https://www.electric-skateboard.builders/t/2-4ghz-nano-remote-sold-out/5017/191?u=jinra
```

---
## \#78 Posted by: Jinra Posted at: 2017-06-02T18:24:37.780Z Reads: 82

```
You need this header to fit the VESC.

http://www.ebay.com/itm/JST-2-0mm-PH-6-Pin-Connector-with-Wire-X-10-Sets-TW-/141757606740?hash=item2101696b54:g:W9EAAOSwgQ9V3m4W
```

---
## \#79 Posted by: trancejunkiexxl Posted at: 2017-06-02T18:27:23.263Z Reads: 80

```
OK so i managed to avoid the constant spikes that occur in the input by making these adjustments to the throttle curve... its works!! now i can gun it and not get spikes. .sure there will be latency but maybe i just keep playing with it and im planning on dual motor anyways..
```

---
## \#80 Posted by: trancejunkiexxl Posted at: 2017-06-02T19:11:59.464Z Reads: 80

```
damn ya i dont have those jst connectors.. i should get em cuz their worth it right?
```

---
## \#81 Posted by: Jinra Posted at: 2017-06-02T19:24:17.280Z Reads: 76

```
I always use sensors on my boards.
```

---
## \#82 Posted by: trancejunkiexxl Posted at: 2017-06-02T19:26:18.653Z Reads: 80

```
<img src="/uploads/db1493/original/3X/4/4/448d42060cff6f1b5dfe53c91a38e9db4eb9a064.jpg" width="281" height="500">
can u identify which ports for this vesc =( soo many
```

---
## \#83 Posted by: Jinra Posted at: 2017-06-02T19:27:24.246Z Reads: 82

```
Upper right in that picture. From left to right the ports are

* GND
* Hall sensor
* Hall sensor
* Hall sensor
* TEMP
* 5v
```

---
## \#84 Posted by: trancejunkiexxl Posted at: 2017-06-02T19:29:55.859Z Reads: 83

```
<img src="/uploads/db1493/original/3X/a/4/a4587d69519bf9ba4a8d4bbd723798771d47edbf.jpg" width="690" height="388">

I removed all the kink from the wires and am resoldering them so they cabled will have NO folds whatsoever, I just need to order new radio remotes, so i can do more comparison. Im really liking the custom throttle curve... NO more throttle input spikes when i try to punch it!!! awesome.. I really hope that this isnt some deeper issue i have with my wiring. i took a pic so you can see how i flux and solder my bullet connectors. Yes it is horrible but it should be ok no?
```

---
## \#85 Posted by: Jinra Posted at: 2017-06-02T19:31:32.838Z Reads: 79

```
what do you mean custom throttle curve "no more spikes"? Did you do something?
```

---
## \#86 Posted by: trancejunkiexxl Posted at: 2017-06-02T19:32:15.136Z Reads: 80

```
appconfig - enable acceleration throttle curve
```

---
## \#87 Posted by: trancejunkiexxl Posted at: 2017-06-02T19:33:05.455Z Reads: 83

```
<img src="/uploads/db1493/original/3X/f/e/fe8745fa5a782735f4dcebee97469d979d5ce454.jpg" width="690" height="388">

i tried playing with the brake one but the vesc kept rebooting!! super weird.. the throttle works great now though
```

---
## \#88 Posted by: trancejunkiexxl Posted at: 2017-06-02T19:35:45.848Z Reads: 78

```
now when i punch it, it accelerates nice and smooth. I will be adding a startup boost from the advanced tab as well, I hear that can help slow starts as well..?
```

---
## \#89 Posted by: Jinra Posted at: 2017-06-02T19:38:20.155Z Reads: 77

```
starupboost = minimum duty cycle when you throttle

It helps with non-sensored setups to not cog when you start. Don't raise it to more than .15
```

---
## \#90 Posted by: trancejunkiexxl Posted at: 2017-06-02T19:40:37.209Z Reads: 78

```
might be a good short term solution till i can sort out the jst connector for the 6 pin, i am confused on that for sure
```

---
## \#91 Posted by: longhairedboy Posted at: 2017-06-02T19:40:58.848Z Reads: 82

```
i think i have mine set to .07 with the sensors. IT helps if you like doing burnouts on launch. lol
```

---
## \#92 Posted by: trancejunkiexxl Posted at: 2017-06-02T19:42:23.758Z Reads: 82

```
good to know, im waiting for parts to dual motor this board does not have enough space sadly, so I will be getting a bigger board
```

---
## \#93 Posted by: trancejunkiexxl Posted at: 2017-06-02T19:42:51.512Z Reads: 88

```
i dont like having to fold cables a million times over to close the lid<img src="/uploads/db1493/original/3X/0/3/03c17aa63a87eca77100a2ed300c2ab1dd734e54.jpg" width="281" height="500">

this is how im soldering just so you have an idea of how bad im doing haha! i generally go over it again till i get it bonded on all sides and just kinda paint it on =/
```

---
## \#94 Posted by: longhairedboy Posted at: 2017-06-02T19:57:31.232Z Reads: 85

```
you can get a much cleaner joint by tinning with a solder pot first

https://www.amazon.com/Solder-Soldering-Desoldering-Capacity-Station/dp/B00RLDQCC4/ref=sr_1_1?ie=UTF8&qid=1496433368&sr=8-1&keywords=solder+pot

you'll also want  bar of solder
https://www.amazon.com/50-Lead-Solder-Made-RotoMetals/dp/B001QUZ6XE/ref=sr_1_1?ie=UTF8&qid=1496433422&sr=8-1&keywords=solder+bar+50%2F50

you'll have it for a while.

oh and don't forget a small bottle of flux. 
https://www.amazon.com/Kester-Rosin-Soldering-Bottle-Clean/dp/B01MR49JY1/ref=sr_1_1?ie=UTF8&qid=1496433479&sr=8-1&keywords=bottle+of+flux
```

---
## \#95 Posted by: Jinra Posted at: 2017-06-02T20:00:10.128Z Reads: 84

```
TIL of a soldering pot. I've just been tinning with my iron, but I suppose this makes it easier if you're doing a lot of wires.
```

---
## \#96 Posted by: trancejunkiexxl Posted at: 2017-06-02T20:24:48.707Z Reads: 85

```
i realize that the joints are not optimal, i will just have to practice and get shrink wrap lol
```

---
## \#97 Posted by: trancejunkiexxl Posted at: 2017-06-02T20:46:01.213Z Reads: 88

```
hey id like to see how u do your work, if u got a vid show me sometime
```

---
## \#98 Posted by: Tuomalar Posted at: 2017-06-02T20:50:40.873Z Reads: 86

```
I recommend you to cut all phase wires as short as shortest and solder new longer (15cm) wires.I personally wouldn't use those banana connectors. I prefer these ones: https://hobbyking.com/en_us/polymax-4mm-gold-connectors-10pairs-set.html
```

---
## \#99 Posted by: trancejunkiexxl Posted at: 2017-06-02T21:58:02.902Z Reads: 87

```
it kinda helped but, im still getting intermittant power some times when i gun it, i also just crashed now so I know whatever i got is working but not that great

as soon as i have new vesc and ubec and pieces i am going to try again i guess
```

---
## \#100 Posted by: trancejunkiexxl Posted at: 2017-06-02T22:00:12.287Z Reads: 86

```
seems the motor runs fine, just sometimes im cogging or stalling how do you troubleshoot this, i am going to order those connectors asap
```

---
## \#101 Posted by: trancejunkiexxl Posted at: 2017-06-02T22:02:49.525Z Reads: 83

```
seems i found some in with my things I will probably do this swap tonight
```

---
## \#102 Posted by: trancejunkiexxl Posted at: 2017-06-03T00:18:21.722Z Reads: 84

```
<img src="/uploads/db1493/original/3X/9/c/9c6fc513f0342d756ffd93869d8ea2d28c4a88c5.jpg" width="281" height="500"> ditched the small connectors for these big guys, sux i cant use new cable solder gun aint hot enough
```

---
## \#103 Posted by: trancejunkiexxl Posted at: 2017-06-03T00:19:47.808Z Reads: 80

```
<img src="/uploads/db1493/original/3X/2/e/2ee268ca8ac1973202029c02b53dae7d5f3c7620.jpg" width="281" height="500">should be zero kinks as i have no wire left all the way down the motor!!!

fyi the throttle adjustments kinda helped but  still sometimes when i accelerate it just stalls and throws me so, im going to re do all the connections
```

---
## \#104 Posted by: Jinra Posted at: 2017-06-03T00:28:35.724Z Reads: 79

```
wait a minute, where did you get this VESC? It looks.. different.. The phase wires are attached to the middle instead of the end with the fets?
```

---
## \#105 Posted by: trancejunkiexxl Posted at: 2017-06-03T00:32:11.621Z Reads: 80

```
https://miamielectricboards.com/shop-1/vesc

think it should be OSEC i dono
 this is a single vesc not a double in the pic
```

---
## \#106 Posted by: Jinra Posted at: 2017-06-03T00:33:53.195Z Reads: 80

```
huh weird, never seen a vesc iteration that looks like that. What do you mean it "stalls" when you accelerate? Like how it acted in the video?

Is this happening when you're already moving on the board? Or from dead stop?
```

---
## \#107 Posted by: trancejunkiexxl Posted at: 2017-06-03T00:38:22.146Z Reads: 80

```
while im moving
```

---
## \#108 Posted by: trancejunkiexxl Posted at: 2017-06-03T01:12:01.777Z Reads: 78

```
ok so the solder job was good! got it back together going for a quick spin on default with no controller curve
```

---
## \#109 Posted by: trancejunkiexxl Posted at: 2017-06-03T01:17:53.669Z Reads: 77

```
and its KO!!! vesc went up in smoke.. probably for the best... just another week delay lol, ive spent more time soldering then riding haha
```

---
## \#110 Posted by: trancejunkiexxl Posted at: 2017-06-03T05:02:45.005Z Reads: 78

```
 the vesc i have is much smaller and usb 2.0 instead of the vesc 4.12 which is usb 1.0 and does not fit in the electronic housing of my current board,
```

---
## \#111 Posted by: Eboosted Posted at: 2017-06-04T05:26:58.650Z Reads: 84

```
Hello, I read you whole thead and saw you video.

Your problem is the lack of sensors and a bad detection, here is what I'd do:

1. Go to Motor Configuration Motor and set battery cutoff start to 36v, battery cutoff end 33v

2. Connect the sensor cables on the VESC

Optional hall-sensors or pulse encoder connector:
[img]http://vedder.se/wp-content/uploads/2015/01/PCB_Front.png[/img]

3. Go to Motor configuration BLDC tab and click on 
start detection"

4. After it stops spinning, you will see on the detection results window the hall sensors order, "hall sensores detected"

5. Click on Sensor mode: Hybrid, click "apply" and then "write"

6. Unplug the USB cable

7. Place an order for at least 3 x 12mm belts and a 12mm pulley from @torqueboards tight them enough until you have no belt slippage, you could also get 15/40T 15mm pulleys from @Titoxd10001, 15mm pulleys won't slip at all unless you tight them extremely loose.

8. Turn around 180 degrees that motor the cables will be pulled out as soon as you start carving.

9. Get tin from amazon, your solder joints are pretty bad, tin would give you a much better finish

10. Get heat wrap to isolate the cables after you solder them

11. As soon as you can get a second motor, it's worth every single penny, braking is much safer and the pushing from stand stills are amazing, so you a lot more control on hard accelerations.

Hope I was able to help
```

---
## \#112 Posted by: trancejunkiexxl Posted at: 2017-06-04T05:29:21.018Z Reads: 77

```
thank you for this valuable information, as soon as I get my parts I will continue my progress on here... I am very curious on how to route the cables after orienting the motor this way..I wish I could see a better example
```

---
## \#113 Posted by: trancejunkiexxl Posted at: 2017-06-09T05:17:58.909Z Reads: 71

```
board is working, still waiting for sensor wires...
```

---
## \#114 Posted by: trancejunkiexxl Posted at: 2017-07-03T16:41:44.993Z Reads: 66

```
So far so good... what would you suspect motor max for 6355 is, and Use Max Watt should I be using this mode? I would like to run slightly aggressive settings for bldc..
```

---
## \#115 Posted by: trancejunkiexxl Posted at: 2017-07-03T16:42:51.746Z Reads: 63

```
i should also note no cogging since installing sensor wire, will be doing some tests today, I definitly feel like the motor has more power though, where do I go for that
```

---
## \#117 Posted by: Eboosted Posted at: 2017-07-03T19:25:57.881Z Reads: 62

```
That's good to know. Now it's your turn to help other members with the same issue
```

---
## \#118 Posted by: trancejunkiexxl Posted at: 2017-07-03T19:45:07.456Z Reads: 62

```
Absolutely 100% with you on that... almost having broke my foot a couple of times, I really want to prevent people from getting hurt... **BLDC settings are absolutely critical for a **safe ride.** I had a false sense of "security" while riding with my current configuration which was a bad call to ride on.** This was my own fault, and it could have been avoided had I the patience to wait for other members to help me...

* I am still looking for optimal BLDC settings so I can do a rolling hard-launch** But the board is now stable on the top end..
```

---
## \#119 Posted by: trancejunkiexxl Posted at: 2017-07-11T16:30:21.335Z Reads: 57

```
<img src="/uploads/db1493/original/3X/c/0/c0510eb747ad56d39b3388e59b9a73308367ceff.png" width="690" height="306">
```

---
