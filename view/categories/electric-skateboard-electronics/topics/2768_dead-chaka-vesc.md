# Dead Chaka VESC

### Replies: 34 Views: 3831

## \#1 Posted by: cmatson Posted at: 2016-05-01T03:29:05.536Z Reads: 254

```
I made a youtube video explaining it, and will link it below- the youtube video may still be processing if you catch this thread early, but I wanted to go ahead and get this up so I can start troubleshooting and documenting the process. @chaka 

**summary:** Road about 10-12 miles today. 2/3 or so with @longhairedboy in the morning, and then went for another couple miles before sundown when it gets slightly less hot here in FL. After stopping, changing some camera settings, and then starting back up, the board just stopped within 300 yards of my ride resuming. The reasonI mention this is because while I changed camera settings for 5ish minutes, you would think the VESC could cool a little, and therefore heat wouldn't have been the issue- not to mention I road it way harder with LHB in the morning.  Space Cell was fine and at about 35%, but I got no throttle response, and my GTB2 light was blinking, showing that the receiver disconnected. 

The rest is shown in the video: 
https://youtu.be/NKJ95Hi1aEI

of course, right when I sell my two unused ESC's, Enertion's VESC's get super delayed, and my chaka one dies- 

I'm officially eboardless for the next month or so..

 yet I have 4 motors, 3 18650 packs, remotes, wheels, and basically everything I need to make 3 completes except **VESC's**

fun times for sure :disappointed_relieved:
```

---
## \#2 Posted by: chaka Posted at: 2016-05-01T03:33:00.280Z Reads: 237

```
Check your xt connector for cold joints.
```

---
## \#3 Posted by: cmatson Posted at: 2016-05-01T03:34:31.280Z Reads: 229

```

will do that tomorrow-  it's 11:30 here, and my dad would (literally) shoot me if I opened the garage door at this time of night. 

appreciate it man.
```

---
## \#4 Posted by: chaka Posted at: 2016-05-01T03:35:31.865Z Reads: 222

```
Let me know either way. We'll get it sorted out ;)
```

---
## \#5 Posted by: Michaelinvegas Posted at: 2016-05-01T03:42:43.001Z Reads: 217

```
Bro you're hard core.... Head Lamp it! 🔦
```

---
## \#6 Posted by: barajabali Posted at: 2016-05-01T04:06:26.868Z Reads: 210

```
strange popping sound , flashing lights these sound like symptoms of a broken solder joint in my eyes.  where you riding in a particularly bumpy place?
```

---
## \#7 Posted by: lox897 Posted at: 2016-05-01T12:02:42.353Z Reads: 197

```
Get your stealthy red shoes on, that way you can be stealth and go 20% faster.
```

---
## \#8 Posted by: cmatson Posted at: 2016-05-01T13:07:21.719Z Reads: 197

```
Looks like the xt60 joints are ok.. <img src="/uploads/db1493/original/2X/7/7a3b7f1b2458b848bc698fa937f9239a89a2be2e.jpg" width="690" height="388"><img src="/uploads/db1493/original/2X/f/f23c2577b5505b3562a701885dc451983f8f7c2d.jpg" width="690" height="388"><img src="/uploads/db1493/original/2X/d/d397c06c7e80f0978dfb5a6c9423fc8fa68df3b5.jpg" width="690" height="388">

Also, I've been using that xt60 -> 12gauge -> 10 gauge -> VESC ever since I first got the VESC, and had to fit it in my crammed wood arbor box. At first, I accidentally cut too much off the 10gauge, so I soldered little pieces of 12 on there before throwing back on the xt60. The space cell uses 12gauge, so it's not going to be a bottleneck.
```

---
## \#9 Posted by: chaka Posted at: 2016-05-01T14:24:04.427Z Reads: 190

```
Time to bring out a multimeter and check your power source. Something is definitely going on with those cables judging by your video.  Since you a hearing a little pop every time means you have a bad connection somewhere upstream from the capacitor.

Soldering these fat cables requires a big soldering iron, 80 watts at least to do a good job. You also need some good flux, I use Kester 186. You can find small bottles on ebay for cheap if you don't want to buy a gallon of it.

Of course you can send the vesc back for repair but I really think it is a cable issue here.
```

---
## \#10 Posted by: chaka Posted at: 2016-05-01T14:29:15.970Z Reads: 188

```
You should also check the solder pads on the vesc to be sure the cables have not lifted.
```

---
## \#11 Posted by: cmatson Posted at: 2016-05-01T15:07:46.889Z Reads: 188

```
solder pads look fine. I soldered this with a Hakko- it looks ugly, but the connections are strong and the solder goes all the way through the wire. 
 
I uploaded another video testing the voltage of the wires after the capacitor array: it's showing 36v just like the space cell. 

https://youtu.be/SKjD6C49k3c
```

---
## \#12 Posted by: chaka Posted at: 2016-05-01T15:44:53.934Z Reads: 182

```
The only thing I can  think of is the solder joint at the PCB has failed. If you want to send it in for repair I will take care of it for you.
```

---
## \#13 Posted by: EnderWiggin Posted at: 2016-05-01T22:48:10.972Z Reads: 175

```
You could ask the inventor himself! He lives in europe so you will have to get on late at night but there are very knowledgeable people on the chat that might be able to help. He might help you out. When i talked to him it was really late. I think something failed you just dont know what. 
http://webchat.freenode.net/?channels=vedder
```

---
## \#14 Posted by: cmatson Posted at: 2016-05-01T23:28:40.905Z Reads: 173

```
Orson Scott card, eh? Hell of a novel, ender's game was. 

I got it all handled out with Chaka- he haas by far the best VESC customer service out there right now. 

Thanks for the help though!
```

---
## \#15 Posted by: longhairedboy Posted at: 2016-05-02T13:44:48.280Z Reads: 169

```
worst case you'll have to ride my rat board for the May ride. Its plenty ornery enough. But i think you'll have a fix or replacement from @chaka by then for sure if you send it off now. I was hoping we'd both be on 10S so we can show those spandex clad cyclist hoards what's up.
```

---
## \#16 Posted by: cmatson Posted at: 2016-05-03T01:57:49.117Z Reads: 162

```
I priority mailed it to Chaka.. hopefully will have a speedy fix. 

I think worst case is I buy a castle 6s esc and get my 6s4p + torqueboards 230kv motor up and running. It would be significantly slower than the rat board though.. 

I really wanted to bring my bro to the ride though! Haha it kills me to see hubs, three batteries, 2 motors, remotes, boards, wheels, and LITERALLY everything I need for 3 boards except VESC's..
```

---
## \#17 Posted by: onloop Posted at: 2016-05-03T02:19:25.872Z Reads: 161

```
[quote="cmatson, post:16, topic:2768"]
LITERALLY everything I need for 3 boards except VESC's..
[/quote]

haha, i know how it feels.... 

I got like 30 Raptors sitting here.... no vesc :frowning:
```

---
## \#18 Posted by: longhairedboy Posted at: 2016-05-03T11:28:40.282Z Reads: 154

```
@cmatson  i could have three personal boards running right now too! The feels bro!  It hurts in the feels. 

I've got 5 Ollins coming but only two of them are mine. My shop mocks me! IT MOCKS ME.
```

---
## \#19 Posted by: chaka Posted at: 2016-05-11T17:22:02.202Z Reads: 150

```
Found the problem.

<img src="/uploads/db1493/original/2X/b/b58d68da896f6c4bf64188aadc33636511f19185.jpg" width="666" height="500">

Decided to switch out the cap 2 C18 while I have it on the bench.

<img src="/uploads/db1493/original/2X/d/dfca358516c763757aacf212225e66186f0f858c.jpg" width="666" height="500">

Then it was off to the ultrasonic bath and some conformal coating.

<img src="/uploads/db1493/original/2X/0/0634e738b7c565b1eae190b8140539b6bd9aa48c.jpg" width="666" height="500">

Some fresh cables too!  Ready for final testing and shrink wrap. 

<img src="/uploads/db1493/original/2X/3/38b6fca9e5a72ff61d613c7d4900ba3baf6d6b06.jpg" width="666" height="500">

Should be good to go! @cmatson
```

---
## \#20 Posted by: Randyc1 Posted at: 2016-05-11T20:28:44.018Z Reads: 141

```
That is Great service Chaka !!
```

---
## \#21 Posted by: longhairedboy Posted at: 2016-05-11T21:46:13.446Z Reads: 137

```
just in time. we have a ride in a little over a week. You should fly out here and join us. Or if you rode that 12S6P of yours you might get here quicker.
```

---
## \#22 Posted by: chaka Posted at: 2016-05-11T22:01:15.142Z Reads: 136

```
He should be getting this any day. I finished all my repairs this weekend and sent them home on Monday.
```

---
## \#23 Posted by: cmatson Posted at: 2016-05-11T23:00:23.574Z Reads: 137

```
Just got it back!

Huge shout out to chaka and ollin boards for **by far** the best VESC service avaliable right now: 100% worth the price jump.
```

---
## \#24 Posted by: cmatson Posted at: 2016-05-30T01:25:52.326Z Reads: 124

```
Just wanna mention I finally got around to programming it again with the latest BLDC tool (didn't want to downgrade the firmware only to have 2.18 come out a week later). 

So I'm back in business, and hope to be taking this board with me to Australia in two weeks!
```

---
## \#25 Posted by: treenutter Posted at: 2016-05-30T01:43:04.887Z Reads: 120

```
@cmatson are you and @onloop joining forces in Australia? At least get together for a ride!
```

---
## \#26 Posted by: Dedbny Posted at: 2016-05-30T01:47:25.631Z Reads: 118

```
Where in Aus are you going. Not Sydney.
```

---
## \#27 Posted by: cmatson Posted at: 2016-05-30T02:56:07.007Z Reads: 117

```
Melbourne and Sydney- I'll be there for 5 weeks (roughly half and half between time spent in the two different cities), and willl see if I can get a flight over to Adelaide to see the Enertion HQ. It looks like a round trip to Adelaide from either city will be about 200USD give or take; I just don't know if I will really have enough time to do anything in Adelaide if I fly there and back on the same day... but at the same time I don't want to dive into hotel costs and such with an overnight trip as any deviation from the internship is outa my pocket, and I'm already going to be blowing alot over the course of 5 weeks. 

I'll just have to see how my schedule works out, as I know I will have 3 day weekends but will be working monday through thursday.
```

---
## \#28 Posted by: Dedbny Posted at: 2016-05-30T04:27:06.376Z Reads: 111

```
What are you over here for. studies? Enjoy. Im in Melbourne
```

---
## \#29 Posted by: lox897 Posted at: 2016-05-30T08:47:11.815Z Reads: 110

```
Sick @cmatson

I'm in Melbourne. Are you staying in the city? I am so close to finishing my board. The copper motor wires are a PITA to solder. Had them working for a few weeks and the board was awesome. I got medium grit sandpaper and it didn't work really well. I'll try some higher grit.
```

---
## \#30 Posted by: lox897 Posted at: 2016-05-30T08:48:31.523Z Reads: 109

```
And... my neighbour is getting an Evolve GT in a week. I am gonna have a go on it once he gets it. Can't wait to meet you!
```

---
## \#31 Posted by: cmatson Posted at: 2016-05-30T12:32:05.646Z Reads: 108

```
Yep, @lox897 @Dedbny I'm going to be doing an internship, and working on site at Microsoft.

As I said I'll be working 4 day weeks, so we definitely should go for a ride some weekend or a Friday!
```

---
## \#32 Posted by: Pablo_702 Posted at: 2016-06-18T02:32:54.911Z Reads: 98

```
So glad i ordered a Vesc from @chaka thats what i call excellent customer service, cabt wait to get it tho
```

---
## \#33 Posted by: Pablo_702 Posted at: 2016-06-18T02:40:48.173Z Reads: 97

```
Btw does any one knows the dimensions of ollins vesc with heat sink specially the height?
```

---
## \#34 Posted by: chaka Posted at: 2016-06-18T02:57:09.919Z Reads: 94

```
19mm x 40mm x 110mm

Give yourself some room for the phase wires and battery cables. Glad to have you as a customer! Let me know if you need any other info.
```

---
