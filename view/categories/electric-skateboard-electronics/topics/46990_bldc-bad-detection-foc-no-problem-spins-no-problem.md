# BLDC Bad detection, FOC no problem. Spins no problem

### Replies: 37 Views: 1614

## \#1 Posted by: Apolo Posted at: 2018-02-21T00:44:12.927Z Reads: 139

```
Using ackmaniacs updated esc tool with his firmware (also tried with default 4.10 that comes with it).

Can move the motor very smooth with arrow keys but when I detect it in bldc, it spins up nicely and normally and slows down, then starts to jitter. 

FocBox single drive 

190Kv TB 6355 sensored
TB 12s2p li ion
36V start cut off
33V end cut off

Motor max 60A
Motor min -55A

Bat max 35A
Bat min (regen) -15A

No load is on the motor and phase wires are properly isolated.
For obvious reasons, I want to stick with bldc on 12s

*I know I'm going to get people telling me to use the search bar, but after almost 2hrs of reading I still got nothing.

CONCLUSION: For those who have the same problem; it's just the vesc tool being buggy. Downgrade to 2.54 or similar and use the old BLDC tool
```

---
## \#2 Posted by: GrecoMan Posted at: 2018-02-21T00:45:33.453Z Reads: 131

```
use the search bar. lol kidding.

no faults?
tried loosening motor from motor mount?
nothing shorted (not just phase wires)?

actually, try unplugging the sensor. see if that works, if it does, take pics of the sensor wire and the order on the focbox

oh yea, and of course, is the sensor plugged into the correct port?
```

---
## \#3 Posted by: ShutterShock Posted at: 2018-02-21T00:53:04.764Z Reads: 120

```
I have this same exact issue, using VESC Tool.  No idea why.  I have been using sensored FOC on 12S because I couldn't figure out why the BLDC motor detection didn't work.  

Only had a problem when moving to FOCBOX's, with my TB vescs, bldc sensored worked fine.

The only annoying thing about FOC is the stupid hard braking at slow speeds <1mph
```

---
## \#4 Posted by: GrecoMan Posted at: 2018-02-21T00:57:10.763Z Reads: 119

```
can I get a pic of where the sensor wire is plugged in?

also, when did you buy the focboxes?
```

---
## \#5 Posted by: Apolo Posted at: 2018-02-21T00:58:37.410Z Reads: 117

```
Cyber Monday, they came in today. Will get pictures when I'm back home
```

---
## \#6 Posted by: ShutterShock Posted at: 2018-02-21T00:58:41.005Z Reads: 114

```
They were part of the black Friday batch, I received them in December.

It would be very hard to plug the sensor wire into the incorrect port imo.  Also the sensored FOC works great, and all hall sensors are detected.
```

---
## \#7 Posted by: Apolo Posted at: 2018-02-21T01:01:58.314Z Reads: 110

```
Just scared to shit running foc on 12s. I've been through the drv trauma
```

---
## \#8 Posted by: GrecoMan Posted at: 2018-02-21T01:03:32.644Z Reads: 106

```
yea kinda forgot this was the focbox ;)

super easy to confuse the ports on the TB vesc
```

---
## \#9 Posted by: GrecoMan Posted at: 2018-02-21T01:04:35.120Z Reads: 102

```
so lemme get this straight, all sensors and everything detect in FOC, just not BLDC? @ShutterShock
```

---
## \#10 Posted by: Apolo Posted at: 2018-02-21T01:05:04.691Z Reads: 101

```
Precisely. I feel like this is a software problem
```

---
## \#11 Posted by: GrecoMan Posted at: 2018-02-21T01:05:40.831Z Reads: 99

```
the reason i will never stop using 2.18 or 2.54.
```

---
## \#12 Posted by: Apolo Posted at: 2018-02-21T01:06:32.524Z Reads: 100

```
How do I downgrade to 2.54? Can't find the firmware
```

---
## \#13 Posted by: louwii Posted at: 2018-02-21T01:06:45.588Z Reads: 100

```
The sensor detection fails when the motor spins in the wrong direction. At least that's what happened to me, in BLDC only, FOC was working fine.
I just had to swtich 2 phase wires and it went fine.
```

---
## \#14 Posted by: Apolo Posted at: 2018-02-21T01:07:14.773Z Reads: 99

```
[quote="louwii, post:13, topic:46990"]
had to swtich 2 phase wires
[/quote]
Tried that too
```

---
## \#15 Posted by: b264 Posted at: 2018-02-21T01:11:19.402Z Reads: 102

```
[quote="Apolo, post:1, topic:46990"]
Bat min (regen) 15A
[/quote]

This needs to be a negative number.
```

---
## \#16 Posted by: DanSkates Posted at: 2018-02-21T01:11:24.844Z Reads: 98

```
I've had this exact issue.  Since upgrading the firmware on my FOCBOXs with the ackmaniac tool - they both detected in BLDC in the VESC tool but then one of the 2 wouldn't in the new tool.  I never managed to find out why unfortuntely however I've been running them in FOC (unsensored 168kv SK3s) on 12s for a few months now and had no issues at all.  Much smoother start up too.
```

---
## \#17 Posted by: Apolo Posted at: 2018-02-21T01:11:52.048Z Reads: 101

```
Yes it is a negative, just made a typo here
```

---
## \#18 Posted by: b264 Posted at: 2018-02-21T01:12:15.580Z Reads: 99

```
Typos can destroy expensive hardware; please be careful!
```

---
## \#19 Posted by: Apolo Posted at: 2018-02-21T01:12:42.811Z Reads: 97

```
Typo on the post, not the vesc tool lol. I triple check everything there
```

---
## \#20 Posted by: ShutterShock Posted at: 2018-02-21T01:36:50.175Z Reads: 96

```
yep exactly, I have no idea why.  It won't even get through the motor detection in BLDC, it fails every time.
```

---
## \#21 Posted by: ShutterShock Posted at: 2018-02-21T01:37:47.646Z Reads: 94

```
Maybe I will try this.  I used the same config as on my TB VESC's so I figured it would be fine, especially since it works in FOC, but this isn't really a hard thing to check either.
```

---
## \#22 Posted by: Brianr058 Posted at: 2018-02-21T03:31:30.143Z Reads: 90

```
the low duty is at 0.05 bump it up to 0.10
```

---
## \#23 Posted by: ThermalM16 Posted at: 2018-02-21T03:36:30.993Z Reads: 91

```
I can fix it! :wink:
```

---
## \#24 Posted by: Brianr058 Posted at: 2018-02-21T03:43:03.306Z Reads: 97

```
![Screenshot_20180220-194204|690x500](upload://5PLpqInUZ47ZVrTZ9i5DxZ5IfLf.jpg)
```

---
## \#25 Posted by: Brianr058 Posted at: 2018-02-21T03:44:49.287Z Reads: 102

```
Open the picture
```

---
## \#26 Posted by: ThermalM16 Posted at: 2018-02-21T03:48:01.875Z Reads: 103

```
Here are the firmwares 
https://theboardtech.com/wp-content/uploads/TheBoardTech_VESC_FW.zip

And here's how you do it
![Downgrade|690x382](upload://253mK2WLFK9RT04WGoEWLeK6F8M.gif)
```

---
## \#27 Posted by: Apolo Posted at: 2018-02-21T03:51:32.087Z Reads: 99

```
I downgraded to ackmaniac 2.54, now using his modified BLDC tool instead of the newer ESC tool. 

Thanks anyway!
```

---
## \#28 Posted by: GrecoMan Posted at: 2018-02-21T14:27:19.709Z Reads: 88

```
and you got it to detect?
```

---
## \#29 Posted by: Achmed20 Posted at: 2018-02-21T14:59:06.091Z Reads: 86

```
have the same problem with the curretn VESC tool. its jsut completly random. sometimes its my left motor, sometimes the right one and FOC works all the time ... . that used to be the other way arround ^^
```

---
## \#30 Posted by: Apolo Posted at: 2018-02-21T15:11:23.850Z Reads: 87

```
Yep. Literally zero problems with ackmaniac bldc tool 2.54
```

---
## \#31 Posted by: Apolo Posted at: 2018-02-21T15:14:23.459Z Reads: 84

```
Got everything working with 2.54. I guess the vesc tool is just bugged. 

One problem solved, another arises.
My Nano X I've been waiting 3 months for doesn't work. Mailed it to @barajabali per enrtion support's request. Hopefully I'll get my replacement soon.
```

---
## \#32 Posted by: SORRENTINO Posted at: 2018-02-21T15:19:30.107Z Reads: 83

```
So I had the same issue with the Vesc tool. Ill I had to do was turn up D to .1 or .12 like @Brianr058 mentioned.
```

---
## \#33 Posted by: TarzanHBK Posted at: 2018-02-21T15:30:40.371Z Reads: 82

```
@Ackmaniac do you know whats wrong with the vesc tool here?
```

---
## \#34 Posted by: Apolo Posted at: 2018-02-21T15:43:59.634Z Reads: 78

```
Also, is there a 3.xx version of your firmware incase the esc tool decides to work?
```

---
## \#35 Posted by: Luuke Posted at: 2018-02-21T17:32:47.032Z Reads: 70

```
Same here!!
```

---
## \#36 Posted by: Apolo Posted at: 2018-02-21T17:52:31.240Z Reads: 70

```
Guys I just tried BLDC detection again with the vesc tool today and it worked. I changed nothing lol.
```

---
## \#37 Posted by: Riako Posted at: 2018-02-22T14:25:10.697Z Reads: 64

```
hahah ... whaaat ?!
Ho guys ! Thanks for this theard,.. I feel less lost :sweat_smile:
I have just post this few day ago :

> http://www.electric-skateboard.builders/t/vesc-boot-loader-installation-tutorial/32103/7

Cause I need to use my fox with VESC TOOL, when I flash my Fox with stlink and last hex files from Benjamin, it upgrade fw to 3.34. Is that the one you test @Apolo ? 

And just to see clear about of it, witch fw and tool is the "best/trusty" to use with a Fox actualy ? ?
```

---
