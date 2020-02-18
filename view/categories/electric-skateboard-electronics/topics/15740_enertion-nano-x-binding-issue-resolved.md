# Enertion Nano-X binding issue (resolved)

### Replies: 48 Views: 4231

## \#1 Posted by: Schulerbible Posted at: 2017-01-07T01:32:07.170Z Reads: 271

```
Hi guys,

I got my Nano-X weeks ago but could not ride my board due to lack of wheels. I did some try testing on the bench and it worked brilliant. Now, 4 weeks later with no further action in between the remote does not bind anymore! The green LED (TX) and red LED (RX) are flashing continuously. 

When I move the cable from channel 1 to Bind on the receiver, the remote binds immediately. Going back to channel 1 same story as before. 

So, while doing tests I was shaking the receiver a bit and bending the cable back and forth and boom, the remote connects again. Not shaking the cable/receiver and the damn thing flashes forever. So, I really think that something is messed up with the receiver. Maybe some cold solder joints, partially loose cables, etc.. I have not opened the receiver yet but I will do so this afternoon and let you guys know what's going on.

Edit:
Inside the Rx is just a solid PCB. However, I have to bend the connector attached to the pins to get the remote to bind. Doing this on my old GT2E all works fine without any issues ... hmm

Edit2:
When I move the connector up/down the pins on the receiver it connects immediately (max 3-5s). And once it is connected I can move the connector up/down shake the hell out of it, bend it back and forth and the binding is still remains active ... wtf???

Cheers
```

---
## \#2 Posted by: Kaden56 Posted at: 2017-01-07T07:00:33.288Z Reads: 232

```
Sounds to me like the receiver is the problem. I hope they send out new ones quickly if that's the case!
```

---
## \#3 Posted by: lox897 Posted at: 2017-01-07T09:20:51.923Z Reads: 220

```
Please send pictures of the receiver
```

---
## \#4 Posted by: Jebe Posted at: 2017-01-07T10:05:37.243Z Reads: 213

```
I have problems too - I have to remove my receiver from the enclosure each time to get it to bind. Even with the remote right against the enclosure it doesn't bind, Once it does though - it's great. Have taken to carrying tools with me to open the enclosure and close it again. Once it's bound it's solid.
```

---
## \#5 Posted by: Schulerbible Posted at: 2017-01-07T23:53:07.431Z Reads: 205

```
Hmm, it's a bit more strange than I thought. Definitely not the transmitter. My wires are soldered to the VESC, however, moving the cable just a tiny bit (tiniest bit) and the thing binds. Not moving the cable at all nothing binds. In order to rule the RX out I have to change the cable.

But anyway, why the heck has the GT2E no issues at all (binds in less than 2s) and the Nano-X is flashing forever??? Ahhh ... 

Here is a picture of the PCB inside the RX housing.
<img src="/uploads/db1493/original/3X/e/8/e85161dd73f696384a255cf48d6ec719d82c5733.jpg" width="690" height="432">
```

---
## \#6 Posted by: lox897 Posted at: 2017-01-08T00:06:45.319Z Reads: 193

```
Is it just the pic or does that pin look burnt?<img src="/uploads/db1493/original/3X/c/7/c73cf984c5f3320d627dcc2f5259badee52a6fa6.PNG" width="640" height="474">
```

---
## \#7 Posted by: lox897 Posted at: 2017-01-08T00:08:03.919Z Reads: 190

```
Could you also post a picture of the other side of the receiver where the headers are soldered? I assume they are through hole, but I could be wrong
```

---
## \#8 Posted by: lox897 Posted at: 2017-01-08T00:09:05.729Z Reads: 190

```
C2 and C4 are missing parts, not sure if it's supposed to be like that though
```

---
## \#9 Posted by: Schulerbible Posted at: 2017-01-08T00:49:24.183Z Reads: 197

```
Here are three more pictures. The marked pin is not burned. All soldered pins look solid. <img src="/uploads/db1493/original/3X/a/4/a42579f9879d1b1c2e0f8e2515d636fd5932b015.jpg" width="690" height="372"><img src="/uploads/db1493/original/3X/3/4/340faba48a44b11a6ef060a02caefa3089fcb050.jpg" width="578" height="500"><img src="/uploads/db1493/original/3X/8/7/879dc8afbb0fc61632354363660d84a73fe79140.jpg" width="666" height="500">
```

---
## \#10 Posted by: lox897 Posted at: 2017-01-08T00:57:22.949Z Reads: 196

```
Oh ok, it was just the photo then. Not the best soldering job on some of those through hole pins.
```

---
## \#11 Posted by: Schulerbible Posted at: 2017-01-08T01:10:23.141Z Reads: 194

```
But it looks solid to me. It's getting even weirder now. When I touch the cable with my bare hands it binds immediately. However, when I use a plastic clamp instead I can bend twist do whatever you can imagine and nothing happens. Only binds when I touch the cable with my hands???
```

---
## \#12 Posted by: lox897 Posted at: 2017-01-08T01:17:52.219Z Reads: 192

```
Something's definitely up with these. Has it got a ferrite ring on it? It must not be making contact properly somewhere.
```

---
## \#13 Posted by: Schulerbible Posted at: 2017-01-08T01:20:13.366Z Reads: 190

```
No ferrite ring installed + no contact to other parts ... and it worked before.
```

---
## \#14 Posted by: Esrapp21 Posted at: 2017-01-08T03:30:01.950Z Reads: 188

```
Has there been any good experiences with this remote? I need some hope for my first eSk8 remote...
```

---
## \#15 Posted by: lox897 Posted at: 2017-01-08T05:25:43.288Z Reads: 183

```
Hmmm. I honestly have no idea then dude, probably best if @onloop sorts this out
```

---
## \#16 Posted by: Schulerbible Posted at: 2017-01-08T08:27:34.218Z Reads: 184

```
Honestly, get a GT2B and a 3d printed housing. The Nano-x looks great but apparently only works 
with lots of luck.
```

---
## \#17 Posted by: Esrapp21 Posted at: 2017-01-08T16:08:44.713Z Reads: 194

```
It's too late... I got the space cell + remote deal a while ago and I am still waiting on it.. I hope by the time I get it this whole thing is resolved.
```

---
## \#18 Posted by: mmaner Posted at: 2017-01-08T20:40:40.665Z Reads: 210

```
I haven't had any trouble, been running it for a few days now.
```

---
## \#19 Posted by: Strawbs Posted at: 2017-01-09T01:20:01.363Z Reads: 208

```
Here is a short video showing my issues.  Enertion support has yet to respond regarding a refund or replacement.

https://www.youtube.com/watch?v=Xra6ieDEfjA&t=3s
```

---
## \#20 Posted by: Kaden56 Posted at: 2017-01-09T05:02:50.740Z Reads: 209

```
Looks like they are on holiday till the 14th for the most part. I contacted them and they just took my email down on a list and said they'll get back to me. Good thing I can't ride my board in this snow right now anyway or I'd be super mad about it. To much hype for a remote that can't even live up to my gt2b.
```

---
## \#21 Posted by: Schulerbible Posted at: 2017-01-09T11:56:46.341Z Reads: 196

```
Just for the sake of interest. Does it bind when you squeeze the cable that is attached to channel 1 (somewhere between the vesc and the receiver)?

I have exactly the same issue but it binds always when I squeeze the cable. Have you tried to use the Winning receiver with the Nano-x controller (... possibly makes no sense).

Cheers
```

---
## \#22 Posted by: Truckster Posted at: 2017-01-09T18:42:11.084Z Reads: 182

```
I have the Nano X as well and no problems. But try again the initial binding step. connecting the servo cable to channel 1 or 2 and then the loop cable that came with the Nano X into the binding position. Then wait till they connect, unhook the binding loop cable and restart the ESC. Then it should work. I have sometimes the issue that it doesn't connect. But if I turn the Nano X on first and then the ESC, I don't have any problems.
```

---
## \#24 Posted by: Truckster Posted at: 2017-01-09T20:06:14.437Z Reads: 181

```
I received a mail today that they left the country for making some contracts and return after the 12th. Regular mail from the webpage should be finde after the 12th
```

---
## \#25 Posted by: Kaden56 Posted at: 2017-01-10T05:44:18.499Z Reads: 179

```
So my Nano x started working every time now out of no where. Take that with a grain of salt though cause it very well may not last long. But if it does then this remote is as awesome as I was hoping.
```

---
## \#26 Posted by: Schulerbible Posted at: 2017-01-10T08:45:50.640Z Reads: 176

```
Well, I hooked my receiver up with an external 5V power supply (no signal line attached to VESC) and the remote binds every time! Maybe I'll get this issue resolved sooner than anticipated.

Ok, resolved, the signal line was half broken, all works again!!!

Maybe this is a good test for the other Nano-Xses out there which never worked or stopped working. Hook it up to an external source (just +5V and GND). Should bind in seconds!!!
```

---
## \#27 Posted by: Esrapp21 Posted at: 2017-01-11T04:50:23.250Z Reads: 166

```
I don't know how he did it, but @onloop has magically fixed a bunch of remotes!
```

---
## \#28 Posted by: mmaner Posted at: 2017-01-11T16:50:34.735Z Reads: 163

```
LOL, that was awesome...  I think he hired a reaaaaallllllyyy good priest, or maybe used some secret RX voodoo :).
```

---
## \#29 Posted by: Kaden56 Posted at: 2017-01-12T00:45:15.504Z Reads: 163

```
Seriously! I was about to throw the remote against the wall the first day so I just put the board in the corner for a few days and then I tried it again and it has worked ever since!
```

---
## \#30 Posted by: Jebe Posted at: 2017-01-12T01:00:23.768Z Reads: 159

```
never got a loop cable with mine
```

---
## \#31 Posted by: vjsharpeyes Posted at: 2017-01-26T02:29:49.648Z Reads: 146

```
Yeah me neither, just remote and receiver. Not even any instructions.
```

---
## \#33 Posted by: i2oadsweepei2 Posted at: 2017-02-18T12:41:16.834Z Reads: 140

```
I just opened my Nano-X yesterday and tried to bind it with no luck. I picked it up from the group buy through Michaelinvegas.  I also went through a bunch of threads in search of advice that would work. No luck. It will not bind while my TB12s esc is plugged in. The moment I pull the esc signal wire, it binds instantly. I'm also using a TB bec to power the system. It's such a basic remote compared to what I use for my rc's. Pretty sure something is up. I'm off to contact enertion support. What has been everyone's experience with repairs?

P.S. When I plug the remote in to charge I don't get any led's. Is this normal?

Cheers,
Kev
```

---
## \#34 Posted by: Schulerbible Posted at: 2017-02-19T07:09:03.963Z Reads: 132

```
[quote="i2oadsweepei2, post:33, topic:15740"]
hen I plug the remote in to charge I don't get any led's. Is this normal?
[/quote]

Mine shows a red LED only when partially charged. Once fully charged all LEDs are off.

Not sure about the signal cable. This issue is still not resolved.
```

---
## \#35 Posted by: i2oadsweepei2 Posted at: 2017-02-19T10:38:47.734Z Reads: 130

```
Thanks @Schulerbible, I'm just not sure what it's doing when I plug it in. Enertion support contacted me after they saw my post above. I've replied and hopefully the conversation will continue after the weekend. Basically they said they have no stock to send a new receiver and I need to send it to a repair agent. I will ask about the charging too.
```

---
## \#36 Posted by: AlM9SlDEWlNDER Posted at: 2017-02-21T21:48:08.393Z Reads: 127

```
I have the same issue. Once I disconnect the signal wire, it binds right away.  I was thinking of putting a NC (Normally closed) pushbutton inline with the signal wire so that I could just hit the button to momentarily disconnect the signal line and get it to bind.  I did the remove the sticky foam mod from one of the other forum posts, and that did not work.  I am thinking that it might have something to do with a floating signal pin and the need for a pulldown resistor.  The signal pin might be floating in an undefined state with some residual voltage in it, and this might cause an issue for the binding process.  I might try to add a pulldown resistor to see what happens.  

[Link on info to Pull-up and pull-down resistors.](http://playground.arduino.cc/CommonTopics/PullUpDownResistor)
```

---
## \#37 Posted by: i2oadsweepei2 Posted at: 2017-02-22T00:51:44.913Z Reads: 123

```
Thats a pretty good idea with the NC button. To me though this is a safety concern and if it's not working properly then I don't trust it. I would still feel like i'm waiting for it to fail in some way at some point. I just sent mine in today for service, The post office said guaranteed delivered tomorrow. It's been a swift and courteous experience so far, and even better since Enertion contacted me first after seeing my post here. I would contact them for help. Once I explained what happened they told me to send it in. Perhaps they know and can advise you on a fix I if you are able to do it yourself. I don't want to void any warranty.
```

---
## \#38 Posted by: i2oadsweepei2 Posted at: 2017-02-26T21:41:48.572Z Reads: 123

```
I shipped my Nano-X to an Enertion repair agent on Tuesday, he received it on Wednesday. He fixed it and I had it back by Friday. Top notch service and excellent communication. I tested it out and it charges when plugged in and now binds in under 5 seconds. It's getting warmer here. Hopefully I can get out for a long run soon. Cheers!

Thank you @EnertionSupport & @onloop
```

---
## \#39 Posted by: Plumb77 Posted at: 2017-02-27T00:21:12.935Z Reads: 122

```
How did you get the return process. They sent me a message but no shipping info.
```

---
## \#40 Posted by: SageTX Posted at: 2017-02-27T00:35:56.036Z Reads: 122

```
This _may_ help.  At least it's something to look for.

https://www.youtube.com/watch?v=sXdfi6yEKRw&t=95s
```

---
## \#41 Posted by: i2oadsweepei2 Posted at: 2017-02-27T02:57:31.771Z Reads: 118

```
They contacted me after I posted on this thread. If you are having an issue I am sure they will contact you as well or you could pm enertionsupport.
```

---
## \#42 Posted by: SeanHacker Posted at: 2017-03-01T20:54:34.124Z Reads: 112

```
Yep. I think that may be one of the receivers that I sent @blasto. Both of my nano-x's bind every single time with no issues now. It's nice that this fix can be done by anyone with a soldering iron.
```

---
## \#43 Posted by: Plumb77 Posted at: 2017-03-11T14:19:19.472Z Reads: 110

```
Which one is the crystal?
```

---
## \#44 Posted by: SageTX Posted at: 2017-03-11T14:41:38.310Z Reads: 109

```
Haven't opened mine yet. Might get to it later today. I'll post a pic if I figure it out.
```

---
## \#45 Posted by: Plumb77 Posted at: 2017-03-11T14:47:47.962Z Reads: 109

```
Okay thanks let me know
```

---
## \#46 Posted by: Shep Posted at: 2017-04-03T00:19:12.205Z Reads: 98

```
I bought three nano-x controllers for a few different builds I'm doing, and none of them work. I contacted enertion and they just sent me a video on how to plug it in and turn it on. Ha.
I think they're just made as cheap as possible, I've never had any troubles with the torque boards remote from DIY.
```

---
## \#47 Posted by: Plumb77 Posted at: 2017-04-03T17:57:45.648Z Reads: 93

```
Any update on this
```

---
## \#48 Posted by: SageTX Posted at: 2017-04-03T18:07:17.714Z Reads: 96

```
Sorry no. My mini remote works so well the nano-x isn't priority.  So few hours....
```

---
## \#49 Posted by: Ken Posted at: 2017-04-24T06:04:02.837Z Reads: 93

```
Here's my issue. Email was just sent to Enertion. Order was placed on 03/07/17, and received a few weeks later, as they were on backorder at the time.
https://www.youtube.com/watch?v=AtePocgin7A&feature=youtu.be
```

---
## \#50 Posted by: Vince Posted at: 2018-03-31T13:56:45.392Z Reads: 50

```
Hello everybody, I have a  problem too with my nano-X controller, the receiver with the remote doesn’t work so I would like to know if I can bind the nano-X with a flysky GT2B reciever and how to do that.
Thanks a lot !
```

---
