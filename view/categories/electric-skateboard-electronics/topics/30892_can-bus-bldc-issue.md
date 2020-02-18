# Can bus / BLDC issue

### Replies: 54 Views: 2556

## \#1 Posted by: L3chef Posted at: 2017-08-17T15:31:43.543Z Reads: 176

```
A month ago I shorted the canbus receiver on my 4.10 vesc. Since then I have replaced the chip.
Now when I try to connect dual vesc´s via canbus I get the fail message "No firmware read response" and the vesc disconnects. This happens as soon as I check the Can FWD box.



What I have tried : 

- Both vesc as master and slave
- Installed st link drivers
- Different usb cable
- Different CANBUS cable


I´m not sure what to try next. Would appreciate some help here.

Regards
```

---
## \#2 Posted by: JLabs Posted at: 2017-08-17T15:34:15.413Z Reads: 168

```
What are you using CAN FWD for? You can run VESC’s via can without forwarding. I was told that you should use that unless there is something specific to use it for and that it was very risky.
```

---
## \#3 Posted by: L3chef Posted at: 2017-08-17T15:39:29.829Z Reads: 163

```
To check if they are communicating. The master vesc´s motor  is only rotating
```

---
## \#4 Posted by: evoheyax Posted at: 2017-08-17T17:00:06.962Z Reads: 156

```
On the master: under ppm, check the box for enable multiple vesc's over canbus, and on the slave: on the app tab, check the box for send status over canbus. Make sure the id in the app tab is different for each vesc. for simplicity and this example, set master to 0 and slave to 1.  Now, plug into master, click connect, before you check the box for connecting over canbus, make sure the number is on 1, and check the box. It should connect then.
```

---
## \#5 Posted by: L3chef Posted at: 2017-08-17T17:06:20.626Z Reads: 139

```
Yup tried it again as you explained. Still no go :confused:
```

---
## \#6 Posted by: Namasaki Posted at: 2017-08-17T17:10:03.027Z Reads: 133

```
If it still doesn't work you could ditch the canbus cable. 
Get a Y ppm splitter and run both Vescs as masters. 
Only feed 5v from one Vesc to the receiver though. 
You have to clip the red wire on one leg of the splitter.
```

---
## \#7 Posted by: L3chef Posted at: 2017-08-17T17:12:14.575Z Reads: 132

```
Yeah I have been running split servo for couple of months now. But I would like to try out @Ackmaniac ´s monitor app. And therfor I need canbus to work so I can get data from both vesc´s right?

Still learning.

thanks for your help
```

---
## \#8 Posted by: evoheyax Posted at: 2017-08-17T17:13:21.393Z Reads: 131

```
If you have a multimeter, another way to check is to turn off your vescs, and check the pins on the back of vesc's canbus port. The middle two should be connected one and one, but not to each other. You should not get a cross signal, just pin 2 to pin 2 and pin 3 to pin 3 should be connected. If that shows them connected, could be a malfunction in one of the vescs.

So

X X
X--X
X--X
X X
```

---
## \#9 Posted by: Namasaki Posted at: 2017-08-17T17:15:08.658Z Reads: 120

```
I run a BT module with monitoring app. 
I just monitor one Vesc and assume that the other is the same or close enough.
```

---
## \#10 Posted by: L3chef Posted at: 2017-08-17T17:19:30.286Z Reads: 120

```
I will try that now.. need to remove some glue first. 
Should the multimeter be in "diode" mode?
```

---
## \#11 Posted by: L3chef Posted at: 2017-08-17T17:20:35.161Z Reads: 122

```
hehe It´s bothering me too much for letting it be. need to fix it :smiley:
```

---
## \#12 Posted by: evoheyax Posted at: 2017-08-17T17:21:18.970Z Reads: 124

```
I'm not sure what the modes called, but if you ouch the 2 leads together, it'll beep until you break the circuit. Only 1 mode that does it, so you'll find it, haha
```

---
## \#13 Posted by: L3chef Posted at: 2017-08-17T17:22:38.610Z Reads: 125

```
<img src="/uploads/db1493/original/3X/f/3/f35ef05bd3701d4b182a73703d4ac9d6503b24da.jpg" width="500" height="500">

This is the cheap meter I got. Updating how it goes
```

---
## \#14 Posted by: Namasaki Posted at: 2017-08-17T17:37:34.531Z Reads: 117

```
[quote="L3chef, post:11, topic:30892"]
hehe It´s bothering me too much for letting it be. need to fix it :smiley:
[/quote]

I can relate to that.
```

---
## \#15 Posted by: L3chef Posted at: 2017-08-17T17:51:11.627Z Reads: 118

```
Didn´t find a beeping mode on my m.m
But when reading 200 ohm it measure ~ 42.0 on both can low and high.
```

---
## \#16 Posted by: L3chef Posted at: 2017-08-18T09:14:30.656Z Reads: 111

```
Still no solution. Is there a way to check individuell vesc for can bus communication?
```

---
## \#17 Posted by: Namasaki Posted at: 2017-08-18T09:19:56.362Z Reads: 112

```
doesn't the diode test beep?
```

---
## \#18 Posted by: L3chef Posted at: 2017-08-18T09:28:20.342Z Reads: 109

```
My multineter doesn't beep to my knowledge
```

---
## \#19 Posted by: L3chef Posted at: 2017-08-18T13:27:19.660Z Reads: 105

```
Diod test is reading 075 on both pinns
```

---
## \#20 Posted by: DanSkates Posted at: 2017-08-18T13:37:22.222Z Reads: 106

```
Hi @L3chef sorry to hijack your thread - I'm just in the process of figuring out how to replace the canbus chip on my FOCBOX as per this topic [here](https://www.electric-skateboard.builders/t/have-i-focked-my-focboxs/30428/19)

Any advice you can give towards finding the correct chip and the method you used?  Those things are bloody tiny!!

Thanks
```

---
## \#21 Posted by: L3chef Posted at: 2017-08-18T13:55:17.681Z Reads: 101

```
No worries. Hijack away :slight_smile:
 I don´t know what chip FOCBOX use but probably the same as 4.12. You should check with the store you got it from.
I replaced the chip with a regular soldering iron. With a pointy tip. Remove the broken chip and clean up the pcb, get some solder to the 8 pinns on the chip and place it in it´s position. Hold it down with something so it doesnt move. and go over the pinns with the iron one by one. Just be careful and it will be over in 5 min :smile: 

Hot air soldering would probably be a better way to do it tho...

Good luck
```

---
## \#22 Posted by: DanSkates Posted at: 2017-08-18T14:02:05.000Z Reads: 98

```
[quote="L3chef, post:21, topic:30892"]
Just be careful and it will be over in 5 min :smile:
[/quote]

Sounds a lot like my love life!!! :joy:

Thanks for the advice - it doesn't seem like it should be two hard...famous last words!  Just looked and the chip appears to be very similar - can I ask where you sourced it?  Thanks man - hope you find a solution to your problem too.
```

---
## \#23 Posted by: L3chef Posted at: 2017-08-18T14:12:00.323Z Reads: 96

```
hahahah :smiley:

It´s not hard at all. Just need to be careful so you don´t poke any components that is close to the chip with the iron. I bought mine from @Martinsp  here on the forum :slight_smile:
```

---
## \#24 Posted by: DanSkates Posted at: 2017-08-18T14:13:59.151Z Reads: 94

```
Legend - I'll give it a go and pm @Martinsp separately - I'll let you know how I get on! :muscle:
```

---
## \#25 Posted by: L3chef Posted at: 2017-08-18T14:49:00.507Z Reads: 93

```
If you decide to replace them yourself you can always start with removing the can receiver befor ordering the parts.
When the chip is removed the esc should power on. If it doesn´t. something else is wrong.
```

---
## \#26 Posted by: DanSkates Posted at: 2017-08-18T14:52:35.152Z Reads: 88

```
Holeee shit - I hadn't realised that.  I'll do that for sure!  Hey, if that's the case could I then just use another method (like split Y) to connect them for the time being as you mentioned at the start of this topic?
```

---
## \#27 Posted by: L3chef Posted at: 2017-08-18T14:54:40.871Z Reads: 85

```
That´s what I have been doing since for ever :stuck_out_tongue:
Many riders prefer split servo insted of can bus
```

---
## \#28 Posted by: DanSkates Posted at: 2017-08-18T14:58:07.299Z Reads: 82

```
Wow - you may just have got me back on my board - I'll feedback when the sun comes up if it works - it's nearly 1am here and I've spent the last 2 hours searching for canbus chips!!! :grin:  Thanks again.
```

---
## \#29 Posted by: Namasaki Posted at: 2017-08-18T17:08:53.643Z Reads: 78

```
http://www.mouser.com/Search/m_ProductDetail.aspx?Texas-Instruments%2fSN65HVD232DR%2f&qs=%2fha2pyFaduiSwNSNMapJZOp5DAyrO2K%2fCQstQslsB94obQk%2fsWfaHA==
```

---
## \#30 Posted by: L3chef Posted at: 2017-08-18T17:12:29.856Z Reads: 80

```
Lol I checked mouser a month ago for that chip.. All out of stock and would get new batch january..2018. 
:slight_smile:
```

---
## \#31 Posted by: Namasaki Posted at: 2017-08-18T18:14:15.099Z Reads: 80

```
A split PPM cable in your future I see.
```

---
## \#32 Posted by: DanSkates Posted at: 2017-08-21T12:50:46.161Z Reads: 79

```
@L3chef you little ripper!!!!  

Unsoldered both chips and the FOCBOXs sprung back to life!!!  Split PPM cable in the post so I'll be up and running again by the end of the week!  Massive thanks for the heads up buddy!

<img src="/uploads/db1493/original/3X/c/9/c981c754615272fb96cfaa6d2bafc2a83147dbe6.jpg" width="304" height="207">
```

---
## \#33 Posted by: L3chef Posted at: 2017-08-22T06:00:44.314Z Reads: 71

```
Hell yeah :smile: happy riding mate!
```

---
## \#34 Posted by: L3chef Posted at: 2017-08-29T15:54:54.074Z Reads: 65

```
So got a new vesc 4.12.. Still no luck with can bus.
Anyone? Master : 
<img src="/uploads/db1493/original/3X/5/1/517ad4f0d0b63f7d5ed601a35f2b866ef9036308.png" width="371" height="500">
<img src="/uploads/db1493/original/3X/9/8/984eb4098f6b065bb219fa4ee2bd92d855cb911a.png" width="371" height="500">

Slave has same settings except other ID and "send status over can" disabled
```

---
## \#35 Posted by: L3chef Posted at: 2017-08-29T15:55:20.635Z Reads: 59

```
well that´s one way to post tiny pics I guess.
```

---
## \#36 Posted by: Jinra Posted at: 2017-08-29T15:57:35.942Z Reads: 57

```
Fix your screenshots mate. Also slave should have "send status over can" **enabled** and master should have it **disabled**. "multiple escs over can" should also be **enabled** on the master.
```

---
## \#37 Posted by: L3chef Posted at: 2017-08-29T16:01:16.280Z Reads: 57

```
YEah don´t know what happened :stuck_out_tongue: 
Sry I misspelled it. Slave vesc has "send status over can" **enabled** and master does not.

Multiple escs over can is enabled on th emaster
```

---
## \#38 Posted by: Jinra Posted at: 2017-08-29T16:07:23.776Z Reads: 57

```
you made sure you plugged in the canbus connection correctly?
```

---
## \#39 Posted by: L3chef Posted at: 2017-08-29T16:08:39.239Z Reads: 55

```
Yes I tried 2 different cables. only Can L and H connected (two pinns in the middle)
```

---
## \#40 Posted by: L3chef Posted at: 2017-08-29T16:24:17.878Z Reads: 56

```
Is there a way where I can check individual vesc´s can bus if it work´s or not?
```

---
## \#41 Posted by: Ackmaniac Posted at: 2017-08-30T09:20:19.296Z Reads: 51

```
Are you sure that when you enable CAN Fwd that you also select the right controller ID of the slave VESC?
```

---
## \#42 Posted by: L3chef Posted at: 2017-08-30T09:54:15.224Z Reads: 51

```
Yes. As soon as I click can fwd with the right id, it disconnects with error "no firmware read response"  or something like that
```

---
## \#43 Posted by: Ackmaniac Posted at: 2017-08-30T09:54:52.668Z Reads: 51

```
Then it is a hardware issue.
```

---
## \#44 Posted by: L3chef Posted at: 2017-08-30T09:56:09.377Z Reads: 50

```
Thank you for confirming that! Most likely it's the can chip right?
```

---
## \#45 Posted by: GrecoMan Posted at: 2017-08-30T10:07:45.192Z Reads: 49

```
If that ends up being the issue just go the split ppm or dual recievers. Those don't require a working can chip
```

---
## \#46 Posted by: L3chef Posted at: 2017-08-30T10:13:26.717Z Reads: 54

```
Thanks for you suggestion mate. I've been splitting y servo for several months now. The reason I wan't can bus to work, is so I can use @Ackmaniac awesome monitor app and swap between modes when needed.
```

---
## \#47 Posted by: Ackmaniac Posted at: 2017-08-30T10:15:23.994Z Reads: 51

```
In theory you can also use 2 bluetooth modules but then you need to connect to them individually and adjust the same modes for both. Too stressfull if you ask me.
```

---
## \#48 Posted by: GrecoMan Posted at: 2017-08-30T10:15:41.427Z Reads: 52

```
Oh I see.  You definitely need canbus for that. Maybe post a picture of the CAN connector and how your plugging the cable in? Alot of people on here can recognize if something is shorted by just looking at a picture
```

---
## \#49 Posted by: L3chef Posted at: 2017-08-30T10:18:19.286Z Reads: 55

```
Sure. I post some pics later on today :slight_smile:
 @Ackmaniac yeah that's plan C. :smile: I will try to swap out the can receiver  first.
```

---
## \#50 Posted by: STREETSURFER Posted at: 2017-09-21T18:57:35.916Z Reads: 48

```
@L3chef Did you ever figure out what the issue was. Did a new canbus chip fix your issues? I'm getting the same no firmware read response issue as soon as I click the fwd can button. The issue is that I was originally running split ppm with the signal wire soldered to the board, but the signal wire got pulled out tearing the contact off. So running can bus is my only option unless there is a different spot on the board that I can solder my ppm singal wire to.
```

---
## \#51 Posted by: L3chef Posted at: 2017-09-22T04:02:07.328Z Reads: 42

```
No I didn't theres some other components on the vesc that is damaged aswell. In a couple of weeks when it's too cold to ride anymore, I will start to swap out the canbus components untill it works again
```

---
## \#52 Posted by: StormTrooperBert Posted at: 2017-09-28T01:04:57.397Z Reads: 38

```
Where can I get a Y piece?
```

---
## \#53 Posted by: Namasaki Posted at: 2017-09-28T21:56:01.605Z Reads: 37

```
I Like these but there are cheaper ones on eBay 

https://www.amazon.com/gp/product/B0015H2UR8/ref=oh_aui_detailpage_o03_s00?ie=UTF8&psc=1
```

---
## \#54 Posted by: StormTrooperBert Posted at: 2017-09-28T21:57:17.800Z Reads: 37

```
Awesome!! Thanks man!!
```

---
