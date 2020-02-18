# I need brushed inrunner speed controller for 100volts

### Replies: 29 Views: 2005

## \#1 Posted by: longhairedboy Posted at: 2017-05-09T14:54:35.370Z Reads: 207

```
anyone know where i can get a brushed D.C. controller that can handle 100volts? This monster truck board showed up at my shop and dude gave me a wad of cash to try and get it running reliably at ~ 96v or so. 

<img src="/uploads/db1493/original/3X/2/6/26b7182268d1c7e51872a52d66be43c2f8643cc8.JPG" width="666" height="500">
```

---
## \#2 Posted by: barajabali Posted at: 2017-05-09T14:56:14.802Z Reads: 203

```
I have no idea but I support this cause ! Haha
```

---
## \#3 Posted by: longhairedboy Posted at: 2017-05-09T14:59:38.982Z Reads: 201

```
these are the old Hyper Vipers. He had a few of them. In the background you can see one he jacked up on HUUUUGE wheels from a golf cart or something and they have motorcycle ties on them. 

Anyway they've got four giant DC brushed inrunners and i need a 100v controller that can take some PWM input so we can use standard remotes.

typically they run at 10S and 13S and he wants one to run at basically what amounts to 26S which is approximately 93 volts.
```

---
## \#4 Posted by: Blasto Posted at: 2017-05-09T15:39:56.406Z Reads: 191

```
"Hold my beer while i stick 100V on this skateboard"

A treadmill motor controller? Would require some hacking to remove the AC rectifiers and an arduino to interpret the remote signal to send to the motor controller... doable, but won't be pretty

Love to see the magic smoke come out of those motors
```

---
## \#5 Posted by: longhairedboy Posted at: 2017-05-09T15:44:10.903Z Reads: 186

```
its going to be interesting. He has plenty of them to smoke, too. 

He's got several of these boards and he's been running them at 72volts. They're designed for 36 and 48, but he strapped a couple  of the packs together in series and they last for a while but start blowing caps in the ESC.  

I told him there had to be something out there, possibly something for ebikes maybe.
```

---
## \#6 Posted by: Jinra Posted at: 2017-05-09T16:17:49.067Z Reads: 173

```
If he only blew caps on the ESC why not slap some higher voltage caps on them and see if they run?
```

---
## \#7 Posted by: longhairedboy Posted at: 2017-05-09T16:19:03.058Z Reads: 169

```
yeah we're trying that first. Then we'll see what else blows after that. Its like playing dominoes except when they fall you put bigger dominoes. 

Eventually we'll get all the way to the traces and when we cook them its done.
```

---
## \#8 Posted by: B4Me Posted at: 2017-05-09T16:26:47.565Z Reads: 166

```
ebikes uses something 42v :(
```

---
## \#9 Posted by: saul Posted at: 2017-05-10T00:10:31.052Z Reads: 154

```
I've seen them but not sure about quality.
I wouldnt want to run voltage that high. Even >40v can be deadly, 96v is all kinds of trouble with the amps you'd need.

Should be something tho
```

---
## \#10 Posted by: Jinra Posted at: 2017-05-10T00:47:23.115Z Reads: 147

```
Yea.. considering North American wall outlets are 120v and just a couple amps could kill you.
```

---
## \#11 Posted by: longhairedboy Posted at: 2017-05-10T11:42:59.032Z Reads: 137

```
it only takes 100-200 milliamps to stop your heart. Everything over that is a light show for the death concert. 

its all about the application. Ever grab some bare wires in your wall with one hand by accident while doing some work on the house? You felt it. It feels like somebody turned your hand into steel and placed it in an ultrasonic paint shaker clamp. Are you dead? no. 

But don't grab one wire in each hand.  You'll probably die.
```

---
## \#12 Posted by: saul Posted at: 2017-05-10T19:02:29.959Z Reads: 122

```
yea but that 120AC,
DC is another game at that kind of voltage.

how many amps did the original controllers put out? I think you could get the performance without overvolting to death. lol
those motors will have a limit somewhere...
```

---
## \#13 Posted by: fedestanco Posted at: 2017-05-10T21:10:55.679Z Reads: 119

```
https://m.nl.aliexpress.com/item/32620526387.html#autostay maybe...
```

---
## \#14 Posted by: Jinra Posted at: 2017-05-10T21:11:54.300Z Reads: 119

```
10 amps is not nearly enough
```

---
## \#15 Posted by: fedestanco Posted at: 2017-05-10T21:14:09.549Z Reads: 115

```
Perhaps if he's got 4 motors he could output 4*10*100=4000w dc.
```

---
## \#16 Posted by: longhairedboy Posted at: 2017-05-11T11:15:16.287Z Reads: 111

```
it has four motors. I forgot to mention that. But all four motors are controlled by a single two conductor output, so they're all in parrallel. I guess that's something you can do with DC brushed inrunners.
```

---
## \#17 Posted by: PXSS Posted at: 2017-05-11T15:09:24.022Z Reads: 100

```
110AC is relatively safe because it goes through 0v 120 times a second (60hz) therefore your muscles dont cramp up and you're able to let go. The average dry skin thumb-finger grasp skin resistance is 20kohm, average resistance per arm is 250ohm. The total resistance from holding a live wire while touching a grounded sourface with your other hand would be 20500 ohm. The current flowing through your body would be 5.36mA which means you'll feel the shock. You would need to hold this wire for a total of 21 seconds in order to cause defribrilation.
```

---
## \#18 Posted by: L3chef Posted at: 2017-05-11T15:31:25.312Z Reads: 96

```
Checked ASP? Think they have one for 24s or something like that
```

---
## \#19 Posted by: longhairedboy Posted at: 2017-05-11T18:39:57.666Z Reads: 90

```
ASP? what's that?
```

---
## \#20 Posted by: Norco Posted at: 2017-05-11T18:56:47.623Z Reads: 89

```
How about these guys. Up to 300amp though u hate to think how big it will be... 

http://www.4qd.co.uk
```

---
## \#21 Posted by: longhairedboy Posted at: 2017-05-11T19:09:59.940Z Reads: 86

```
thanks. I'm going to contact them and send them pics of what i have and see if they have anything similar.
```

---
## \#22 Posted by: smurf Posted at: 2017-05-11T19:21:01.222Z Reads: 84

```
http://kellycontroller.com/kdz7220124v-72v200apm-with-regen-p-960.html?osCsid=p9v2fa1urhtsukh59a51pr8rc1
```

---
## \#23 Posted by: FredSaberhagen Posted at: 2017-05-11T19:21:03.573Z Reads: 81

```
They may be run in parallel but... they don't _have_ to be.  You're just dumping in dc so buy several smaller esc (10a should work fine) - parallel the control signals sure, but give each motor it's own small esc.  Boom ur done
```

---
## \#24 Posted by: longhairedboy Posted at: 2017-05-11T19:34:50.811Z Reads: 84

```
That's a good idea too. IF this doesn't work, that might have to. At the moment we're hoping to find something that can be a mostly drop in replacement for the ones in there. 

I'll post a pic of the ones in there now later and see if it rings any bells with anyone. Then maybe a clue to finding a higher powered one like it will present itself.
```

---
## \#25 Posted by: L3chef Posted at: 2017-05-12T04:14:57.489Z Reads: 76

```
Alienpowersystem
http://alienpowersystem.com/shop/esc/alien-450a-4-24s-sport2-72-mosfet-esc-hv-sensored/
```

---
## \#26 Posted by: longhairedboy Posted at: 2017-05-12T12:04:53.587Z Reads: 72

```
Thats a good option if we end up going brushless because of lack of options. I'm still trying to find one for larger brushed DC inrunner motors though.
```

---
## \#27 Posted by: HyperViper Posted at: 2018-03-11T04:06:16.133Z Reads: 46

```
you can see twice that at 220v on instagram. my name is 4x4boards  Jake the man hoooked it up with twin 220. four 48v batteries.
```

---
## \#28 Posted by: HyperViper Posted at: 2018-03-11T04:07:26.582Z Reads: 45

```
thats pretty much it.  used two esc's in parallel, each handling 2 motors and 110v    4x4 style  my insta is 4x4boards
```

---
## \#29 Posted by: HyperViper Posted at: 2018-03-11T04:08:26.934Z Reads: 46

```
i think it's like 20 thousand now :slight_smile:
```

---
