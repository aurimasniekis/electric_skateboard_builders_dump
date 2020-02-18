# KALY NYC Board BLOWN VESC - Ernesto has dropped all contact, HELP

### Replies: 71 Views: 2840

## \#1 Posted by: Dogman1247 Posted at: 2018-07-30T04:50:57.328Z Reads: 485

```
I have a kaly nyc street carver

Ernesto has dropped all contact, Ive tried instagram, his cell phone, calls, texts, nothing in the past few weeks. So here we are.

I had to replace a vesc 
I have a vesc X and one focbox currently in the board, but the vesc that I think is bad it is not "plug and play" I cannot just plug the new one in (see photos below)
```

---
## \#2 Posted by: Dogman1247 Posted at: 2018-07-30T04:54:45.288Z Reads: 482

```
![IMG_4638|375x500](upload://bNxxRbck4XXd5R84CIXtn0sqD3q.jpg)![IMG_4639|375x500](upload://5MhE4YHFy56ClGCcb0kfnkjOwQU.jpg)

The board should plug into the three little connectors here

the older photos before had this funny little splice connecting the two vescs, (I am a total noob at this since ernesto has dropped off the face of the earth and has his customers do vesc repair and gives them zero instructions.)

here is the photo of before (the little splice I was talking about 

![IMG_4600|375x500](upload://hjyuofX6qP7XrF31KrbGpJ77dSJ.jpg)
![IMG_4599|375x500](upload://wl9ntppjgrckoE1xuSZcsSugUrA.jpg)
![IMG_4598|375x500](upload://hP3coZsNisjaqlPEIQLNKnsWCh.jpg)
```

---
## \#3 Posted by: Andy87 Posted at: 2018-07-30T05:05:24.846Z Reads: 456

```
I don’t exactly see what’s your problem.
You can’t connect the receiver with both controller? 
If yes, than search for y-split here.
Should give you an answer how to connect the wires.
Or just try it here with @Kaly.
I‘m sure he will reply as soon as he has a free minute
```

---
## \#4 Posted by: Michaelinvegas Posted at: 2018-07-30T05:10:51.098Z Reads: 449

```
https://www.electric-skateboard.builders/t/new-vesc-user-read-this-complete-walktrough-of-the-vesc/2980
```

---
## \#5 Posted by: Dogman1247 Posted at: 2018-07-30T05:14:49.954Z Reads: 436

```
I got that part down, Ive messed around in bldc tool a bit, but my issue is with these wires the hardware part Im unsure where to plug anything in, and if I need to solder anything.
```

---
## \#6 Posted by: Dogman1247 Posted at: 2018-07-30T05:16:56.199Z Reads: 437

```
im reading this one here

https://www.electric-skateboard.builders/t/vesc-faq-connect-two-vesc-via-canbus-for-dual-motors/142

i dont understand which wires to plug in.
```

---
## \#7 Posted by: Dogman1247 Posted at: 2018-07-30T05:19:19.455Z Reads: 411

```
I have the 2m setup so the Vesc are talking to each other, the 3 pin connector how do I know which one to connect to what I believe is the signal for the remote? it would leave one of the vescs 3 pin connectors disconnected.
```

---
## \#8 Posted by: Mikenopolis Posted at: 2018-07-30T05:20:44.357Z Reads: 410

```
It’s really hard to see what you are trying to show. From what I see, Ernesto is using canbus so there would be no Y-Splitter. The top vescX is the master, so the remote’s receiver should connect to that one, the bottom FocBox is the slave so it should have nothing connected besides the two canbus cables and motors sensor, let that other cable dangle. 

When setting just make sure the slave FocBox takes into from the master vesc. 

Is this what you are asking?
```

---
## \#9 Posted by: Dogman1247 Posted at: 2018-07-30T05:23:10.540Z Reads: 405

```
I believe it is the Y split i am looking for the older one has one built in it appears... I have the older vesc that was having issues

hers a photo of it

![IMG_4640|375x500](upload://7tnGVxoyckYhehOjN0zcyXlDjpW.jpg)![IMG_4641|375x500](upload://exhVoRph5ffak3DPVz0djLPj0HL.jpg)
```

---
## \#10 Posted by: Dogman1247 Posted at: 2018-07-30T05:24:40.450Z Reads: 383

```
I think your correct mike, I am just a noob and thinking a dangeling wire does not make any sense... I will give that a try and see if i can configure which is master and slave.
```

---
## \#11 Posted by: Mikenopolis Posted at: 2018-07-30T05:34:14.855Z Reads: 383

```
Was that black and white canbus cable there before?!

FocBoxes comes with that receiver wire soldered on so it’s always there. VescX didn’t...if you don’t want to deal with making a y splitter then just do this and use canbus. Make sure you NEVER disconnect the canbus cable if the board is on!

![image|438x500](upload://7KHit9p8vXm32NH5rz28MjiA59y.jpeg)
```

---
## \#12 Posted by: Blasto Posted at: 2018-07-30T05:36:21.764Z Reads: 367

```
I believe @Kaly uses can bus for loading settings only. And uses split ppm for control
```

---
## \#13 Posted by: Dogman1247 Posted at: 2018-07-30T05:37:23.823Z Reads: 375

```
the red line your drew I have connected that one,

the green one It is currently not connected to anything.

![795ae2164ef7fc4d06b7e6783ec4e73a4bc8424d_1_375x500|375x500](upload://br1TEQIjEP4bNBvZgquleDmr6EW.jpg)

this is how kaly nyc had this one setup.. with some weird single cable hooked up so the two vescs connected
```

---
## \#14 Posted by: Dogman1247 Posted at: 2018-07-30T05:38:06.884Z Reads: 348

```
soooo if this is true... What should I do?
```

---
## \#15 Posted by: Mikenopolis Posted at: 2018-07-30T05:40:06.143Z Reads: 349

```
If that’s what he does. How does the Bluetooth module work I thought it didn’t work via ysplit becuase it would only read the one vesc it’s connected to?  Does he leave the canbus on along with ysplit!?
```

---
## \#16 Posted by: Andy87 Posted at: 2018-07-30T05:51:57.821Z Reads: 344

```
Bluetooth connected to the master.
master slave via canbus for setup and transfer data.
y-split for speed control.
should work without problems
```

---
## \#17 Posted by: Dogman1247 Posted at: 2018-07-30T06:13:00.807Z Reads: 346

```
So I need to get a Y split?
```

---
## \#18 Posted by: Andy87 Posted at: 2018-07-30T06:21:44.996Z Reads: 349

```
The question is
What is not functioning?
If you can set up your controller as master slave via can than just connect the master to the remote receiver and good to go.

If you want to go with ysplit than you can make your own too if you have a solder iron.
Just make sure that the 5V wire just connected to one controller. (Should be the middle wire. Just cut on one side€. And don’t forget to heat shrink the single wires after soldering.
You won’t short anything
```

---
## \#19 Posted by: dareno Posted at: 2018-07-30T07:57:34.697Z Reads: 346

```
![image|375x500](upload://7Ib9RxAZ7EFbryWAbMqiL3mcpE4.jpg)
so here we have the vesc x top of pic
![image|375x500](upload://7kjxNpO2ojKc0FSmLZ3MCU3EizF.jpg)
here we have the focbox top of pic

What did you change from the original install?
When you dismantled did you photograph?

I agree with mike it looks like the set up is can bus for programming and split ppm for signal.  The splice is probably the splitter to connect the receiver to both vescs but a bit unclear.  How was it originally set up before you removed the blown vesc?
```

---
## \#20 Posted by: Kaly Posted at: 2018-07-30T11:20:48.194Z Reads: 324

```
Hi
The set up is done via can bus.
Read the VESC walktrough link by @Michaelinvegas and you should be up and running in no time.
it is easy to understand once you actually read it.

here are the programming values, since you want less powerful brakes 
Motor Max 60
Motor Min -40
Battery Max 30
Battery Min -8
```

---
## \#21 Posted by: Ixf Posted at: 2018-07-31T01:11:05.658Z Reads: 279

```
Couple of notes here...
How did you know the vesc was blown?
Was it throwing DRV?
Do you have pictures of original setup?
NO Vescs are plug and play...  its probably best to slow down and read through the docs before moving forward, bad setup can blow the VESC.

As for Ernesto's setup.  its like what blasto said.  PPM splitter to control, canbus to program.
```

---
## \#22 Posted by: Dogman1247 Posted at: 2018-08-01T06:06:05.776Z Reads: 256

```
[quote="Kaly, post:20, topic:63276"]
@Michaelinvegas
[/quote]

its been ages, Ive called, texted, instagram nothing..

thanks for getting back to me here on the forums.

The new vesc you sent me has no split PPM only a can bus setup

the current PPM is going into the reciever on the VESC X

the New Focbox ppm is just dangeling and doing nothing...

I can get one motor to spin up on vesc tool and the other can spin up via the remote control.
```

---
## \#23 Posted by: Andy87 Posted at: 2018-08-01T06:42:04.751Z Reads: 240

```
did you set up your controllers to communication via can bus?
you need first to enable that.
open your vesc tool or bldc tool and config. one as master and one as slave (ID 0 and 1) and enable sent status via can.
you can also enable traction control in case you want.

If this not functioning just make a Y-Split cable out of your two cables going to the focboxes.
I think it was already written here how to make it. It shouldn't be a big problem. 

Try this and let us know if you got a result from it.
We will get you back to dual, don´t worry ;)
```

---
## \#24 Posted by: Dogman1247 Posted at: 2018-08-01T22:36:00.989Z Reads: 217

```
So I gotta get a solder kit together if this can bus system wont work?
```

---
## \#25 Posted by: Andy87 Posted at: 2018-08-01T22:49:47.206Z Reads: 212

```
You can buy just one of this 
https://www.firgellirobots.com/products/y-split-flat-parallel-cable-female-futaba-2-female-futaba-60-strands 
Guess on amazon you can get them too
But you need to cut the middle wire on one site
```

---
## \#26 Posted by: Battosaii Posted at: 2018-08-01T23:15:13.090Z Reads: 201

```
Split ppm is a set up escs don't come set up you have to do it your self. 

It's very simple the esc communicate via Can bus or split ppm for remote signal. If you are running split ppm and only conect it to one esc it's impossible that the other will spin too unless you are a wizard. The VescX has pins to plug in the receiver and the Focbox has a wire harness with a plug at the.end they look different but they work exactly the same. Plug them in and it will work.
```

---
## \#27 Posted by: Bobby Posted at: 2018-08-01T23:21:38.156Z Reads: 201

```
Not trying to sound like a dick but if you read a bit, you would easily figure this out. Al the info needed is on this website and videos most likely on you tube. Search the forum, its a goldmine of knowledge
```

---
## \#28 Posted by: Dogman1247 Posted at: 2018-08-01T23:45:45.397Z Reads: 197

```
is this kit plug and play I dont have to do any soldering?
```

---
## \#29 Posted by: Dogman1247 Posted at: 2018-08-01T23:47:33.568Z Reads: 201

```
Well I kind of just wanted to buy a esk8 that doesnt constantly break down on me and me as a consumer has  to open this up get on the forums and mess with this thing... 

Defiantly one of the benefits of purchasing an evolve..
```

---
## \#30 Posted by: sayekim Posted at: 2018-08-01T23:54:36.043Z Reads: 200

```
To be fair you do have the option to send the board back for repairs. You’d have to do the same with an evolve board when that fails. Note I typed when.
```

---
## \#31 Posted by: Dogman1247 Posted at: 2018-08-01T23:56:04.221Z Reads: 191

```
Well I cant send it back when ernesto drops off the face of the earth, has no contact 

Ive already sent this board back now twice its been nothing but issues.
```

---
## \#32 Posted by: sayekim Posted at: 2018-08-02T00:03:58.254Z Reads: 199

```
Yes that is not pleasent and I agree you deserve more and direct support from what I have read but the truth there is I only know of one side of the story here. 
If I were the noob here I’d want to have kaly give me step by steps to fix it. 

Never mind that now though. Do you know what to do now and get it to work?

If it were me I’d simply forget the split ppm and run the receiver to the master only and use the canbus for the communication between the two focboxes. 
Otherwise simply split the ppm and follow what was told. Both will work.
```

---
## \#33 Posted by: Dogman1247 Posted at: 2018-08-02T00:07:35.779Z Reads: 198

```
Im currently stuck with the Can bus system

only able to get one motor to spin when using vesc tool 

messed around with it a but setting up master and slave and now its saying firmware issues (which I already updated) 

if your able to skype or facetime id love to
I PM'd you
```

---
## \#34 Posted by: Andy87 Posted at: 2018-08-02T00:57:11.580Z Reads: 186

```
Depends 
If on one of the focboxes the cables already soldered than you need to get rid of them.
If the wires just plugged than you just need to unplug the old wires, cut one side of the new cable the 5V wire and you good to go
```

---
## \#35 Posted by: Andy87 Posted at: 2018-08-02T00:58:15.901Z Reads: 190

```
So both now have the same firmware, right?
```

---
## \#36 Posted by: Dogman1247 Posted at: 2018-08-02T00:59:36.062Z Reads: 198

```
I believe so, I am able to get both motors to detect atm and going through this video here 
https://www.youtube.com/watch?v=v1glLDO-EjA&t=604s

by far the best video ive seen yet

Are you able to skype?

westonevans1 is my skype id
```

---
## \#37 Posted by: Dogman1247 Posted at: 2018-08-02T01:17:46.567Z Reads: 190

```
having some issues getting both motors on firmware with canbus, im unsure which motor is the master and which is the slave, Ive been playing around with them setting them at 0 and 1 and using the can in vesc tool,

can get one motor to spin normally and the other one will not register... kinda hard to type about much easier to video chat about
```

---
## \#38 Posted by: Andy87 Posted at: 2018-08-02T01:18:57.326Z Reads: 190

```
Sorry no Skype. Only phone and it’s 3 in the night in Germany 😅
Look here
![image|690x318](upload://gY318gfJMbmHgl0w1RqSn6vIjM9.jpg)
Set multiple vesc over can to true in both controllers 
Plus one need to have the id 0 and one the id 1
Try this, should work after
```

---
## \#39 Posted by: Dogman1247 Posted at: 2018-08-02T01:20:12.042Z Reads: 180

```
thats what ive been using, I will upload a video of my issues in about 30 minutes
```

---
## \#40 Posted by: Andy87 Posted at: 2018-08-02T01:22:58.265Z Reads: 180

```
Forgot, there is a ppm wizard in the new vesc tool.
Did you try to set up with it? 
There you guided through the process.
```

---
## \#41 Posted by: Dogman1247 Posted at: 2018-08-02T01:25:11.018Z Reads: 172

```
ya been using the wizard motor setup and then input setup wizard basically the video word by word
```

---
## \#42 Posted by: Bobby Posted at: 2018-08-02T01:57:26.442Z Reads: 170

```
I feel your pain and was honestly in the same boat until I was fed up feeling helpless. Did the same as you did... got on this site read up, watched videos and asked questions. It’s always scary at first but this site really is a godsend.....I personally would just reflash both Esc’s and start motor detection and all that using  split ppm. Set up one ESC, then do the other exactly the same way and theennnn add the split servo (one 5v wire clipped)  I wish you nothing but good luck and hopefully you ride soon!
```

---
## \#43 Posted by: Bobby Posted at: 2018-08-02T02:00:04.791Z Reads: 166

```
Another tip... make sure you never have any exposed wires... i didnt realize my motor was eating away at one of my phase wires and now i have a drv failure 😩. One blown focbox but a wealth of knowledge gained from that experience lol
```

---
## \#44 Posted by: Dogman1247 Posted at: 2018-08-02T04:32:10.210Z Reads: 171

```
I really dont wanna go the ppm way.... i dont want to do any wiring at all...

im going to sell this thing once i get it working if your interstred
```

---
## \#45 Posted by: Mikenopolis Posted at: 2018-08-02T04:46:04.547Z Reads: 174

```
I’m sure a bunch of us on this forum would buy your “broken” board at a broken board price!

I thought Ernesto is communicating now. Did he just pop up and make a comment and left?!

Look for the “cheap or free request only” thread and ask for a split ppm cable it’s not hard to make for most of us if we have the cables on hand

https://www.electric-skateboard.builders/t/wanted-cheap-or-free-in-progress-requests-only/60454
```

---
## \#46 Posted by: Bobby Posted at: 2018-08-02T06:32:07.996Z Reads: 171

```
Go to your local hobby or rc car store and buy ine for like 5 bucks.  I bought a splitter and the two wires that connect to the vesc and splitter.
```

---
## \#47 Posted by: Dogman1247 Posted at: 2018-08-02T08:20:38.605Z Reads: 166

```
gotcha thanks, ya ernesto popped in and left a comment, can see he has been watching the post got a text from him last night but saying he will make quick guide with screenshot but he is quite elusive and hard to get ahold of.

I am going to attempt to try this can bus system, Once I get it going im going to sell this thing if you know anyone thats in the market can send you some videos and facetime with ya if youd like
```

---
## \#48 Posted by: Photorph Posted at: 2018-08-02T09:17:38.487Z Reads: 156

```
[quote="Dogman1247, post:47, topic:63276"]
but he is quite elusive and hard to get ahold of.
[/quote]

This should not be the case given how much the board costs, builders who sell boards should have a max response time of 2 days.  If they can't sustain that, then they need to hire more people and focus more on customer service rather than just selling boards.  If you start a business you have to be prepared to answer questions from customers, no matter how silly they are.  And yours were actually valid concerns and issues. 

You paid a lot of money for that board, expect good customer service and don't settle for being ignored.
```

---
## \#49 Posted by: Dogman1247 Posted at: 2018-08-02T09:20:25.293Z Reads: 160

```
well put ive been waiting a few weeks he has sent me a new vesc is pretty sweet, But failed to include any instructions of any kind.

All in all in over it defiantly not worth it, super fast fun board when it works, but Ive had so many issues, breaking down on me, leaving me stranded, parts breaking, motor issues, I cannot trust the thing to not leave me stranded somewhere, for 2300$ I believe I paid could use that money and buy a pretty nice motorcycle or a cool vacation,
```

---
## \#50 Posted by: Photorph Posted at: 2018-08-02T09:33:51.792Z Reads: 160

```
Yea, this is why I've stuck to reliable boards like boosted.  I have really wanted a Kaly but recently I ordered a Lacroix, those guys have fast responses and excellent customer service (I hope it stays that way!)

It's great that he sent you a new VESC, but I think the assumption that you will read and learn how to do it yourself should not be made.  The $2300 you pay is a lot of money, part of that is for post purchase support.  So what are your plans with the board now?
```

---
## \#51 Posted by: Dogman1247 Posted at: 2018-08-02T09:36:09.270Z Reads: 158

```
well If I cant fix it, Im going to sell it either way fixed or not... If It does not sell Im planning on making a video of me drenching it in gasoline then shooting it with my rifle until it blows up.
```

---
## \#52 Posted by: Photorph Posted at: 2018-08-02T09:40:15.954Z Reads: 155

```
haha good plan.  But seriously...I would make sure it gets fixed.  Ernesto has to help you out asap and resolve it quickly.  If he doesn't take care of his customers, his business won't last long.
```

---
## \#53 Posted by: Andy87 Posted at: 2018-08-02T09:44:06.299Z Reads: 154

```
I can’t agree with you about boosted.
My battery stopped to charge after 250km.
I‘m now in clearance with them already 2,5weeks.
Each mail took about 3-5days to get reply. 
Sure better tan no reply but till everything is managed summer gone...

About the kaly built just want to let something here:
The 2300dollars not too much for a trampa premium build. All parts already 1500$ minimal. 
I think 800$ to put everything together and design is not too much.
```

---
## \#54 Posted by: Andy87 Posted at: 2018-08-02T09:48:56.195Z Reads: 157

```
For sure Kaly should take care about his customers, but no need to fire it too early😂
My trampa build just burned down some days ago.... can’t see this burning decks anymore.
Always breaks my heart 😭😂
I still don’t understand why it’s not working with your setup...
But honestly, the worst thing which can happen, just buy two new focboxes for 150-180$ and all board will be running like new.
You only have a problem with the communication between your controllers
```

---
## \#55 Posted by: Andy87 Posted at: 2018-08-02T09:49:33.145Z Reads: 155

```
How is your status at the moment?
You made some more trouble shooting?
```

---
## \#56 Posted by: Dogman1247 Posted at: 2018-08-02T09:50:48.166Z Reads: 154

```
I think the vescs are fine (I think) , Im having some issues with using vesc tool and configuring them, 


I just want to ride the board im always fixing this silly thing.
```

---
## \#57 Posted by: Andy87 Posted at: 2018-08-02T10:02:20.722Z Reads: 151

```
I more used to work with bldc tool (the old version) but started with vesc tool too.
Usually you just do like you did.
First motor wizard 
Than ppm wizard
In ppm wizard you chose dual set up and configurat master or slave
After you maybe add your Bluetooth module if you have but that’s all
Where is the Problem?
I mean where you stuck?
```

---
## \#58 Posted by: Dogman1247 Posted at: 2018-08-02T10:03:38.157Z Reads: 150

```
would be best to facetime/skype with you to walk me through it
```

---
## \#59 Posted by: Kaly Posted at: 2018-08-02T12:54:59.811Z Reads: 155

```
First thing 
I have help him a few times already. 
Never have any issues giving advise. 

With all my clients I put a lot of effort on providing support, service and I cover shipping cost and part cost during the warranty period. 

I try to put the best parameter combination for the board on the setting. 
If after a year the  customer wants to modify the software on the board and put its custom settings and software it has to be a **50/50** deal or at least a **30/70** deal when it comes to the understanding of the software and hardware. 

The customer should _**Read**_  the documentation and understand the _**Software**_  and _**Components**_  before _**moving on**_ to working on modifying the device.

* If you contact boosted with a modified version on their software, let me know what the response is.

I’ve try to get him to go over the software and hardware, to move along with the configuration. 

Some time ago Via FaceTime we reprogrammed a VESC and while configuring the second VESC, his computer crashed midway uploading the firmware, I send a replacement FOCBOX for **_free_**. 

Now the bottom line is that I don’t mind FaceTiming and giving the support ANYTIME ( ask my clients ) , but we need to be at least on the **_SAME PAGE_** :-)  when it comes to the basics of the software and device. 

This way we all can move along without issues and can _**troubleshoot**_ simple problems.
```

---
## \#60 Posted by: Dogman1247 Posted at: 2018-08-03T04:12:26.459Z Reads: 153

```
Thank you for walking me through it and getting it back up and working again I appreciate it, I will mail you back the other vesc thanks for sending that.

I did contact you many times via text and call for weeks no answer, Jun 9- jun 26th no response, june 27th sends new vesc
July 6nd I ask if vesc arrived you said you sent it, it arrives. with no instructions.

call texted, instagram, nothing no response until july 29th when I made this post on the forums, 

 I created this topic and joined the esk8 builders website because I have not been able to get ahold of you.
 I think the forums work best for you. 

As far as modifying the board I never have or wanted too because of my lack of knowledge with these esk8's I have had to learn due to it breaking down on me all the time, Motor issues, the pulley, blown vescs, 

I have sent the board into you twice now and I appreciate you splitting the shipping cost with me, However when I get it back it will work for a week or two then have another issue, I fix this thing more than I get to ride it. 

My computer never crashed when loading firmware to other vesc, the bldc tool for it stopped working.

Thank you very much for facetiming me today and getting the board back up and running did a test run it seems to be going well,  

If anyone wants to buy it, it is for sale. 
feel free to message me on here for details
```

---
## \#61 Posted by: Photorph Posted at: 2018-08-03T04:27:35.877Z Reads: 145

```
glad that Kaly got back to you and got you going again.  You can sell the board in the US pretty easily, specially to someone in NYC since they can get a hold of Ernesto easily by walking up to his shop.
```

---
## \#62 Posted by: Dogman1247 Posted at: 2018-08-03T04:29:04.370Z Reads: 148

```
that would be the best way to do it, If I lived in nyc 

just expensive shipping it to and from hawaii all the time
```

---
## \#63 Posted by: Dogman1247 Posted at: 2018-08-03T04:30:08.950Z Reads: 151

```
Here it is for sale PM for details I will upload better photos and videos of it,

can facetime with you if you would like to see it live and I can hook it up to vesc tool etc.

located in maui hawaii.

![IMG_4710|375x500](upload://27d5WheYIQm9hmhLXDbhJHaWmX6.jpg)![IMG_4709|375x500](upload://7su8XJ0ZP1DvNIju5OYQ9puNiJB.jpg)![IMG_4708|375x500](upload://kvLaoUWLJ6XKhvNVu1L2UO5nSsK.jpg)![IMG_4711|375x500](upload://z6V1gMCBuCswXsj9WQmYDzrrsea.jpg)![IMG_4712|375x500](upload://cPLCgKLRDfFl0OfpeWRXj45AInU.jpg)![IMG_4707|666x500](upload://gt9xB3PKuE2C72paWyU4JeoKaji.jpg)
```

---
## \#64 Posted by: Photorph Posted at: 2018-08-03T04:36:14.292Z Reads: 145

```
Make a new thread for it, also would post it on the reddit for sale section. 

https://www.reddit.com/r/ElectricSkateboarding/

 I would also post on craigslist and facebook market place.  Just increases visibility.
```

---
## \#65 Posted by: Andy87 Posted at: 2018-08-03T05:07:10.766Z Reads: 143

```
What was the problem in the end?
How you fixed it?
Why motor detection failed in bldc mode?
```

---
## \#66 Posted by: Silverline Posted at: 2018-08-03T06:53:27.992Z Reads: 135

```
Looks like the trucks is turning the wrong way ? When using regular skate wheels it's okay, but not with AT wheels ?
```

---
## \#67 Posted by: okp Posted at: 2018-08-03T06:55:31.418Z Reads: 138

```
no, that's the way I've been riding on all my custom builds and videos. No worries with the truck hanger mount. I did it because it gives a more roadster look to the board.
```

---
## \#68 Posted by: Silverline Posted at: 2018-08-03T07:02:34.919Z Reads: 138

```
Yeah it looks greate. But it was my understand , that you change the angle ?
```

---
## \#69 Posted by: topcloud Posted at: 2018-08-03T13:59:06.900Z Reads: 142

```
I'm 6' 2", 190, and I ride my Kaly Trampa almost every day, always on thane (ABEC 97s), always on Kalifornian roads. 

I'm not in NYC and I bought my board from a friend of Ernesto's here on the forum; so, no connection to the builder.

In the past year or so I've experienced two problems with my Kaly Trampa:

* One time, when I was jumping the Kaly off of curbs from wet grass into the street, I slid into a recessed manhole cover that caught my back wheel, which flipped my board like 3-4 times while it tumbled down the road and the XT90 safety key fell out.

* Another time, when I was doing about 8 MPH in pitch dark and probably a little high ;) I hit a speed bump and the Trampa deck just perfectly absorbed all that energy and catapulted my dumb ass into the air where I did the full Air Jordan.

I'm sorry that you've experienced problems, yet in my experience, my Kaly is the toughest DIY board I have.  This pic is from the other day.

![c%25XdmsYITPShwfJyZuo2sA|375x500](upload://bXU9grXvIKVncf2MtkJdBhAbiMO.jpg)

I wish I had a use for another one, good luck on the sale bro.  There's nothing wrong with finding a local retailer, buying an Evolve, immediately upgrading it and then, winding up back here.  

Everybody goes through this, it's healthy lol.  Be well!
```

---
## \#70 Posted by: Eboosted Posted at: 2018-08-06T06:02:04.051Z Reads: 126

```
All eboards will fail, no one will work perfect forever, remember this boards are subjected to extreme vibrations, dust and water everyday. However, 98% of problems can be fixed or diagnosed with a basic troubleshoot procedure.

I suggest you look help on the forum if you ever encounter a problem. If you don't have any knowledge at all then all you need is the willing to fix it and follow the recommendations from people around here, believe me this forum is crowded with so many nice fellows eager to get you back on the road, much more than other forums out there.

Of course you could also not be that flexible and demand support exclusively from the builder, post publicly how bad the communication with him is, but this won't help you enjoy this hobby and might lead to frustration.

@kaly is a true innovator and we all have respect for his work, he needs to give support to hundreds of boards out there so he might not available right away but he will get back to you
```

---
## \#72 Posted by: Andy87 Posted at: 2018-08-15T20:56:20.247Z Reads: 101

```
Maybe we can help you here if it’s just an easy question?
```

---
