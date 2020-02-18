# Lipo Battery Issues and Questions

### Replies: 41 Views: 3241

## \#1 Posted by: lilracerboi Posted at: 2016-04-29T22:47:46.457Z Reads: 180

```
Okay so I just got two new Zippy 3S 5000mah batteries in the mail today.
After some past experiences, I've come to fear connecting two lipos together in series.

Anyways, I chopped off the bullet connector and put a couple of Dean's plugs onto the batteries.
Then I plugged the series cable with no issues, but when I plugged the balance leads to the 3S to 6S adapter it went up in sparks and now the balance lead on one of the batteries is burned.

<img src="/uploads/db1493/original/2X/4/4f4976bb3a2384e449190f50d7a867bde69829c1.jpg" width="666" height="500">

Here is what the adapter looks like:

<img src="/uploads/db1493/original/2X/e/ed4fa02ee675d443f555860a03e10318ea3d2e92.jpg" width="666" height="500">

Did I need to cut one of the wires on the adapter?

With all that said, is it still safe to use one or both batteries? Or do I have to get new ones?
```

---
## \#2 Posted by: b-rad Posted at: 2016-04-29T23:04:50.481Z Reads: 171

```
Maybe you should have put the balance leads in first, then put the batteries in series
```

---
## \#3 Posted by: lilracerboi Posted at: 2016-04-29T23:08:48.421Z Reads: 169

```
I thought about that after it happened, but I didn't think it made a difference.
```

---
## \#4 Posted by: b-rad Posted at: 2016-04-29T23:14:43.015Z Reads: 169

```
Yeah man i hate when stuff like this happens. I had that happen to me on a 6s lipo one time and i never used it again cause i dident feel comfortable charging it again... but im curious to know if this is fixable too...
```

---
## \#5 Posted by: lilracerboi Posted at: 2016-04-29T23:23:55.582Z Reads: 166

```
This will soon be the last time I deal with lipos.
I've decided to just save money and get the SPACE Cell.
Screw it, right? Safety first.
```

---
## \#6 Posted by: b-rad Posted at: 2016-04-30T01:53:50.392Z Reads: 161

```
Ehhhh... idk about coughing up $350 rather than max $150 for a lipo battery that will pretty much do the same thing. Just a little more hastle. No biggie.
```

---
## \#7 Posted by: b-rad Posted at: 2016-04-30T01:54:25.782Z Reads: 157

```
But if u got the money..... get the space cell... if your on a budget, stick to lipos
```

---
## \#8 Posted by: Chris_KP Posted at: 2016-04-30T02:08:34.654Z Reads: 152

```
that happend to me but on the deans connector first.

A fix for this issue is to decide which battery will be your positive and negative. 
then make sure that the outer red cable on the balance lead is on the positive side and the outer black cable on the other connector should be next to the black lead, then put a mark on each connector so you know where to connect it.
```

---
## \#9 Posted by: laurnts Posted at: 2016-04-30T02:15:43.478Z Reads: 146

```
Exactly like what @Chris_KP said. You need to decide which battery is postive side and the other one negative side.

The simplest solution would be to switch side your 6s balance plug connector. If its on left move it to right, if its on right move it to left (the 3s side). While doing this Do NOT change the side of your main connectors.

If you did it lucky and correct theres no short. If it does short, just do it like i said switch the side.

The easiet and safest way is to use multimeter.
```

---
## \#10 Posted by: Chris_KP Posted at: 2016-04-30T02:17:38.247Z Reads: 141

```
I was just passing on what you said hahahaha
```

---
## \#11 Posted by: laurnts Posted at: 2016-04-30T02:30:33.036Z Reads: 143

```
I know. It's kinda hard to explain it very short without diagram and or example, but I am happy you understand! :smiley:
```

---
## \#12 Posted by: lilracerboi Posted at: 2016-04-30T03:11:36.598Z Reads: 141

```
<img src="/uploads/db1493/original/2X/0/04d619caf07a38fa9c054a728a67da94c29ef724.jpg" width="666" height="500">

Here's how I had it connected before it sparked.

Should I have plugged the balance adapter before connecting the series connector?
The black sharpie mark on the balance adapter is indicating the pin that was sparking and is now burnt.
I plugged the non-burnt balance connector first and the burnt one was plugged second.
If someone could tell me why it happened, that would be great.

I already have a set of batteries setup, so these are my second set.
```

---
## \#13 Posted by: lilracerboi Posted at: 2016-04-30T03:15:42.886Z Reads: 135

```
I've already gone way over budget, so dishing out the money for the Space Cell is no problem.
I went in knowing this was going to happen. I figured this would be a continuous work-in-progress.

Even though I've been using lipos for awhile with somewhat good experience, it still gives me anxiety every time I'm handling them.
```

---
## \#14 Posted by: laurnts Posted at: 2016-04-30T03:16:25.519Z Reads: 135

```
It doesnt matter which connector you plugged in first, the balance or the series. Short is just short.

For now keep the main series connector plugged. We are just going to swap the balance lead around. Put the burned female to the unburned male. Then put the burned male to the unburned female.

You should have no spark at all if your batteries are not connected to ESC / VESC.
```

---
## \#15 Posted by: lilracerboi Posted at: 2016-04-30T03:23:47.107Z Reads: 131

```
Man, I'm so scared to plug it in, even if I'll be outside. Lol

I won't even be able to plug it into the burnt female because the pin melted down, so it's shorter and has a bulb too big for the male pinhole.

But, the batteries are good though, right?
```

---
## \#16 Posted by: laurnts Posted at: 2016-04-30T03:28:37.934Z Reads: 127

```
Yes. The batteries are fine. One of a few reason why connecting the series harness first is better is because if you short it out, the balance plug melt with spark but batteries are safe.

I know how scary it's and I am still paranoid as well time to time when working with lipo. Thats why most of the time when I am working with lipo / dismantling them, I always have my multimeter to double check and triple check before connecting the plugs if its going to short or not.

The way to fix those is actually by soldering them if you dont have spare balance head. But please be very careful if you cut those balance lead. You will have to cut 1 cable at a time, work with it and shrink wrap them immediately before doing the next one.
```

---
## \#17 Posted by: laurnts Posted at: 2016-04-30T03:29:21.103Z Reads: 121

```
I mean soldering the wires directly without using connectors.
```

---
## \#18 Posted by: lilracerboi Posted at: 2016-04-30T03:31:23.715Z Reads: 118

```
I won't go the solder route. Too afraid to do that.
I'll just order another adapter since they're cheap.

Are you advising me to solder the cables or is getting another adapter just fine?

Also with a multimeter, when using it, how can I tell if it's going to short or not?
```

---
## \#19 Posted by: laurnts Posted at: 2016-04-30T03:49:48.513Z Reads: 119

```
Well if you can get the same balance plug male and female is better, make sure to get couple of them as you might short it out again.

Soldering is also fine, but you got to make sure you're soldering it correctly according to the order I've just told you.
And if you're soldering, start with the negative one first (safer).

Just put multimeter on voltage reading. Then put 1 lead from multimeter to one female and put the other lead from multimeter to one male side. If theres a solid voltage reading from 3.6v up to 25.2v ish as ur using 6s, then if you connect them it will definitely spark up.
```

---
## \#20 Posted by: lilracerboi Posted at: 2016-05-04T20:16:34.781Z Reads: 102

```
I received the new balance adapter today.
I'm still afraid to plug it in, so what should I do?

Also, should I replace the burnt balance connector on the battery? (First picture above).
```

---
## \#21 Posted by: laurnts Posted at: 2016-05-04T20:21:50.271Z Reads: 95

```
Im going to be here online for some minutes, so you can always ask questions. First replace the old balance connector with the new one. After complete please post new photo while having your series harness attached. Also mark both of your new balance connector for the 3s side, one is A / red and the other one is B / blue.
```

---
## \#22 Posted by: lilracerboi Posted at: 2016-05-04T20:24:59.369Z Reads: 100

```
When you say replace the balance connector, are you talking about the plug on the battery itself, i.e solder a new one, or the adapter which plugs into both batteries?
```

---
## \#23 Posted by: laurnts Posted at: 2016-05-04T20:32:09.075Z Reads: 97

```
The plug from the battery that you burned down.
```

---
## \#24 Posted by: JTAG Posted at: 2016-05-04T20:59:32.901Z Reads: 99

```
Big: 

<img src="/uploads/db1493/original/2X/1/1145ab5d4c5cae334c1c1dad5b17fc72240df089.jpg" width="690" height="388">

Over the US right now :imp: .
```

---
## \#25 Posted by: lilracerboi Posted at: 2016-05-04T21:05:22.016Z Reads: 99

```
Lol Everything is all good now.
@JTAG helped me out with this issue.

Thanks for the support everyone.
```

---
## \#26 Posted by: lilracerboi Posted at: 2016-05-04T21:08:47.033Z Reads: 98

```
Actually, I have one more question regarding lipos.

When I go to plug the main Deans connector to the charger, it always makes a spark. I read sparks aren't an issue, but I'd rather not have them. I know where to go for the solution to the spark on the ESC, but can that solution apply to the charger as well?
```

---
## \#27 Posted by: jrpwit Posted at: 2016-05-12T03:43:19.406Z Reads: 92

```
Srry this question isnt directed at the person I am replying to but I couldnt figure how to create a new topic as I just created an account. 

Okay so here my question is: How do I wire a bms to multiple premade lipo batteries?

So recently I was planning on creating a 12s battery pack using 3s 5000mah batteries. 
Here is the batteries I am using http://www.hobbyking.com/hobbyking/store/uh_viewitem.asp?idproduct=8579&aff=1086883.
Additionally here is the bms which is compatable with lipo batteries.
http://www.batterysupports.com/44v-48v-504v-12s-30a-12x-36v-lithium-ion-lipolymer-battery-bms-p-268.html

I have already purchase all these items too but am confused as to how I will wire the balance wires connected to each battery. Currently I have been just using a 6s setup with a balance charger but want to upgrade to this new battery. I haven't seen any posts or videos similar to a battery that I am making because I am using premade batteries. Any help would greatly be appreciated. Thanks!!
```

---
## \#28 Posted by: jrpwit Posted at: 2016-05-12T03:43:51.016Z Reads: 90

```
Also if you guys would like to know this is the charger I am using.
http://www.batterysupports.com/432v-44v-504v-4a-lithium-ion-lipo-battery-charger-12s-12x-36v-p-167.html
```

---
## \#29 Posted by: willpark16 Posted at: 2016-05-12T03:52:14.777Z Reads: 90

```
why not go li ion if u were gonna buy a bms?
```

---
## \#30 Posted by: jrpwit Posted at: 2016-05-12T04:04:05.554Z Reads: 85

```
Already got the batteries and lipos are cheaper.
```

---
## \#31 Posted by: willpark16 Posted at: 2016-05-12T04:31:25.778Z Reads: 83

```
cheaper doesnt always mean better man
```

---
## \#32 Posted by: jrpwit Posted at: 2016-05-12T05:22:46.514Z Reads: 85

```
Sigh I know that but like I said I already bought them. I just need some help wiring them to the bms
```

---
## \#33 Posted by: willpark16 Posted at: 2016-05-12T06:37:09.985Z Reads: 85

```
ok ill help u tmrw its late here bro
```

---
## \#34 Posted by: b-rad Posted at: 2016-06-13T04:06:36.847Z Reads: 80

```
I am also interested in this because i plan on doing the same thing
```

---
## \#35 Posted by: mason Posted at: 2016-06-13T04:22:06.303Z Reads: 76

```
NO DON'T DO THIS IT WILL FRY EVERYTHING like what happened to me
```

---
## \#36 Posted by: seanpain4 Posted at: 2016-06-13T05:00:40.162Z Reads: 75

```
It will not fry everything if done correctly.
```

---
## \#37 Posted by: Hummie Posted at: 2016-06-13T05:06:31.969Z Reads: 74

```
This bms has a 30 amp limit.  So does the space cell.  Very lame. Really limits ur possible power.
```

---
## \#38 Posted by: Luke Posted at: 2016-06-13T06:19:51.098Z Reads: 76

```
@massy has gotten around this by bypassing the bms. I think this means that while the bms takes care of charging the vesc is in charge of discharging.. I need to ask him about how he did this too because I'm wanting to use one of the lower amp rating bms from battery support than the amps I wanna draw.
```

---
## \#39 Posted by: lowGuido Posted at: 2016-06-13T09:39:43.837Z Reads: 76

```
This topic has been covered plenty of times[quote="seanpain4, post:36, topic:2735, full:true"]
It will not fry everything if done correctly.
[/quote]

this = true

----------
```

---
## \#40 Posted by: Pablo_702 Posted at: 2016-06-29T20:47:13.975Z Reads: 68

```
@laurnts i man i just read this about the balance leads, and since im wiring up i wanted to triple make sure im doing it right i understood that in my 2 3s in series for a 6s i have to mark my negative lipo and make sure the black wire is on the outside when i plug them in and the red on the outside on my positive lipo, but i also read in this forum that theres people cutting 1 wire of the jst, if recall correctly the negative(black wire) of your negative side lipo, why is that they are cutting that wire and how this translate to balance charging them? compared to your method?
```

---
## \#41 Posted by: laurnts Posted at: 2016-07-01T21:52:23.323Z Reads: 63

```
If I am not mistaken what you mean by cutting one black wire is the black wire in the middle. You don't actually need them to be connected with anything. Even if you do want to connect it, you can connect it with the positive side which also sits in the middle of the balance lead (the last red wire of negative side of the battery).
```

---
