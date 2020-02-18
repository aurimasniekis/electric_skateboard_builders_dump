# Yuneec Ego ESC (ECU) problem

### Replies: 41 Views: 8848

## \#1 Posted by: samusaki Posted at: 2016-06-29T12:06:37.713Z Reads: 227

```
Hey there.
I have 2 Yuneec Ego. 
Mine and friends. 
Both dead.

I have put new ECU (ESC) on mine EGO, but it died in 2 ceconds, so i guess problem was not faulty ECU , but something to do with battery or the motor.

Friends Ego is waterdamaged... It says on the Ego website that it is water resistant...
I have ordered new controller for friends board, but i dont wana fry another 100eur for 2 seconds of  fun. 

Can you guide me on , how can i test motor , battery , and find cause of the problems for both boards?
```

---
## \#2 Posted by: Lizardking0069 Posted at: 2016-06-29T13:27:47.931Z Reads: 213

```
 What happened between the last time it ran and when it stopped working?

Also, by not working you mean that the LED does not turn on or something elae?

Finally get a multimeter and tools. Based on the info you give me I can guide you on which parts to dismantle and inspect.
```

---
## \#3 Posted by: samusaki Posted at: 2016-06-29T13:37:34.304Z Reads: 207

```
I have the tools.

First board seems to be water damaged.

Second board, stoped working after i was hitting brakes when driving downhill. Very short hill only 10 meters.
After that, i have brought board home, disassembled controller , and was visually inspecting it. 
It looks good, every thing looks new. I have left it turned on for 1 minute or two, and then i noticed smoke comming from one of the tiny components of the ECU.
Looks like transistor for me, 1 mm in diameter , very small.

After it stoped working, i have bought new controller. Connected it , and it died in 2 seconds.
Thisnew ECU also gets hot (the same little transistor that has blowed on the first board) in 3 seconds of beeing turned on.

Not sure, if that makes it clear to you ? :slight_smile:
```

---
## \#4 Posted by: Lizardking0069 Posted at: 2016-06-29T13:44:25.488Z Reads: 176

```
Take the first board apart and dry it out. 😁

Second one could be multiple things. The BMS could have melted the fets. Open the battery and look at the blue shrink wrap. Check if it has melted on the side opposite the on/off switch.
```

---
## \#5 Posted by: samusaki Posted at: 2016-07-01T03:59:20.130Z Reads: 151

```
So i checked both skates. 
The one with the water, gives 29.3v . The other gives the 29.25v.
Batteries looks beautiful. No signs of melting of corrosion. Looks like new.
What next?
```

---
## \#6 Posted by: Lizardking0069 Posted at: 2016-07-01T11:48:16.364Z Reads: 143

```
That is great news! Batteries are good.

Next, check the ESC (or ECU) It may have water or water damage on it. If you see evidence of water take the board out and clean it thoroughly with alcohol then let it dry.
```

---
## \#7 Posted by: samusaki Posted at: 2016-07-01T12:21:22.712Z Reads: 142

```
Ok, i am cleaning ECU on the water damaged board.

What about the second board ? 
I has no water damage . I was new.
I have taken it out of the box, and first ride it on a street. Then i turned down the hill. 
After hitting brakes, it turned off, and since is not working.
I have dismantled this second board, and found no visible burns or damages on ECU.
So i have turned it on (siwtch), and just looked at the controller.
One of the small parts has burned under my visual inspection. 
Since, i have bought new ECU.

I have put new ECU onto that board, and the new ecu immediately stopped working, and the same part that has burned on the first ECU has started to get hot on the new one. 

On only difference this time, is that on the burned ECU nothing works. And on a new ECU, LED turns on , and the component starts to get hot. 

Because of this , i have never turned half dead ecu on again on that board.
```

---
## \#8 Posted by: Lizardking0069 Posted at: 2016-07-01T13:12:02.673Z Reads: 134

```
Maybe the motor wires are shorted. That would smoke the ESC.
```

---
## \#9 Posted by: samusaki Posted at: 2016-07-01T17:20:02.498Z Reads: 125

```
How to test motor wires?
```

---
## \#10 Posted by: Lizardking0069 Posted at: 2016-07-01T17:44:20.738Z Reads: 124

```
Check resistance between wires and continuity between the mitor wires and the metal of the rotor(ground).

The resistance between the wires should be the same and there should be no continuity between the motor wires and the ground.
```

---
## \#11 Posted by: Lizardking0069 Posted at: 2016-07-01T23:58:23.631Z Reads: 123

```
Also, if the second yuneec was new why not return it and get another one?
```

---
## \#12 Posted by: samusaki Posted at: 2016-07-02T09:31:29.896Z Reads: 122

```
 continuity (beeper thing on multimeter?) 

Resistance is 0 between all of 3 wires.
No beeping if i touch any wire and the ground.

The motor has sensor - s. What is the deal with the sensors?
Can i test them ?
```

---
## \#13 Posted by: samusaki Posted at: 2016-07-02T09:33:18.883Z Reads: 117

```
well, i got one new - water damaged. (dealer refused to fix , because its water damage , altho it says in ego faq that it is water proof.  second one was new - from a guy  . it has no receipt.
```

---
## \#14 Posted by: adam_alkobi Posted at: 2016-09-29T03:37:00.873Z Reads: 100

```
I'm wondering if any of you guys have fixed your boards cause that is what has happened to mine I'm wondering if i should buy the new ESC or ECU
```

---
## \#15 Posted by: samusaki Posted at: 2016-09-29T12:22:18.105Z Reads: 102

```
I suggest you buy your own VESC ESC and program it.

Dont forget, you will have to buy remote control with radio receiver and transmitter. 
You will have to program transmitter and receiver and esc to talk to each other . 
You will have to make sure, ESC works with yuneec motor.

Its alot of job, but after you will complete it, you will have your own board with powerful electronics and every part of it is your own build, and you will know how to fix later issues. 

If ESC brakes, you can always use online fix services. BTW i recommend the 120$ VESC one. You can ebay them or google from germany. 


If you will buy new ECU like i did, you might also fry the sh!t out of it, because there is more to it them ECU, also battery charging, battery balancing, motor powering, transmitting... 

If you dont want to bother, just ship it to dealer, and pay what he charges. :D  should be around 200$
```

---
## \#16 Posted by: alpmanalp Posted at: 2016-10-31T11:35:07.177Z Reads: 90

```
Hello everyone
I would appreciate if anyone can tell me the value of the capacitors and the name of the IC that I marked on stock esc.
Thanks 

<img src="/uploads/db1493/original/3X/f/7/f738ab02e5d1bf1f49ac51b672e8d258fcbdccda.jpg" width="690" height="391">
```

---
## \#17 Posted by: samusaki Posted at: 2016-10-31T11:53:15.551Z Reads: 92

```
Ok, i will check it up later today.
```

---
## \#18 Posted by: samusaki Posted at: 2016-10-31T11:55:46.832Z Reads: 88

```
Guys , I found out , that my ESC failed 2 times , because motor H sensors was going shorting circuit. 
I bought new motor, and every think started to work :D 

>LESSON HERE  : CHECK MOTOR BEFORE PUTTING NEW ECU .
```

---
## \#19 Posted by: samusaki Posted at: 2016-11-01T17:50:13.441Z Reads: 96

```
<img src="/uploads/db1493/original/3X/f/e/fe7828a09cb677858c40cf6bb4cc469e3e3a3df5.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/d/0/d0d8a0d8c2900de625ccbaaf7844dc3119a42241.JPG" width="375" height="500">
```

---
## \#20 Posted by: alpmanalp Posted at: 2016-11-02T10:41:29.926Z Reads: 95

```
thank you. Still can not see the ic i mention. If you bend the capacitor a little bit you can see it. Please read it your self instead of sending the picture. It is not possible to read the ic on the picture.
best
Alpman
```

---
## \#21 Posted by: alpmanalp Posted at: 2016-11-16T13:16:15.286Z Reads: 88

```
I know I am being trouble but. I really need the name of the IC I can not read it from the pictures you sent. Please take a look at the my photo it is marked (red circle) please try to read the name of the IC for me. Thanks
Alpman
```

---
## \#22 Posted by: samusaki Posted at: 2016-11-16T14:33:30.350Z Reads: 82

```
Hey, no problem. If i don't do it by tomorrow, i have totally forgotten, so please remind me , thanks !
```

---
## \#23 Posted by: alpmanalp Posted at: 2016-11-28T12:29:36.611Z Reads: 75

```
hello just to remind you about the ic...
```

---
## \#24 Posted by: samusaki Posted at: 2016-12-07T18:43:13.398Z Reads: 76

```
SORRY !!!! <img src="/uploads/db1493/original/3X/5/e/5ef2a14b9497514a57aa7e2c8eea36af508ee002.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/2/b/2b6a2339552332e443b011300d6507b5d1bf98cb.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/f/2/f2cf7c12021805c5ae7c6c4358175886f7b7dcbd.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/7/0/7047f2109e0bc334260d70a96a1752192cba6231.jpg" width="375" height="500">

this one only has 2 capacitors ;/ 

Ok dissassambled the 3rd controller, nad it  has 3 capacitors, and the little one is 16v220uF
```

---
## \#25 Posted by: jga Posted at: 2016-12-08T14:41:16.203Z Reads: 72

```
Just to go back a bit up in this thread, I had the same problem with the E-Go some month ago: started to blink yellow after a ride, would not start, and finally no light at all, all dead!
I contacted Yuneek in the US, who were quite helpfull, but I leave in Europe so I had to contact their service center in Europe, located in Germany. To make it simple, I was not too impressed with their services.
Anyway, after finally receiving my board (which cost me a bomb to send) they told me the damage was due to water ingress and the battery and ESC had to be changed. Cost brought down to 320 euros as a "commercial gesture". I paid as I wanted to get my board back. To my comment that it was supposed to be waterproof, I never received any answer, but when I received the board back I noticed they put an additional seal around the battery enclosure. Not sure it is really waterproof or even splash proof as I never used it under the rain.
Since then the board has worked fine, but I am now always very careful when the road is slightly wet.
```

---
## \#26 Posted by: 3d-guy Posted at: 2017-03-07T18:41:58.471Z Reads: 67

```
caps=
35v 470uf

ic=
5450
tl 44h
zc98g4
```

---
## \#27 Posted by: tueboard Posted at: 2017-05-09T20:53:19.346Z Reads: 56

```
so it's posible to use a VESC on yuneec ego 1 ?
```

---
## \#28 Posted by: NulodPBall Posted at: 2017-07-15T19:38:07.462Z Reads: 49

```
If you're willing to recreate the functions that the old controller had (i.e. new Bluetooth controller,  etc.).
```

---
## \#29 Posted by: NulodPBall Posted at: 2017-07-15T19:44:12.668Z Reads: 49

```
Samusaki:
In regards to your repeated comments on lack of waterproofness...I hope you realized that unless something is designed to be used under water, it's not water proof  (look up definitions of water resistance), and even then it's only water resistant.

I was in a sport that learned to coat the motherboard so the board doesn't fry when it rains...but >>no-one<< expected the board to work after being submerged in water...even though it tended to be, but only for short times.

Just sayin'
```

---
## \#30 Posted by: primexample Posted at: 2017-09-02T19:20:50.181Z Reads: 49

```
Hello, new here and this seemed like the best place to ask for help after doing a search.

I have a yuneeq ego that has is not working.  Last I checked it turns on but does not connect via phone connection.  The remote has already not been working or holding charge but main concern in getting the board to work again.

Before it completely stopped working it would randomly lose connection to the phone and as time went on that problem became worse.  The board would only connect for a few seconds the stop working.  Also, if the board did decide to connect, connectivity would be lost after hitting any small bump in the road.

Now it seems the board will not connect at all and does not accept a charge.

I am wondering what specific tools I need to disassemble the board and what would should I test?

If anything was not clear please let me know and I will try to clear it up.  I have not tried to turn on or connect the board in months.  I will double check the symptoms and update tonight if needed.

Any help is much appreciated.

Thank you!

Happy Labor Day weekend!
```

---
## \#31 Posted by: jga Posted at: 2017-09-02T19:55:05.023Z Reads: 46

```
Hello,
welcome in the world of the "non-working E-Go"! Same problem as you with battery not charging. It worked a bit the first months, then one day it stopped. I sent it for repair to Yuneec, they replaced battery and ESC and it cost me 300 euros +postage. Allegedly "damage due to water". With all due respect to @NulodPBall, there is a gap between a submarine board and being able to suffer a few drops of rain, and I don't thing Yuneec is anywhere there.
Anyway, I was able to use my repaired board for a few months before it let me down again. I am in the process of changing the electronics to have hopefully a more reliable system.
I think Yuneec should stick to drones...
```

---
## \#32 Posted by: plusto Posted at: 2017-11-21T15:42:31.093Z Reads: 33

```
Hi friends. 

Unfortunately I had ride on a few puddles the other day on my EGO-2 and this what I found since it does not want to start. This is the ECU. Is there any hope? What is that white sticky stuff? Would Yuneec warranty cover this?

https://photos.app.goo.gl/5QKTO6DzM0wCdf9B2[https://photos.app.goo.gl/5QKTO6DzM0wCdf9B2](https://photos.app.goo.gl/5QKTO6DzM0wCdf9B2)
```

---
## \#33 Posted by: jga Posted at: 2017-11-21T16:10:57.601Z Reads: 37

```
I don't know where you are based. In Europe their after sales service is in Germany. So the first hurdle is to send the board there (in my case 50 GBP). Then if it's a water damage it won't probably be covered by the warranty. They will if you're lucky propose a replacement with a discount. In my case battery+ECU 320 Euros.
Then it will still not be even splash-proof.
It's very strange because it seems very well sealed. I don't know where the water is going through.
```

---
## \#34 Posted by: rifaterdemsahin Posted at: 2018-04-21T11:38:23.870Z Reads: 33

```
I should have read this post before attaching a new ECU. Lol. Losing 100 pounds.

after attaching the new ECU. it worked for  10 meters than died. No lights from any where.

As the postal cost is from uk 50 pounds. thinking to send the motor.

Is there anyway we can clean the motor and make the ECU work ?
```

---
## \#35 Posted by: rifaterdemsahin Posted at: 2018-04-23T23:27:21.047Z Reads: 31

```
i did fry it i think
```

---
## \#36 Posted by: mofrofirefly Posted at: 2018-05-07T16:35:58.637Z Reads: 39

```
Hello all I am new, I have a Yuneec EGO2 and was looking for some help trouble shooting a problem.
My board sat in the garage for a month or 2 when I was unable to ride it, everything seems fine on my board, battery is charging fine and remote connects to ecu fine but when I turn the board on it doesnt beep and the led on the esc just kinda flickers. I can make the wheels turn with the remote but only if I spin them by hand at first. I tried riding it by push starting and it will barely move. No indicator lights on the remote shows charged battery and remote. Any ideas?
```

---
## \#37 Posted by: scepterr Posted at: 2018-05-07T16:46:18.376Z Reads: 41

```
Re-bind the remote to ecu, directions are in the manual on yuneecs site
```

---
## \#38 Posted by: mofrofirefly Posted at: 2018-05-07T18:43:14.737Z Reads: 39

```
I tried that with no luck.  I bought another ecu and remote off ebay and hooked it up and had the same issue.
```

---
## \#39 Posted by: michhola Posted at: 2018-05-30T13:01:34.847Z Reads: 35

```
Hey guys,

My Ego stopped working 2 days ago after a hill climb against the wind - went up the hill and back down the other side then turned off the board for a few minutes. When I turned it back on - I got the low battery warning. Then seconds later it just died. My girlfriend pulled me with her Yuneec and the board would spontaneously give the start up beep. Got home and hooked it to my charger. Even though charger shows full charge board won't start up. No beep no LED light.

Does anyone know what the problem could be? Which parts need replacing. 

Will add that the board is 2,5 years old and I car drove over it a year ago and I already have gotten myself a Koowheel gen 2 (much faster :D ) but I am kind of sentimental and don't want to chuck the board out;
```

---
## \#40 Posted by: Danish Posted at: 2018-10-02T02:04:09.798Z Reads: 16

```
Hello Every one,

I have Ego 2 board using it from past 2 years. It got wet 3 times in two years and I kept it to dry and it worked. But recently it was again rain splash and the board is not getting on. 

Any suggestions please
```

---
## \#41 Posted by: Sn4pz Posted at: 2018-10-02T20:33:41.080Z Reads: 15

```
Read the thread
```

---
