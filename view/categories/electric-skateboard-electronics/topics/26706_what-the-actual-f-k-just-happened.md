# What the actual F**K just happened?

### Replies: 42 Views: 2440

## \#1 Posted by: Geddi Posted at: 2017-07-03T22:20:41.457Z Reads: 398

```
This just happened:

So I finished my board about two weeks ago and decided to not take it on the busy streets before I was feeling really comfortable with it and had tested it all the way through. So today it did a little more testing. A nice evening ride on my new awesome board and I finally felt comfortable enough to try and go fullspeed. I was afraid before because I did not have any longboard experience before that.  I went fullspeed (43km/h btw.) and even raced the board uphill to test its limits. And guess what? It was awesome. Everything went totatlly fine. So after about 25min I decided to ride back home ( still 73% battery left). I was not going fast (on a flat street) ( I think about 20 km/h), when it suddendly the motor kind of blocked. I do not know if it completely  blocked. It caught me off guard (enjoying the evening breeze) and it threw me of the board like a rocket. I managed to pull off a proper landing and all I got was a little scratch on my back, but imagine that happening on a normal street with somebody behind me. Anything that would have been driving behind me would have just gotten straight over me (aka --> dead). So I am really glad that I am still in testing phase and after that will be for a long while. However after it threw me off  I immediatly looked at the board and found that the turning the motor by hand was really difficult. Then I tried pushing the board like a normal longobard, but it was really hard. The motor just kind of blocked ( not totally but rotating was a lot harder). So the rest of the way I rode the board home ( It was working totally fine exept the motor was turning harder and don't worry I didnt go faster than 5 or 6km/h) Btw. I was about 5min away from home. When I took another look at the motor at home I found that I was back to normal again (btw. directly after the accident I turned  the board and the remote off waited a little and then turned it on again, but nothing changed). And by normal I mean you could easily push the board or rotate the motor by hand with almost no resistance, like it should be.
Has anyone any Ideas what happend? Maybe you @Namasaki ( we have a smilar build) or you @Jinra ( you have loads of experience I think) 
Maybe I pushed it to hard the minutes before? But I would say it had about 30sec rest before I drove again after coming back downhill. I think the total ride was about 20min. Could the vesc have overheated (because it is covered up), but that would not explain the motor behavior would it?

My build:
Alien 6374 200KV
Bestech BMS
10S lipo battery 
Maytech VESC
```

---
## \#2 Posted by: wmj259 Posted at: 2017-07-03T22:31:36.980Z Reads: 378

```
[quote="Geddi, post:1, topic:26706"]
somebody
[/quote]

Stuff like this most often is because of your VESC settings. Please post the screenshots.
```

---
## \#3 Posted by: Jinra Posted at: 2017-07-03T22:33:59.915Z Reads: 372

```
Along with your VESC settings, tell us what remote you were using as well, and post the VESC settings for that too.
```

---
## \#4 Posted by: Geddi Posted at: 2017-07-03T22:36:22.899Z Reads: 365

```
alright just a sec
```

---
## \#5 Posted by: trampa Posted at: 2017-07-03T22:38:57.550Z Reads: 354

```
Could be your remote/receiver, sending a full brake signal when loosing connection to the hand held radio. What remote do you use? Any remote used on a board should never ever send a brake signal when loosing connection. Unfortunately some do, especially some models designed for esk8.
I once had a motor that had a bad contact somewhere in the windings. Caused the same issue. Full brake at speed, randomly after being O.K. for days. 

First check what happens when you switch of your remote. Does the board brake?

Frank
```

---
## \#6 Posted by: Geddi Posted at: 2017-07-03T22:42:32.142Z Reads: 335

```
but that does not explain why the motor was so hard to rotate when the board was turned off
```

---
## \#7 Posted by: Jinra Posted at: 2017-07-03T22:43:13.479Z Reads: 326

```
If it happens when the board is completely off, it's probably your phase wires shorting. You have to make sure no two phase wires on your motor are touching or it'll be hard to turn even when off.
```

---
## \#8 Posted by: Geddi Posted at: 2017-07-03T22:43:33.236Z Reads: 329

```
<img src="/uploads/db1493/original/3X/9/d/9dcbfc99fee9d0bba44a964f8f55494dc5cde287.png" width="690" height="388"><img src="/uploads/db1493/original/3X/5/1/51372143fef98cab5c3d4279ff8d8c6aeb586fbc.png" width="690" height="388"><img src="/uploads/db1493/original/3X/7/c/7c92e8dc192c77522ab6bd2025d822424ae5d45d.png" width="690" height="388"><img src="/uploads/db1493/original/3X/9/1/91b83db1e9e3d86fc02e52868dc3c2e726f1ea4a.png" width="690" height="388"><img src="/uploads/db1493/original/3X/f/1/f1ff53dfceb735258e7596451c97c09ebd1a7f4f.png" width="690" height="388">
here you go @Jinra @wmj259

I use the APS remote and their receiver.
```

---
## \#9 Posted by: Geddi Posted at: 2017-07-03T22:45:09.531Z Reads: 298

```
<img src="/uploads/db1493/original/3X/2/b/2be09d9833cbec604053a50e4e5475b1f539377b.jpg" width="375" height="500">
 @Jinra nope. I dont think thats the case.
```

---
## \#10 Posted by: Jinra Posted at: 2017-07-03T22:46:09.035Z Reads: 300

```
It must be internally shorting in the motor itself. Try wiggling the motor cables around in different positions with it off and see if the motor is hard to turn at any point.

If the enamel coating on the phase wires (inside the motor) are worn or insufficient it can be shorting.
```

---
## \#11 Posted by: Geddi Posted at: 2017-07-03T22:48:20.760Z Reads: 299

```
the motor once received a little bump. ( more like scratiching the street a little). But that was two weeks ago.<img src="/uploads/db1493/original/3X/b/f/bf02749b16d17ee66512f04faec8aefc36a01d60.jpg" width="375" height="500">
whatever I do  with the motor does not change anything. Also it kind of felt like that the resistance was getting less over time.
```

---
## \#12 Posted by: Jinra Posted at: 2017-07-03T22:49:59.203Z Reads: 297

```
If you want to see what I'm talking about. disconnect your phase wires and touch any two of them together and try turning your motor. Does that feel similar to how it was when your board cut out?
```

---
## \#13 Posted by: Geddi Posted at: 2017-07-03T22:52:54.964Z Reads: 295

```
Yeah it was kind of like that. Question is why did it last for a couple of minutes and then suddenly was gone. And has not come back yet.
I guess what you are saying is I should prepare to buy a new motor
```

---
## \#14 Posted by: Geddi Posted at: 2017-07-03T22:56:03.162Z Reads: 289

```
Also, 
If those wires thouch or anything like that inside of the motor. You could still ride it? Because I could.
```

---
## \#15 Posted by: Jinra Posted at: 2017-07-03T22:57:01.584Z Reads: 287

```
It could have shorted in a certain position, then it moved out of that position and was no longer shorting. That's why I asked you to wiggle the phase wires around as much as possible to see if you can recreate it.

Alternatively, it could be shorting with the VESC. It is a Maytech VESC so I wouldn't entirely trust it in terms of reliability.
```

---
## \#16 Posted by: ShutterShock Posted at: 2017-07-03T22:57:27.713Z Reads: 284

```
This is absolutely possible, it happened to me when I was riding the board around without the wires plugged in to test the motor angle.  The two leads bumped together and the board stopped instantly lol didn't expect it at all
```

---
## \#17 Posted by: Geddi Posted at: 2017-07-03T22:58:38.225Z Reads: 276

```
So the vesc could be shorting as if I let those motor wires touch itself?
Is there a way to narrow down, whether it is the motors fault or the vescs fault?
```

---
## \#18 Posted by: Jinra Posted at: 2017-07-03T22:59:11.940Z Reads: 273

```
You just gotta test, no one on this forum will be able to say for sure.
```

---
## \#19 Posted by: Geddi Posted at: 2017-07-03T22:59:38.005Z Reads: 271

```
but how do you suggest? I cannot recreate the scenario of driving on the street in my garrage.
```

---
## \#20 Posted by: Jinra Posted at: 2017-07-03T23:06:09.680Z Reads: 269

```
Your integrator limit and bemf coupling parameters seem kind of low, could you post detection results as well.
```

---
## \#21 Posted by: Geddi Posted at: 2017-07-03T23:07:42.403Z Reads: 259

```
Will do. What settings do you recommend. I honestly have no Idea what does parameters do. It is set to default.
```

---
## \#22 Posted by: Schulerbible Posted at: 2017-07-03T23:11:07.982Z Reads: 251

```
Was this a brand new motor, must have gone through a lot of abuse? And why don't you align the phase wires towards the truck as it was pointed out many times? Every time the truck hanger turns you put stress on the phase wires which could have led to an internal damage!?
```

---
## \#23 Posted by: Geddi Posted at: 2017-07-03T23:12:10.936Z Reads: 255

```
<img src="/uploads/db1493/original/3X/7/3/731384a0490f92cbf4c15408f2e7dc2afef01b71.PNG" width="690" height="130">
@Jinra
```

---
## \#24 Posted by: Jinra Posted at: 2017-07-03T23:13:16.296Z Reads: 251

```
Oh yea that's WAY off. Make sure you hit "apply" **AND** "write configuration" to apply the values.
```

---
## \#25 Posted by: Geddi Posted at: 2017-07-03T23:13:59.939Z Reads: 251

```
It is from APS. And it looks like that because it scratched the street once on flat ground at very low speeds. Also there is a lot of space for those wires to move. No truck movement could have ever caused damage.
```

---
## \#26 Posted by: Geddi Posted at: 2017-07-03T23:17:32.121Z Reads: 248

```
Thanks for pointing that out. Whatever that changed I hope it is good . Learned another thing.
```

---
## \#27 Posted by: Geddi Posted at: 2017-07-03T23:19:23.476Z Reads: 241

```
Any Idea how I could try to recreate the scenario?. Or is the only option putting on full body armor and riding at rather low speeds till it happens again?
```

---
## \#28 Posted by: Jinra Posted at: 2017-07-03T23:20:51.983Z Reads: 239

```
That would work, though you might end up in the same scenario of not knowing whether it's the VESC or the motor. Perhaps it was simply the settings that were wrong, but it shouldn't happen when the whole system is shut off.

Honestly, my guess is motor, but if you want to be safe, replace both motor + VESC. Otherwise, suit up!
```

---
## \#29 Posted by: Pedrodemio Posted at: 2017-07-03T23:21:09.406Z Reads: 231

```
Did you check your motor bearings? That happened once, it did not throw me off, but it can't even start the board

One bearing was worn and sometimes it would lock and other it would be fine, heat can have an effect on that due to the metal expanding a little bit, if the tracks or the balls have wear, Just a little bit of expansion can lock the whole assembly
```

---
## \#30 Posted by: Geddi Posted at: 2017-07-03T23:23:44.648Z Reads: 226

```
yeah I actually took a look at that, but they are fine and I don't see a reason why they would not be.
```

---
## \#31 Posted by: Geddi Posted at: 2017-07-03T23:27:45.895Z Reads: 217

```
I knew this was a wallet draining project over time from the beginning, but I didint think it was goint to happen that fast :D . Well I think new motor and VESC it is. Probably not a maytech vesc and a different motor ( I did not have the best experiences with APS to be honest). And a new motor pulley will be needed as well then. Still I do not know. APS makes great products I think and the motor really looked like a high quality product and I think it is ( I mean mistakes happen, but...).
```

---
## \#32 Posted by: jazzcool Posted at: 2017-07-04T00:04:17.519Z Reads: 211

```
I'm nearly sure you got a loose magnet inside the motor. Because you had a bump on your motor and it's hard to turn by hand. I come from the drone racing world and it's common.
```

---
## \#33 Posted by: Smorto Posted at: 2017-07-04T00:25:03.707Z Reads: 208

```
I agree with @Jinra that it is a short in either the motor or the vesc.
```

---
## \#34 Posted by: Geddi Posted at: 2017-07-04T05:32:45.338Z Reads: 202

```
yeah I am probably going to exchange the motor And if that does not help the vesc as well.
```

---
## \#35 Posted by: Okami Posted at: 2017-07-04T07:50:26.313Z Reads: 203

```
Well, it looks like some people already threw ideas here on what could be guilty but I thought to share my experience I had recently -

I was making a new motor plate and stupidly I left the motor on the table where there happened to be a lot of metal shavings.

Somehow some huge shavings got inside the barrel and it also did not allow the motor to turn nicely, I could move it to one side but not to the opposite one, otherwise it just locked instantly.

I assume this might not be your case but I experienced something similar - difficulty to turn, as metal shavings blocked the gap between the magnets and stator, I assume If i did try to run the motor, it might have just snapped fragments of magnets in the process.

---

Besides this - I had to open the motor and clean the shavings for it to operate good once again. 

Im not sure is this a possibility for you but it looks like alien motors have openings just across the 'street' not on the side, like my turnigy motor has.

---
So yeh, if everything else fails to eliminate the problem (like you try different vesc but problem still might persist) then who knows, maybe a small fragment got into the motor or something.

Though, I think this is unlikely a case for you but as I said at the beginning, I still thought to mention it, just in case :)
```

---
## \#36 Posted by: lrdesigns Posted at: 2017-07-04T08:42:18.735Z Reads: 183

```
Also check the length of your motor screws, if too long they can touch the motor windings and cause a short.
```

---
## \#37 Posted by: Geddi Posted at: 2017-07-05T06:59:26.920Z Reads: 164

```
@Okami @Jinra and everybody else
I managed to recreate the scenario under not so deadly circumstances. When the board instantly breaked all of a sudden, I flipped it arround and found that the motor was hard to turn once again. I instantly disconnected the motor wires and made sure non of them touch each other. --> Problem was gone. As soon as I plugged them in again the problem was back. After a few 100m of riding in that state it was working normal again.

It seems to be the maytech VESC, that is somehow shorting the motor at random I think.
I will replace the VESC and let you guys know how it went.

**Thank you guys for helping me out!**
```

---
## \#38 Posted by: lrdesigns Posted at: 2017-07-05T07:05:58.352Z Reads: 161

```
That is really strange, normally esc's either work or let the smoke out. Interested to know if this solves the issue. I have maytech's and they have been good to me.
```

---
## \#39 Posted by: psychotiller Posted at: 2017-07-05T07:16:28.832Z Reads: 158

```
I fried a mosfet (or 2) on one of my vescs a while back and it phased out the motor. (put on the brakes) Permanently though. Whether it was on or off. Can be repaired.
```

---
## \#40 Posted by: Geddi Posted at: 2017-07-06T23:14:28.262Z Reads: 143

```
well i don't think i am capable of doing any repairs on that thing. Also I am going to wait with my pruchase a little. Just to make sure I do not waste my money
```

---
## \#41 Posted by: hornet90 Posted at: 2017-07-16T13:11:03.474Z Reads: 124

```
did u get it back up and running
```

---
## \#42 Posted by: Geddi Posted at: 2017-07-21T12:22:08.885Z Reads: 95

```
i have not done anything yet, but adjust a few vesc settings. The problem has not really come up again. Maybe every couple km for less than a half second, but not permanently. Its not enough to throw you off though. I am still going to exchange stuff. I have not done it yet because I am thinking about upgrading to two motors soon.
```

---
