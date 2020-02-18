# Need help configuring focbox unity

### Replies: 16 Views: 260

## \#1 Posted by: thisguyhere Posted at: 2019-07-06T23:13:36.420Z Reads: 75

```
https://forum./t/need-help-configuring-focbox-unity/3870
```

---
## \#2 Posted by: LEE Posted at: 2019-07-07T11:32:41.721Z Reads: 58

```
In my case, it fails on the PC.
It has never been successful on a PC.
The Android App will succeed.
Try it on the Android App.
```

---
## \#3 Posted by: thisguyhere Posted at: 2019-07-08T15:43:49.101Z Reads: 46

```
so mine's dropping ble connection after like 30 seconds.

going to try another device, but so far my unity experience has kinda been shit.
```

---
## \#4 Posted by: Deodand Posted at: 2019-07-08T19:35:50.639Z Reads: 42

```
Highly recommend a pc for now if your phone is bugging. The app is built on qt at the moment  (non-native) and the BLE library it uses doesn't have the best compatibility with all phones it seems. We are working on native apps for iOS and android but limited resources means slower progress.
```

---
## \#5 Posted by: Deodand Posted at: 2019-07-08T19:38:52.971Z Reads: 41

```
Ok followed link, see you are having trouble with flux linkage. Can you let me know what your setup is? Belts? Motor kv? If its belts are you doing the hand spin with belts installed on the wheel, it works best that way. 

Are both flux linkages not detecting?
```

---
## \#6 Posted by: thisguyhere Posted at: 2019-07-08T19:41:48.001Z Reads: 40

```
thanks jeff for the input.

the thing is, connected to PC via usb doesn't work either, it fails when you go to spin the wheels for flux linkage detection.

o --- new post.

[quote="Deodand, post:5, topic:97972, full:true"]
Belts? Motor kv? 
[/quote]

yes belts, 6374 190kv motors.

[quote="Deodand, post:5, topic:97972, full:true"]
If its belts are you doing the hand spin with belts installed on the wheel, it works best that way.
[/quote]

tried both, with belts and spinning the wheel, and also wheels removed, spinning motors by hand.

[quote="Deodand, post:5, topic:97972, full:true"]
Are both flux linkages not detecting?
[/quote]

not sure if both are failing, but i can't get past the detection.

i think one motor is succeeding.

i'll keep giving it a go, i've got extra motors so i'll try it with those.
```

---
## \#7 Posted by: Deodand Posted at: 2019-07-08T19:45:36.392Z Reads: 36

```
Share back some screenshots of the full app if you can't get it to pass. Wanna have a look through the parameters it's reading back.

Sorry for the basic question but you are giving each wheel a nice strong hand spin?
```

---
## \#8 Posted by: thisguyhere Posted at: 2019-07-08T19:47:04.868Z Reads: 37

```
[quote="Deodand, post:7, topic:97972"]
Sorry for the basic question but you are giving each wheel a nice strong hand spin?
[/quote]

it's a legit question - i'm giving it everything i've got.

i'll continue messing with it tonight and post results.

thanks again jeff.
```

---
## \#9 Posted by: barajabali Posted at: 2019-07-08T19:47:49.787Z Reads: 36

```
I am just going to leave this here :  https://enertionboards.zendesk.com/hc/en-us/articles/360000774196-How-to-update-configure-the-Unity-for-DIY-Board-VIA-Android-OR-Windows-PC
```

---
## \#10 Posted by: Deodand Posted at: 2019-07-08T19:49:43.708Z Reads: 36

```
Yeah it shouldn't really take that much just a nice firm spin. Don't pull something trying to spin it harder :smile:  , check all the bullet solder joints as well. 

We'll get it sorted hopefully its a simple fix.
```

---
## \#11 Posted by: thisguyhere Posted at: 2019-07-08T19:51:32.369Z Reads: 34

```
i suspect it's a problem on my end, not the unity, sorry for mischaracterizing my problem.

maybe i will reflow the solder on all connections.

i've tried with hall sensors on and off, could that have an impact?
```

---
## \#12 Posted by: Deodand Posted at: 2019-07-08T19:59:28.686Z Reads: 34

```
No the halls won't effect that portion so don't worry about those for now.
```

---
## \#13 Posted by: thisguyhere Posted at: 2019-07-09T06:42:50.827Z Reads: 30

```
it's 100% user error.

i was spinning the motor by the shaft.  tried spinning the motor by grabbing the can and giving it some torque and it's reading flux no problems.

this is after trying on three different sets of motors, trying left and right for each, swapping phase wires, with and without hall sensors.  turns out i wasn't grabbing the motor right, so stupid.
```

---
## \#14 Posted by: Deodand Posted at: 2019-07-09T20:15:55.757Z Reads: 25

```
Sorry we should do a better job explaining with some tutorial videos.
```

---
## \#15 Posted by: thisguyhere Posted at: 2019-07-09T21:15:41.277Z Reads: 24

```
it's not you, it's entirely me lol :smile:

as always, thanks for the help!
```

---
## \#16 Posted by: thisguyhere Posted at: 2019-07-11T04:00:20.984Z Reads: 17

```
@Deodand 

just took it out for the first time, first time using a unity.

tested on 6" pnumatics and i just have to say, the brakes are SO NICE.

you've gone and completely fixed the braking problem for large diameter wheels on FOC.

good job jeff, you're gonna get rich doing whatever you're planning on doing.
```

---
