# Help with Stealth &#124; hi5ber, Zenith &#124; Caliber 2 &#124; single R-spec 190kv &#124; Custom Carbon Enclosure &#124; Spacecell &#124; VESC

### Replies: 52 Views: 4583

## \#1 Posted by: King1017 Posted at: 2015-09-15T23:49:49.262Z Reads: 166

```
I am totally new to the diy side of this. I had planned on just purchasing a board but decided I would like to give building one a go instead. 

My goal if possible is to build a single motor board that has a top speed of 22-25mph, and has a range of at least 10 miles. I have been doing some research on components but I would greatly appreciate suggestions on what batteries, motor, and esc. 

I already have a set of 90mm wheels so I am going with that, mounted to a pair of caliber trucks. I also intend on ordering the single motor mount kit from Enertion.

Thanks in advance.
```

---
## \#2 Posted by: onloop Posted at: 2015-09-16T00:01:56.477Z Reads: 146

```
What wheels are they?
```

---
## \#3 Posted by: lox897 Posted at: 2015-09-16T00:07:57.767Z Reads: 143

```
Batteries:
Do you have hills where you will ride? If so you may need 8-12s but you can use this on flat aswell and you will get more torque. If you don't need torque then 6s should be fine for Flats only. You should wire 2 packs in series to make the total S rating. If you have 10S get 2 5S packs and wire in series. If you get 6S wire 2 3S batteries in series.

I would get some help from others for the mah as I don't have much experience there...

ESC: Torque Boards ESC or VESC from enertion. VESC is the best IMO but it requires a bit more configuration to suit your motor. If VESC get the october batch from Enertion.

Motor: TorqueBoards Motor or R-SPEC from enertion. Both come with keyways so you don't have to dremel a flat spot for the set screw to sit flat.

If you have anymore questions don't hesitate to ask.
```

---
## \#4 Posted by: King1017 Posted at: 2015-09-16T00:09:00.062Z Reads: 134

```
Flywheels. They are generics I believe, but I have a nice set of bearings in them.
```

---
## \#5 Posted by: King1017 Posted at: 2015-09-16T00:28:48.506Z Reads: 133

```
I will typically be riding on flats. My original plan was to go with a 6s set-up, but I would rather over build it. Why 2 batteries in series, instead of one? Also any thoughts on the monster mamba 2 esc?
```

---
## \#6 Posted by: lox897 Posted at: 2015-09-16T00:32:52.063Z Reads: 130

```
I think it puts less stress on the motor/s... Double check with others...
```

---
## \#7 Posted by: lox897 Posted at: 2015-09-16T00:34:29.584Z Reads: 132

```
The Mamba Monster can only support up to 6S so if you want to over do it this esc won't work. The ESC's I suggested are made for eboards especially VESC from Enertion so you will get a better result.
```

---
## \#8 Posted by: lox897 Posted at: 2015-09-16T00:35:09.860Z Reads: 130

```
Can you provide a link to the wheels you have so I can have a look?
```

---
## \#9 Posted by: lowGuido Posted at: 2015-09-16T00:45:53.872Z Reads: 127

```
the only reason to wire 2 packs in series over just one pack is because of the lower profile on the board. chemically and electrically they are the same.
```

---
## \#10 Posted by: lox897 Posted at: 2015-09-16T00:49:11.321Z Reads: 124

```
Thanks lowGuido! I forgot about that.
```

---
## \#11 Posted by: King1017 Posted at: 2015-09-16T01:21:28.062Z Reads: 126

```
http://m.ebay.com/itm/Brand-New-Blank-Pro-90mm-Lime-Longboard-Flywheels-ABEC-7-Bearing-Spacers-/141727700938?nav=SEARCH

They are just like these. Got them off ebay, and picked up the bearings from Zumiez in the mall when I build my son a board for the park.
```

---
## \#12 Posted by: lox897 Posted at: 2015-09-16T01:22:36.746Z Reads: 126

```
They should work. I think @torqueboards uses blank pro's. He may give you some advice on mounting them.
```

---
## \#13 Posted by: onloop Posted at: 2015-09-16T01:34:10.073Z Reads: 121

```
they should be compatible with the 36T wheel pulley we supply in our kits.

Probably just need to drill it out a little with a 6mm drill bit. nothing major.
```

---
## \#14 Posted by: King1017 Posted at: 2015-09-16T01:40:48.970Z Reads: 122

```
Will the r-spec motor fit my criteria for this build? Also can anyone help me with how many mahogany I need in a battery setup?
```

---
## \#15 Posted by: lowGuido Posted at: 2015-09-16T01:46:52.314Z Reads: 119

```
Id start with a minimum of 5000 mahogany :stuck_out_tongue:

(LOL I think you mean mAh mili Amp hours)
```

---
## \#16 Posted by: onloop Posted at: 2015-09-16T01:48:21.236Z Reads: 122

```
read this: http://www.electric-skateboard.builders/t/what-is-battery-c-rating-is-it-important-for-electric-skateboards/36

it has a lot of info about batteries, not much about wood though :smile:
```

---
## \#17 Posted by: King1017 Posted at: 2015-09-16T01:48:44.318Z Reads: 132

```
Haha, that's a good auto correct.
```

---
## \#18 Posted by: cmatson Posted at: 2015-09-16T02:34:23.812Z Reads: 140

```
I have a 5,000mah 6s 25c battery, and I usually get 8 miles off my single 50mm motor. I'd recommend you put two 5000mah in parallel to give you some extra range. The good thing about this is that you can always buy one 5,000mah 6s at first, and if you aren't satisfied with the range it's easy to add a second. 

For the speeds you want though, you may want to go up in voltage (6s -> 8s, 10s, or 12s) to be able to get the speed you want without loosing a ton of torque. Don't get me wrong, it's perfectly doable with a simple 6s setup, but if you can afford higher voltages they are always worth it. Both of my first two builds were 6s, so don't feel pressured into thinking you need all that power- especially with flats. It's just there if you want to go that route.

An enertion kit + 245kv turnigy sk3 63mm motor and 6s should yield around the speeds you are looking for. I have a 245kv setup right now geared 13/36, and I hit 20-22mph (I believe the stock enertion gearing is 14/36 or 15/36 which will be slightly faster, giving you your desired speeds)

For a higher voltage setup (if this is something you'd want, again, it's all personal preference/budget)
I'd get an Enertion 190kv 63mm motor (best motor out there) + 10s (two 5s in series, or an Enertion SPACE cell battery: I have the space cell, and it's pretty legit) + either a VESC esc (it is a little more complex than plug and play, but nothing unreasonable. anyone could figure it out by reading a thread or watching a setup video) or a Torqueboard's 145amp esc. 

Again, the higher voltage means higher cost, but it's also higher performance. If that's not what you want to get into (I totally understand) than 6s is still pretty freakin sweet.

Good luck!
```

---
## \#19 Posted by: King1017 Posted at: 2015-09-16T02:43:16.242Z Reads: 134

```
Cost isn't a huge issue, of course I would like to keep it as low as possible but I always want ro be more than just content with my build. Like I said I was going to shell out 1,300-1,500 for a name brand board before I decided to go this route.
```

---
## \#20 Posted by: King1017 Posted at: 2015-09-16T02:47:52.865Z Reads: 134

```
Where can I find a Torqueboards esc?
```

---
## \#21 Posted by: cmatson Posted at: 2015-09-16T03:12:54.457Z Reads: 133

```
then honestly, in your situation I'd just go the high voltage route. you'll still save 300sih dollars give or take, as a 10s setup of the following set me back 950-1000 dollars in the end with misc stuff like some extra wire and connectors added in:
enertion mount
enertion 190kv
enertion space cell
torqueboard's esc + programming card(I'd get a VESC though- the amp draw on the torqueboard's is a little too much for the space cell, and you can easily blow the batteries fuse) link for ya if you still want to get it, and use it with lipo's (which it works perfectly with): product/torqueboards-12s-120a-car-esc-opto-hv/
castle BEC (will need a 10s BEC to power you remote reciever- don't need it for the vesc though)
abec flywheels 83mm
arbor timeless walnut deck
caliber trucks
flysky GT2B remote 

like I said, the only think I would change is take off the torqueboard's esc ($145+ tax + $20 shipping +the programming card for that which is an extra $15), and the castle BEC ($10-15) for a VESC (simply $120ish). You'd save like $70, and it's a better setup for the space cell (which is well worth it).
```

---
## \#22 Posted by: King1017 Posted at: 2015-09-16T13:04:53.046Z Reads: 133

```
So I think I am going to go with:
Enertion 190kv r-spec motor
Enertion single truck mount
The Space Cell battery (mostly because it seems to be the simplest set up for a new guy)
I will do a Flysky 2.4ghz transmitter 
And I think I will try to do the vesc (but I am a little nervous about setting that up, I'm hoping it won't be to bad.

Does anyone have anything else to add? Except the board and hardware am I forgetting something?
```

---
## \#23 Posted by: longhairedboy Posted at: 2015-09-16T13:10:58.727Z Reads: 126

```
You'll need a box to put everything in. @psychotiller makes these awesome vacuum molded ABS boxes. He might sell you one if you give him some specs. 

I made my own out of fiberglass which was enlightening as well as very smelly. If you're brave you might try that approach as well. 

Also, order extra belts. You probably won't get the pulleys perfectly aligned the first time and if you don't you'll wear out your belts quicker than normal. 

And don't forget the thread locker! Thread lock EVERYTHING.
```

---
## \#24 Posted by: King1017 Posted at: 2015-09-16T13:59:12.399Z Reads: 118

```
I have alot of experience with working with carbon fiber, so I plan to build a box out of that.
```

---
## \#25 Posted by: lowGuido Posted at: 2015-09-16T14:41:09.117Z Reads: 124

```
have you considered making a whole deck from carbon??
I think that will be my next project..
```

---
## \#26 Posted by: King1017 Posted at: 2015-09-16T14:46:31.491Z Reads: 127

```
I have, but for my first go at it I have my eye on a bamboo/fiberglass longboard deck as my starting point. Plus I have never attempted to build a carbon board of any kind. Plus everything else that goes with building an e-board is already an experiment for me. So maybe next time if this goes well.
```

---
## \#27 Posted by: cmatson Posted at: 2015-09-16T17:09:38.025Z Reads: 127

```
VESC isn't as hard to set up as everyone eludes to. Windows, Mac, or Lunux; doesn't matter what you have, it all will work. There are videos on youtube: https://www.youtube.com/watch?v=utZSvkY3Z0U

Edit: didn't mean to reply to you @longhairedboy -meant for @King1017
```

---
## \#28 Posted by: psychotiller Posted at: 2015-09-16T18:28:22.727Z Reads: 130

```
@longhairedboy Thanks for the PR! 
<img src="/uploads/db1493/original/1X/2724aa2e626c969ad0790823e513db1c2e61ae69.jpg" width="646" height="365">
```

---
## \#29 Posted by: King1017 Posted at: 2015-09-17T00:25:07.234Z Reads: 127

```
So does the software already come installed on the vesc? Or is that something that needs to be bought extra?
```

---
## \#31 Posted by: cmatson Posted at: 2015-09-17T01:06:26.641Z Reads: 134

```
don't follow what lox put- it isn't necessary... you don't need all that confusing stuff.

 Just search (on this forum) for BLDC tool. Two forum posts (one for windows, one for mac) will pop up, and you download the BLDC program for whatever operating system you are on. It is as easy as that: one program. @lox897 was linking you to something that comes pre installed on the VESC
```

---
## \#32 Posted by: cmatson Posted at: 2015-09-17T01:09:57.916Z Reads: 135

```
here are just individual files for windows and mac (this is what I did- super easy step)
http://www.electric-skateboard.builders/t/vesc-faq-windows-version-of-bldc-tool/141

http://www.electric-skateboard.builders/t/vesc-faq-osx-version-of-bldc-tool/140
```

---
## \#33 Posted by: lox897 Posted at: 2015-09-17T01:13:22.429Z Reads: 125

```
Thanks cmatson. I will delete post. My bad.
```

---
## \#34 Posted by: cmatson Posted at: 2015-09-17T01:14:02.475Z Reads: 123

```
no worries, all part of the learning process!
```

---
## \#35 Posted by: King1017 Posted at: 2015-09-17T01:30:45.707Z Reads: 122

```
Wow, this site is amazing. I was just totally spoon fed a guide to build one of these. I hope as I go I am able to contribute back to others. Thanks everyone
```

---
## \#36 Posted by: cmatson Posted at: 2015-09-17T01:34:58.993Z Reads: 119

```
everyone's gotta start somewhere! I didn't know of any forums like this when I build my first board a little over a year ago, but man it would've helped me so much. I was 15 building my first board- naturally, I ordered some wrongs things, burnt out a motor, and basically spent $200 over my budget because I was stupid, lol.
```

---
## \#37 Posted by: lox897 Posted at: 2015-09-17T01:56:11.271Z Reads: 119

```
I was 12 when I started my first build and still am 12 except I'm out of spending money. Have to wait until Christmas... :pensive:

I agree with cmatson... I wish I got the Enertion R-Spec from the start so I didn't have to dremel a flatspot on the motor and align properly.
```

---
## \#38 Posted by: psychotiller Posted at: 2015-09-17T02:08:09.840Z Reads: 117

```
That is a nice feature. But if you take your time and do it right it will be solid.
```

---
## \#39 Posted by: lox897 Posted at: 2015-09-17T02:17:34.029Z Reads: 115

```
Yeah. I have an uncle as an engineer so that helps.
```

---
## \#40 Posted by: psychotiller Posted at: 2015-09-17T02:24:23.995Z Reads: 113

```
Make sure to take the motor shaft out to do the work. Metal shavings are the enemy.
```

---
## \#41 Posted by: lox897 Posted at: 2015-09-17T02:36:11.985Z Reads: 114

```
I will do that. Thanks psychotiller your help is much appreciated.
```

---
## \#42 Posted by: King1017 Posted at: 2015-09-21T00:10:34.973Z Reads: 103

```
One more question. I am getting ready to order parts. And now I'm wondering what the benefits would be to running a dual motor set up over a single motor. If I ran 2 motors I plan to order the space cell 2 190kv r spec motors and 2 vesc. If I run one motor I will obviously just get half that and the space cell. Would the dual set up be worth the additional cost? And why?
```

---
## \#43 Posted by: lox897 Posted at: 2015-09-21T00:48:00.803Z Reads: 103

```
If you want more torque and want to be able to go up hills faster then 2 motors is the way to go. Some single motor setups burn out going up hills depending on your weight. Also you can connect your VESC together with CANBUS if you want 2 motors.
```

---
## \#44 Posted by: King1017 Posted at: 2015-09-21T01:01:40.666Z Reads: 102

```
I'm sorry I don't know what CANBUS means. Can you explain?
```

---
## \#45 Posted by: lowGuido Posted at: 2015-09-21T01:12:04.366Z Reads: 106

```
it means you can easily join them together.

with regards to your motor question. If you don't have many hills around, you don't weigh a lot and you want long range, then single motor is the go.
```

---
## \#46 Posted by: lox897 Posted at: 2015-09-21T01:15:01.244Z Reads: 104

```
Here's a guide on it: http://www.electric-skateboard.builders/t/vesc-faq-connect-two-vesc-via-canbus-for-dual-motors/142
```

---
## \#47 Posted by: lox897 Posted at: 2015-09-21T01:28:54.268Z Reads: 100

```
It basically means that instead of using a Y connector to get the 2 VESC to connect to the receiver you use CANBUS and tell the BLDC tool that you are using CANBUS.
```

---
## \#48 Posted by: King1017 Posted at: 2015-09-25T12:11:56.988Z Reads: 104

```
Little update. 

I ordered my deck this week, it should be here by Monday. I'm not going to say what it is yet but I will start a new build thread when it gets here. I also just placed my order through Enertion for: 190kv r-spec motor, Vesc, spacecell battery and charger and a motor mount. My gt2b should be here Monday as well slow shipping, but it is coming straight outta Compton. 

So when parts come in I will be starting a new thread to show my build in detail, which can hopefully in turn help other people who are looking to do the same thing all of you have helped me get started. 

One other question while I'm here. What connector comes on a spacecell? Does the same connector come on the vesc?
```

---
## \#49 Posted by: lowGuido Posted at: 2015-09-25T12:28:36.501Z Reads: 104

```
apparently not at this stage. @Chap had to solder his connectors on to the VESC. check out his thread:
http://www.electric-skateboard.builders/t/enertion-diy-assembly-help/221

I understand that the plan is to get the space cell and the VESC to be plug and play but time constraints and shipping needs and, wait. you have already posted in that topic.

edit: Is it the carbon deck?
```

---
## \#50 Posted by: lox897 Posted at: 2015-09-25T12:44:42.703Z Reads: 101

```
Onloop said that the 4.8 VESC will come with XT60 just like the space cell.
```

---
## \#51 Posted by: King1017 Posted at: 2015-09-25T12:47:23.563Z Reads: 98

```
Yeah all carbon. I will post pics as soon as I get it.
```

---
## \#52 Posted by: lox897 Posted at: 2015-09-25T13:22:13.649Z Reads: 105

```
Good luck! This will be a great build! Can't wait to see it.
```

---
## \#53 Posted by: onloop Posted at: 2015-10-30T23:22:45.880Z Reads: 113

```
In order to make the "E-board Builds" category really easy to search & locate specific builds i am asking that you change your title to something descriptive that better expresses the makeup of your build.

Most of the new build threads tend to end up with a name such as 
**"new- noob - noobie - beginner - first - build - help - newb"** this becomes hard to keep track of.

I would like to see each build thread with a descriptive title, such as;
**Project Name | Deck Name | Trucks | Motor type | Mounting method | Voltage/Battery | ESC**

Example
**The Samurai | Custom Deck | Paris Trucks |  R-SPEC | Custom Mount | 10S | VESC**
```

---
