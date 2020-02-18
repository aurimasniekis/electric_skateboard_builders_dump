# Enertion DIY Assembly Help

### Replies: 66 Views: 7796

## \#1 Posted by: chap Posted at: 2015-09-21T01:28:59.486Z Reads: 179

```
Greetings Crew,
I’m building a pintail eboard, in the traditional wood longboard style.  Small enough to carry, just big enough for stability.  I had the deck made at croozerboards.com, and was very happy with the experience - he did exactly what I asked for, good price, fast turnaround, good communication.  Fun all around process.  

As far as the build, I’m somewhat of a DIY guy, but really didn’t want to get involved in a ton of research, and frankly had a fear of getting stuff that wouldn’t work with other components.  With that in mind, I went with enertion after seeing the clean battery and ESC aluminum enclosures in the videos, and plug and play setup.  Only issue is that the power kit was not currently available due to components being rebuilt.  I ended up waiting, and was then told that I could buy the updated components separately.  They were a bit pricey, but I just wanted stuff I knew would work together, so I did it.  

Only problem is what I received were more of one-off components that don’t have plugs / connections that match eachother, and don’t have mounting attachments or the aluminum enclosures.  There is also zero documentation, and the enertion videos don’t pertain to these newer components at present.  So now, here we are - instead of cruising around town on the board, I'm a bit frustrated in having to dump more time / research / assembly into this.  Anyways, I would love a touch of insight from you all on how to pull the rest of this off, if you’d be so kind.

Here’s what I have (pics to follow)
1 croozerboards pintail
1 enertion dual rear motor mechanical kit
2 rspec enertion motors
2 enertion vesc’s
1 enertion spacecell battery
1 quick charger
1 gt2b transmitter & receiver

I'm trying to upload images, but it is telling me new users can't upload images.  I'll comment on a few topics, and come back to add images, unless someone can authorize me to post the component layouts etc.
```

---
## \#2 Posted by: lox897 Posted at: 2015-09-21T01:37:16.344Z Reads: 159

```
Did the enertion motors come with 5.5mm gold connectors? It's a packet of these gold looking things.

If not then you will need to use connectors and solder them on.
You will need: 

XT60 Connectors MALE from HobbyKing or another place that you can find (post the link so we can double check)

If there wer no 5.5mm gold connectors that came with the enertion motor you will need those aswell.

COULD SOMEONE PLEASE CORRECT ME IF THE SPACE CELL HAS XT90?
```

---
## \#3 Posted by: lox897 Posted at: 2015-09-21T01:38:19.592Z Reads: 148

```
You will also need to configure the VESC with the BLDC tool. There are a few posts on this forum on how to set it up depending on what operating system you have.
```

---
## \#4 Posted by: lox897 Posted at: 2015-09-21T01:43:24.351Z Reads: 144

```
I know it sounds hard but there are a lot of vids and tutorials out there. GOOGLE is your friend! :stuck_out_tongue_winking_eye:
```

---
## \#5 Posted by: chap Posted at: 2015-09-21T02:03:04.359Z Reads: 144

```
Whoa - love how willing to help you are.  An honest thank you.

Yes, the enertion motors came with 5.5mm gold connectors.  I don't know where to solder them to on the ESC, however.  (Will upload a photo of my parts as soon as I'm enabled on this form due to being a new user)  

I think the lack of any sort of documentation is my main holdup.  Well, that, and where there are plugs (on the battery, or radio control unit), that there aren't reciprocating equivalents.
```

---
## \#6 Posted by: lox897 Posted at: 2015-09-21T02:10:35.667Z Reads: 144

```
Solder them directly onto the board. Have a look at this link and read the product description. There is a picture of where you solder the wires. (sl33py solders his connectors straight onto the pcb you can do this too if you dont want to buy wire) Also post a pic once you solder everything so more experienced people (not me!) can have a look at the soldering job to make sure nothing blows up if a wire comes loose. 

Finally! Here's the link lol: http://www.enertionboards.com/electric-skateboard-parts/vesc-motor-controller/
```

---
## \#7 Posted by: lowGuido Posted at: 2015-09-21T02:18:24.268Z Reads: 140

```
so one side of the VESC has 3 pads on it and that for the motor wires.
https://cdn1.bigcommerce.com/n-yp39j5/zad02/product_images/uploaded_images/20150522-082329.jpg?t=1432249306

its the blue red and yellow parts in this pic
```

---
## \#8 Posted by: chap Posted at: 2015-09-21T02:24:14.674Z Reads: 140

```
Ok, got it re: where to solder the 3 motor wires.

On that enertion ESC diagram (http://www.enertionboards.com/electric-skateboard-parts/vesc-motor-controller/) , what is the thing coming in from the right?  Does a split from the battery connect with one of these black cylindrical looking things (not sure what they are), and then soldered to the middle of the board? 

How does the Radio Control unit connect?  I'm seeing the yellow, red, black wires go to it in lowGuido's diagram, but I don't have those wires coming off of mine, or a connector that seems to match...
```

---
## \#9 Posted by: lox897 Posted at: 2015-09-21T02:26:41.163Z Reads: 135

```
Those are capacitors. You don't have to worry about them to much as they should come with your board. Unless you got the last batch.
```

---
## \#10 Posted by: lox897 Posted at: 2015-09-21T02:30:53.501Z Reads: 141

```
Regarding the radio control unit aka receiver buy this and just plug one into the VESC and one into your receiver.  Here is a link to one you can buy: http://www.hobbyking.com/hobbyking/store/__5491__Flat_26AWG_servo_wire_1mtr_R_O_B_.html
```

---
## \#11 Posted by: lox897 Posted at: 2015-09-21T02:32:05.930Z Reads: 139

```
Connect in channel 2
```

---
## \#12 Posted by: lowGuido Posted at: 2015-09-21T02:32:38.808Z Reads: 140

```
so in that image you mention..
<img src='/uploads/db1493/original/1X/c20e7b95a4fa7a69e92b833eddaf9eb7afcda72d.jpg'>

the red and black wires are where the battery connects to the VESC. (Im gonna assume that cannecting the battery wired direct to where the FETS are on the board maximizes current to the FETs while also minimizing PCB space. it also maximizes annoying places to have to solder as a side effect)
the Caps (black things) sit in parallel with the battery. you can think of the caps like a battery but faster. they take care of the surge that the batteries cant.

im surprised you didnt get the receiver wires.. that should have been the easiest part to connect.
```

---
## \#13 Posted by: chap Posted at: 2015-09-21T02:33:42.959Z Reads: 139

```
Here are my parts.  So, still unclear on how the battery and Radio unit connect given these plugs.<img src="/uploads/db1493/original/1X/552eb19041a10861854a9728fbfa77919516697f.png" width="466" height="500">
```

---
## \#14 Posted by: chap Posted at: 2015-09-21T02:35:02.841Z Reads: 131

```
And it still seems like the capacitors would be integral, given they came with this specific kit
```

---
## \#15 Posted by: cmatson Posted at: 2015-09-21T02:35:40.591Z Reads: 132

```
you will need to get a servo cable and then solder it on to hook it up to a receiver. The VESC really isn't that complicated, but it will take soldering, and some reading(read some of the VESC posts here on the forum about how to connect two of them together, and just the setup process in general). 

Here is a thread on wiring stuff while keeping it neat: http://www.electric-skateboard.builders/t/cable-porn-ohhhhh-yeahhhh/198

Wiring the capacitor + motor wires shown in this pic:
<img src="/uploads/db1493/original/1X/3c22402b9747cf35562b10e884cd2be7695c6825.png" width="690" height="487"> 

Also read up on some other build threads because they will definitely help: I know you don't want to do research, but that's part of the DIY way... you have to learn how to do it yourself, and there may be some challenges. You will not regret getting the enertion hardware though: it's basically the best out there. Good luck!
```

---
## \#16 Posted by: lowGuido Posted at: 2015-09-21T02:38:39.022Z Reads: 128

```
I think the issue here is that @chap wanted plug and play. what he got was a crash course in electronics (and programming soon as he loads linix)
```

---
## \#17 Posted by: cmatson Posted at: 2015-09-21T02:39:33.080Z Reads: 125

```
ya, It happens- But make sure @chap you know there is a version of the BLDC tool for windows and mac to you don't need to load linux
```

---
## \#18 Posted by: chap Posted at: 2015-09-21T02:42:45.526Z Reads: 131

```
Ha - indeed

Ok, well thanks here guys.  You've helped me get over a couple of the hurdles that were snagging me.  Will keep you posted on the end result.  And again, a sincere thank you for your all's willingness to help.
```

---
## \#19 Posted by: lox897 Posted at: 2015-09-21T02:45:09.761Z Reads: 131

```
I don't think @chap knows where to solder the receiver wires. Maybe someone could post a pic for him.
```

---
## \#20 Posted by: cmatson Posted at: 2015-09-21T02:46:59.245Z Reads: 137

```
lowGuide's pic shows it pretty well: three wires, in three specific holes on the corner: it's pretty easy to see in the pic

Also color coding for the win!
```

---
## \#21 Posted by: lox897 Posted at: 2015-09-21T02:52:18.853Z Reads: 131

```
Noticed that after I posted the comment. Thanks cmatson.
```

---
## \#22 Posted by: cmatson Posted at: 2015-09-21T02:54:43.669Z Reads: 139

```
Everyone has to start somewhere!

so basically here is what you'll have:

two motors connected on the propulsion kit (enertion has an assembly video about it)
the motor wires going to each VESC (use bullet connectors so you can detach the motors when needed)
*one* VESC with a servo wire going to a receiver, and both the VESCs connected over CANBUS (also a thread on how to do that- just search up connecting VESC over canbus) 
each vesc with it's own capacitor and +/- leads coming off (like in the pic I showed)
those two sets of +/- wires merged together into one +/- (as shown in the @longhairedboy sexy cable thread...) 
that +/- leading into the space cell with an xt60 connector. If you are in the states, I will ship you two deans connectors (similar performance to xt60) for free if you pay shipping: I have so many of them, and I just don't know what do with them all... lol. They look like this, and are slightly smaller than an xt60: <img src="/uploads/db1493/original/1X/452cd6841f8151aaed7d85d811e39933a29dfc79.png" width="358" height="318"> 

Then it is just about making an enclosure! ( @psychotiller has a pretty sweet one for sale made for a space cell + VESCs)
```

---
## \#23 Posted by: onloop Posted at: 2015-09-21T03:10:52.732Z Reads: 130

```
Hey chap!.

Welcome to the forums, 

Sorry about the lack of documentation... to be honest I just don't have time to make any detailed documents - I'm just one guy here.. However I do try to get most of the import info that is required posted up onto this forum and if I don't post it the other members here put info up too..... and by the looks of it the quality of the help you have recieved from everyone is world class! Big thanks to everyone on here!

Regarding the VESC not coming with wires and connectors... well that's a long story.

Basically the supplier had crap wire which I refused, I ordered the correct stuff and was going to solder it for everyone myself. But my wire order was delayed. The vesc was already delayed at thus point and I was about to go away for 3 weeks. 

So basically I had to ship what I had. Otherwise the weeks would just keep rolling by without people getting their orders... most poeple don't like waiting.

It would have been delayed until mid October.

I hope you get everything sorted!.

Eventually I'll have a complete kit ready to go... but it's not as easy as you would think. Making complex things simple is an art form... it takes time to do it right!... 

Kind regards Jason.
```

---
## \#24 Posted by: cmatson Posted at: 2015-09-21T03:24:12.615Z Reads: 123

```
on a side note, will your October batch of VESC's have the wires pre-soldered?
```

---
## \#25 Posted by: sl33py Posted at: 2015-09-21T04:28:16.486Z Reads: 126

```
@chap - welcome to DIY!  You got some great kit and are almost there!

Do you have a decent soldering iron already?  You really will need one for the heavier gauge wires you will want for power and the VESC's.

On a previous order of the VESC's direct from Vedder he sent a link to a youtube video showing him soldering up one.  I found it helpful the first time i did one, so watch it and hopefully it helps you as well.  That's at least the hardware side of it...
https://www.youtube.com/watch?v=-fyj5TxxoU8 

Connectors - i'd recommend picking a standard and not mixing connectors if you can help it.  Besides the 5.5mm bullet connectors to the motors, all your other connectors should be the same.  it will make things easier down the road.  With the SPACE cell you don't have the same issues since the charging is all through the BMS (which is nice).

Have you started looking at the programming of the VESC?  It seems a bit daunting the first time, but it's really pretty easy now with some versions ported to Windows and Mac.  You just need to make sure the version of the ported BLDC tool match your firmware on the VESC's.

HTH - GL!
```

---
## \#26 Posted by: chap Posted at: 2015-09-21T04:51:31.277Z Reads: 118

```
@cmatson and ALL - VERY helpful, and thanks for meeting me more than half way on this stuff.  Cheers

cmatson, I'll shoot you a pm to get your paypal / venmo on shipping that connector.

Cheers, Guys!
```

---
## \#27 Posted by: lox897 Posted at: 2015-09-21T14:06:29.576Z Reads: 102

```
Correct me if I'm wrong but... Deans connectors are not rated for a 60amp current. People have said all over forums that deans connectors melt, catch fire etc)

I really would go with XT-60 just to be safe...
```

---
## \#28 Posted by: treenutter Posted at: 2015-09-21T14:29:00.271Z Reads: 102

```
I'm interested in this as well @lox897. I haven't seen any reports of Deans connectors causing fires. AFAIK, Deans doesn't publish an amperage rating; but I see plenty of RC folks pulling 100A (example below). 

So far I've been planning to use Deans, but I'd be switch if there's some info that concludes that something else would be better.

http://www.rcgroups.com/forums/showthread.php?t=590567
```

---
## \#29 Posted by: lox897 Posted at: 2015-09-21T14:48:31.491Z Reads: 102

```
Deans Ultra have been reported to pull 100amps but normal Deans are supposed to be terrible and hard to pull apart.

One guy said this: 
The Deans Ultra plug is rated for 60A continuous and 75A burst. Use bullets as I have already crashed twice using them. They tend to pull apart inside the housing with continuous high amperage currents.

There are heaps of videos on them failing and I have heard lots of people on RC forums are switching to XT-60 for reliability.

i am always going to use HXT-4mm, XT-60/90 or EC3/5
```

---
## \#30 Posted by: lox897 Posted at: 2015-09-21T14:57:16.396Z Reads: 100

```
This is what HobbyKing said: These are for those customers still stuck with the old t-connector.
We suggest all customers to upgrade to the new XT-60 connector where possible as that is the connector attached to nearly all our batteries, esc, charger and models.
```

---
## \#32 Posted by: King1017 Posted at: 2015-09-21T15:54:52.439Z Reads: 98

```
I am interested in knowing this as well.
```

---
## \#33 Posted by: lox897 Posted at: 2015-09-21T15:58:41.620Z Reads: 100

```
How's your build going?
```

---
## \#34 Posted by: treenutter Posted at: 2015-09-21T16:07:28.610Z Reads: 95

```
@onloop also posted a pic in this thread of the wiring for a GTB2 to VESC http://www.electric-skateboard.builders/t/what-is-the-best-2-4ghz-controller-for-vesc/155/10
```

---
## \#35 Posted by: King1017 Posted at: 2015-09-21T16:30:47.486Z Reads: 92

```
I wasn't sure if i should upgrade to a dual motor set-up or not, but i have decided to stick with a single for now. I will be ordering all my stuff from Enertion within the week, but will have to wait until October 1st or so it looks like for the Vesc. I have my trucks and wheels so far. My GT2B is on its way to my house and i am still debating on the board itself, but i plan to pick it up today.
```

---
## \#36 Posted by: lox897 Posted at: 2015-09-21T16:38:22.302Z Reads: 89

```
Nice! Good luck! Remember to make a build thread once it's done or while you are doing it!
```

---
## \#37 Posted by: King1017 Posted at: 2015-09-21T16:44:27.002Z Reads: 86

```
For sure. Do you have any builds posted? Always looking for insperation.
```

---
## \#38 Posted by: lox897 Posted at: 2015-09-21T16:48:47.310Z Reads: 92

```
Yep. Mine isn't done yet. Waiting until Christmas to finish it. (I'm 12)

Here's a link for what I've done so far:
http://www.electric-skateboard.builders/t/my-eboard-build-wip/187/3
```

---
## \#39 Posted by: cmatson Posted at: 2015-09-21T16:53:58.505Z Reads: 91

```
I have used deans on everything I've every built: Two 8th scale rc cars pulling 150amps, and two eboards(a 6s build and a 10s build). I've never had then melt, get stuck together, or be too hard to take apart; ya they can stick a little, but it's not a huge deal, especially when you use a space cell and rarely need to separate them. 

haha if you don't want them, don't buy them! you can always get xt60s or 90s (I have some xt90s that I wanted to try out, but they are SOOO freain big...).
```

---
## \#40 Posted by: lox897 Posted at: 2015-09-21T17:01:52.721Z Reads: 93

```
@cmatson I just watched your "How to build an electric skateboard" video. I am going to use that method that you used for the batteries. Great idea!
```

---
## \#41 Posted by: cmatson Posted at: 2015-09-21T17:10:26.927Z Reads: 97

```
Awesome! it's pretty rock solid!
```

---
## \#42 Posted by: sl33py Posted at: 2015-09-21T17:41:21.261Z Reads: 100

```
i ran deans for years - great connectors and nothing i'd hesitate to use.  I prefer the soldering especially of the XT 60/90's over the deans.  Especially when 12/10awg wire is used.  Just easier IMO.

Pick one and you are set.  Nothing to avoid as long as you are using good/appropriate wire gauge and good solder connections on the connectors.  It's hard to solder big wires without a good solder iron!  Need a lot of heat as the thick wire pulls it away quickly.

GL!
```

---
## \#43 Posted by: treenutter Posted at: 2015-09-21T17:54:25.665Z Reads: 104

```
Thanks @sl33py and @cmatson that's good to hear! There are many conflicting opinions about connectors.

@sl33py I completely agree re: having a good soldering iron. I just upgraded to a 60-watt soldering iron with swappable tips. The wide tips and strong heat make soldering large wires much easier, and the result is far better!

Has anyone tried using xt60 with 10AWG? It looks like it doesn't fit (see pic below), but some folks report that it works. @cmatson you're right xt90 are huge!

<img src="/uploads/db1493/original/1X/d7f12fb7317521dea8686d24a2838b352631a26f.jpg" width="600" height="388">
```

---
## \#44 Posted by: sl33py Posted at: 2015-09-21T18:08:08.726Z Reads: 97

```
XT60 really maxes at 12g.  I used XT90's with 12/10.

XT90's are pretty big but i have big hands and like the grip.  Also with the XT90 anti-spark it's worth the larger plugs throughout IMO.
```

---
## \#45 Posted by: claudiofiore88 Posted at: 2015-09-21T20:48:21.006Z Reads: 92

```
The xt90's are huge indeed. I wish they made xt60's with the built in anti spark. I hated the dean's connectors. I found them difficult to plug into one another and easy to ruin with too much heat or too long of applied heat with the soldering iron. I hated soldering them.
```

---
## \#46 Posted by: lowGuido Posted at: 2015-09-21T21:01:51.181Z Reads: 93

```
I have used deans connection on every board i have made. None have melted or become damaged. They are just so much more compact than anything else. I have had up to 10AWG on with no drama.
```

---
## \#47 Posted by: cmatson Posted at: 2015-09-21T22:13:31.394Z Reads: 87

```
yep, if you just solder them quickly, and don't fiddle with the same solder joint for 30 minutes, they won't give you any trouble. Plus, they are a dime a dozen if you do screw one up
```

---
## \#48 Posted by: lowGuido Posted at: 2015-09-21T22:30:25.291Z Reads: 90

```
yup. get your solder game on point! use a good quality iron that can heat instantly so there's no messing about.

if you mess around and keep the heat on for too long then you can start to melt the plug, and that's no good. 
Rookie mistake.
I think a lot of people are lacking in soldering skills and then blame the connectors when it turns to shit :smile:
```

---
## \#49 Posted by: claudiofiore88 Posted at: 2015-09-21T22:50:01.819Z Reads: 90

```
I have an [X-Tronic #6040][1] soldering iron, so it's not a bad soldering iron.  I've found that connecting the opposite connector while soldering acts as a heat sink and pretty much eliminates melting of the connector.  What I don't understand is what temperature to set the iron at when doing various soldering.


  [1]: http://www.xtronicusa.com/home/#!/X-TRONIC-6000-SERIES-MODEL-6040-HOT-AIR-REWORK-STATION/p/9238596
```

---
## \#50 Posted by: lox897 Posted at: 2015-09-22T02:54:11.410Z Reads: 88

```
@lowGuido I have never used Dean's so I was basing my comment on what has been said on forums.
```

---
## \#51 Posted by: cmatson Posted at: 2015-09-22T04:33:35.670Z Reads: 87

```
no worries-

and just in general, before totally throwing something under the bus, at least keep an open mind to trying it for yourself first. I actually haven't seen anywhere that a deans connector has caused a type of failure on a board...and I have been reading ES posts for about 6 months. Yes, they can pull apart from vibrations because they are held together by friction, and yes, they have small solder tabs so they can be more difficult to work with. But at the same time they are dirt cheap, and perfect if you just want to buy a set of like 40 of them and be good to go for a while without ever worrying about connections...  

I know people screw up with soldering, but that isn't the connectors fault: heck, you can destroy an xt90 of you fiddle with it for too long with you soldering iron- they are all just plastic; regardless of the size. 

If you: solder them correctly and (depending on situation) wrap your final product in electrical tape (I did this on my space cell build because I knew I wasn't going to be unplugging it a lot), they are completely fine.
```

---
## \#52 Posted by: lowGuido Posted at: 2015-09-22T05:35:56.254Z Reads: 82

```
No Offence meant @lox897 but have you even ever built an electric skateboard? I think you base all of your comments on what you have read on forums.

Edit: I'm sorry if that came across a bit harsh.
```

---
## \#53 Posted by: lowGuido Posted at: 2015-09-22T05:39:11.790Z Reads: 83

```
@claudiofiore88 for small joins like servo cables set around 200C and for things up to 10awg i crank it up to around 300C-350C but get in and out quick.
```

---
## \#54 Posted by: lox897 Posted at: 2015-09-22T12:48:09.227Z Reads: 82

```
A few replies above I have a link to one
```

---
## \#55 Posted by: lox897 Posted at: 2015-09-22T12:49:45.416Z Reads: 86

```
I know. That's what I was thinking the whole time I was posting comments and ai knew someone was going to comment on that. Anyway, I was basing my opinion on other opinions on Deans so one day I will try it and give you a different opinion, maybe. :smile:
```

---
## \#56 Posted by: lox897 Posted at: 2015-09-22T13:00:24.442Z Reads: 90

```
Here it is: http://www.electric-skateboard.builders/t/my-eboard-build-wip/187
```

---
## \#57 Posted by: SwissFozz Posted at: 2015-10-18T20:33:15.391Z Reads: 98

```
Hi chap and everyone else.

I have a related question to this thread on the motor to VESC connections. 

Assuming that good connections can be made, how do you know which wire from the motor connects to which connector? I have three cables coming off the motor, all black, nothing distinguishing one from another. Does it matter which gets connected where?

All help appreciated!
```

---
## \#58 Posted by: lox897 Posted at: 2015-10-18T21:00:43.828Z Reads: 102

```
No. If your motor is going the wrong way just switch any 2 wires. I'd use connectors and not solder straight to board because if you have to switch then that would be annoying. I think there is also an option in the VESC settings to reverse the spinning.
```

---
## \#59 Posted by: chap Posted at: 2015-11-02T20:44:44.080Z Reads: 105

```
Guys - life was been kicking my ass the past couple months, and this project had to be put on hold, but I've come up for air now, and anxious to finish this thing up.

As a refresher, its a VESC / SpaceCell / Dual Rear R Spec Motors / Enertion Drive Kit on a pintail longboard (see pic).  I have the radio controller, but nothing else... Am looking to make one final order, and get everything remaining I need for final assembly.  

Would you all be so kind to look over this list, and let me know if I need anything else, or if you'd do something differently?

Soldering iron kit - (60w $15)
http://www.ebay.com/itm/14in1-60W-110V-Electric-Soldering-Tools-Kit-Set-Iron-Stand-Desoldering-Pump-/311275130419?hash=item4879718e33:g:wYoAAOSwjVVVyt8e

5.5mm bullet connectors to the motors (included)

XT-90 Connectors (10 pairs: $15)
http://www.ebay.com/itm/10-Pairs-XT90-Battery-Connector-Set-4-5mm-Male-Female-Gold-Plated-Banana-Plug-US-/151680900067?hash=item2350e2dbe3:g:ZWgAAOSw6BtVVHYY


Heat Shrink Tubing ($7)
http://www.ebay.com/itm/127pc-Heat-Shrink-Wire-Tubing-Assortment-Wrap-Electrical-Connection-Cable-Sleeve-/251727383870?hash=item3a9c1f0d3e:g:0vEAAOSwHnFVy9hZ

Electric Tape

Carbon enclosure case? Or how do you all recommend mounting the Space Cell

Anything else I'm missing to finish the complete build?

<img src="/uploads/db1493/original/1X/51adbc2b879346756c2255cf114329e45c94e21f.jpg" width="690" height="499">
```

---
## \#60 Posted by: cmatson Posted at: 2015-11-02T21:51:44.012Z Reads: 97

```
that soldering iron won't do you much good with think wires: it is worth paying a little more because I don't think you can get a strong connection with that one.

even a middle grade weller soldering gun would be 10 times better; I used this one for a while, and it'll get the job done:http://www.amazon.com/Weller-8200PKS-120-volt-Universal-Soldering/dp/B002YDMZF4/ref=sr_1_1?ie=UTF8&qid=1446500689&sr=8-1&keywords=soldering+gun

then just get some solder (because a kit really isn't worth it- you just need an iron + solder) and you'll be good!

The space cell comes with an xt60 on it, and enertion's vescs now ship with an xt60 aswell. so I'd change you 90's to 60's, and see if you can buy like 5 pairs instead of 10 (just to save some $$)

everything else looks good! if you are concerned about spending the extra $ on the soldering iron, then you can always skip the heat shrink tubing, and just use electrical tape- but honesly, a bad soldering iron could ruin your build because all the joints are weak, and would eventually break while riding.

glad you are ready for your build!
```

---
## \#61 Posted by: lox897 Posted at: 2015-11-02T22:33:08.452Z Reads: 90

```
@cmatson Nailed it! I 2nd changing those XT90 to XT60
```

---
## \#62 Posted by: lox897 Posted at: 2015-11-02T22:33:43.262Z Reads: 90

```
Have a look at psychotiller's space cell enclosures.
```

---
## \#63 Posted by: chap Posted at: 2015-11-03T19:27:31.556Z Reads: 90

```
Awesome - orders placed - will keep you all posted, and reeeeeally appreciate the guidance.
```

---
## \#64 Posted by: lowGuido Posted at: 2015-11-04T05:30:44.510Z Reads: 93

```
I was gonna say I'll put it together for you. Or atleast help but theres that geographic divide. .
```

---
## \#65 Posted by: treenutter Posted at: 2015-11-04T16:07:36.248Z Reads: 99

```
@cmatson got it right; get a decent soldering iron. For the thick wire joins (14AWG and up) use a wide tip not one of the pointy ones. Also, I've found that flux paste is invaluable for getting good results with thicker gauges. Even with flux-core solder, I find it helps.
```

---
## \#66 Posted by: chap Posted at: 2016-09-29T20:55:35.614Z Reads: 42

```
(Holy thread resurrection) So here we are - its all soldered up, wired up, and ready to roll - except I'm stuck on the BLDC Tool telling me I need to update my firmware (VESC 4.7), but then after it runs it, it disconnects the VESC, and when I reconnect, its still showing the same original v1.10 firmware.  Have rinsed and repeated many a time, to no avail.

After searching, it appears I need to buy a ST-Link/V@ for STM8 and then reload the bootware or something?  Is there a way I can just use the old firmware, with an old BLDC tool, and get it to work? or is that non-advised.  Just been working on this thing little by little for enough time, and ready to RIDE it at last.

Any help is most appreciated.  

Cheers & Thanks, Guys,
```

---
## \#67 Posted by: chap Posted at: 2016-09-30T12:46:19.374Z Reads: 36

```
@onloop  Any thoughts here?
```

---
