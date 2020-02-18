# Board on full throttle after 2mm \[HELP\]

### Replies: 37 Views: 352

## \#1 Posted by: xsynatic Posted at: 2019-03-10T13:16:02.704Z Reads: 105

```
Hello there,

I currenty build my first DIY board but i have yet again some issues. I'm not sure how to extend the throttle curve. Currently the Motor spinns at full speed after about 2-3mm of movement. Thats 1/3 of the thumbwheel. How to i extend the curve so full throttle is only when the wheel is at the end? (Same basically for the brakes)

Vesc 4.12

TB 6374

12S2P

What infos do you need if any?
```

---
## \#2 Posted by: Andy87 Posted at: 2019-03-10T13:20:23.625Z Reads: 100

```
Did you adjust your pulswith according to your remote?
I mean did you go through the ppm wizard?
```

---
## \#3 Posted by: Jarno Posted at: 2019-03-10T13:22:19.179Z Reads: 97

```
Can you show screenshots of the PPM mapping and PPM Throttle curve?
```

---
## \#4 Posted by: xsynatic Posted at: 2019-03-10T13:39:49.662Z Reads: 91

```
yes. Brake is 100. Full throttle is 100 and nothing ~0. by ppm wizard you mean "Setup Input"?

@Jarno Here you go.

EDIT : I played a bit with the throttle curve but from hearing it, it didn't change anything major.

![h|690x388](upload://d7uuFfEBRSuXuecfhTYT7gOrN71.png) ![hh|690x184](upload://b3bagy0kSVOh55ugDKwiYNmB507.png) ![hhh|690x185](upload://8JBxmwJfLF5iOA4yRVTtItMj7VH.png)
```

---
## \#5 Posted by: Andy87 Posted at: 2019-03-10T13:45:57.189Z Reads: 84

```
Exactly this.
Which remote you use?
Do you have different speed modes, and if yes in which you made the confirmation?
```

---
## \#6 Posted by: Jarno Posted at: 2019-03-10T13:46:38.603Z Reads: 81

```
I'm guessing you are not standing on you board while trottling? I think it may be that once your motor starts running without a real load it can go to max ERPM with a small current i.e. not max trottle. Can you try to do a duty sweep (Experimental tab) and see what happens?
```

---
## \#7 Posted by: xsynatic Posted at: 2019-03-10T13:49:09.415Z Reads: 79

```
I use the 2.4ghz Nano remote. I don't have different speed mode, but i want them if possible. A seperate reverse function would be cool too. (Not the Boosted board style)
```

---
## \#8 Posted by: Jarno Posted at: 2019-03-10T13:49:44.581Z Reads: 80

```
[quote="xsynatic, post:1, topic:86763"]
How to i extend the curve so full throttle is only when the wheel is at the end?
[/quote]

To do this make the trottle curve this:
![image|690x379](upload://nKghIwUcdXsR4EuB8BW3vxlXnii.png)
```

---
## \#9 Posted by: xsynatic Posted at: 2019-03-10T13:51:51.604Z Reads: 76

```
correct. It was an empty load while testing it out.

duty sweep just "clicks" as if the Motor is unsensored and doesn't know which way to go.
```

---
## \#10 Posted by: Jarno Posted at: 2019-03-10T13:59:29.523Z Reads: 73

```
Can you try the other tests?
```

---
## \#11 Posted by: Narnash Posted at: 2019-03-10T14:00:19.071Z Reads: 72

```
Do you test the speed on a "bench" setup or while riding the board?

With a VESC you typicly control power (current) and not the speed, like a real car.

So you may reach the max speed of your setup with half throttle/power, but on full throttle your acceleration is faster.

But as some already mentioned, you can also modify the power gain per % on the remote by software.
```

---
## \#12 Posted by: xsynatic Posted at: 2019-03-10T14:01:15.288Z Reads: 63

```
all 3 do the same
```

---
## \#13 Posted by: xsynatic Posted at: 2019-03-10T14:02:47.654Z Reads: 64

```
My only way to test it is to unplug it and take it outside (not now because it starts raining) Or inside my room where i can move 1 1/2 Meters.
```

---
## \#14 Posted by: Friskies Posted at: 2019-03-10T14:11:45.593Z Reads: 61

```
What everyone is trying to say is that if there is nobody standing on the board when you push the throttle (the wheels are not on the ground), it will always go full speed no matter your position on the throttle.
```

---
## \#15 Posted by: Andy87 Posted at: 2019-03-10T14:12:06.023Z Reads: 63

```
So it’s not this one?
![image|327x500](upload://gWLmHR4mNdVVKLlptezBwmDQlr3.jpeg) 

Reverse is no problem, just change your drive mode in the vesc settings to current reverse with breaks. Don’t nail me on the exact naming.
```

---
## \#16 Posted by: xsynatic Posted at: 2019-03-10T14:15:33.992Z Reads: 59

```
Yes, thats the one.

I only can use reverse modes with the boosted style of reverse (Which i don't like) or no reverse at all.

![hhhh|690x356](upload://7AB9plxqVVdlv8aU73iggOgeCo0.png) ![hhhhh|634x497](upload://ueVgKJWliZbGgCklreA8T7DCeKi.png)
```

---
## \#17 Posted by: xsynatic Posted at: 2019-03-10T14:17:13.233Z Reads: 54

```
So i have to adjust the throttle curve and stand on the board the maybe see a difference.

How about Reverse and Speed modes? The remote itself has a seperate reverse button and a speed mode switch mode i don't know if i can program these.
```

---
## \#18 Posted by: Andy87 Posted at: 2019-03-10T14:21:10.120Z Reads: 53

```
[quote="xsynatic, post:16, topic:86763"]
boosted style of reverse
[/quote]

What you mean with it? 
You want to go reverse only after switching the button?

[quote="xsynatic, post:17, topic:86763"]
speed mode switch
[/quote]

Now you have speed modes? 🤔😂
Make sure you did the mapping in the fast mode.
```

---
## \#19 Posted by: xsynatic Posted at: 2019-03-10T14:25:15.092Z Reads: 53

```
yes, i only want throttle and brake on the thumbwheel. Activating Reverse via the button.

The remote has a switch for speed modes. It doesn't make any difference between those 2.

@Andy87
```

---
## \#20 Posted by: Jarno Posted at: 2019-03-10T14:26:52.147Z Reads: 51

```
Did you do the setup in fast mode? This needs to be done!
```

---
## \#21 Posted by: xsynatic Posted at: 2019-03-10T14:27:36.023Z Reads: 49

```
Not sure. I can redo it.
```

---
## \#22 Posted by: Jarno Posted at: 2019-03-10T14:27:45.952Z Reads: 50

```
Please do.
```

---
## \#23 Posted by: xsynatic Posted at: 2019-03-10T14:28:25.001Z Reads: 49

```
what would be the problem if i've done it on the other one?
```

---
## \#24 Posted by: Jarno Posted at: 2019-03-10T14:30:36.963Z Reads: 48

```
Speed mode on the controller works as follows:

In fast mode the ranges of you controller are big.

In slow mode the range is limited.

If you setup in slow mode and switch to fast mode you get to your max at say 50% of full trottle.
```

---
## \#25 Posted by: xsynatic Posted at: 2019-03-10T14:33:34.824Z Reads: 45

```
So doing the setup with the fast mode automatically limits the "slow" mode to 50%?
```

---
## \#26 Posted by: Friskies Posted at: 2019-03-10T14:34:27.009Z Reads: 45

```
You need to stand on the board and it will be fine as long as you do the following:

- Program the controller via the PPM wizard
- Turn the remote on before the board and the push to full throttle and then full brake then turn the board on.


The stock throttle curve should be fine and make sure you run the wizard with the board in fast mode. The slow mode switch will limit throttle to 70% for both Acceleration and Brake.
```

---
## \#27 Posted by: Jarno Posted at: 2019-03-10T14:34:31.305Z Reads: 44

```
It will limit the slow mode to something.
```

---
## \#28 Posted by: xsynatic Posted at: 2019-03-10T14:40:26.902Z Reads: 42

```
Now i got it. Thanks. Any idea about the Reverse problem? The nano remote has a seperate reverse button which i want to use but don't know how to enable.
```

---
## \#29 Posted by: Friskies Posted at: 2019-03-10T14:42:51.717Z Reads: 40

```
It can be done but you need Acks firmware and to pug in a PPM channel to another remote. Honestly I don't recommend using reverse to begin with. You may one day hit it whilst at 50kmh and not have a good time or even just from the standstill and have a bad time.
```

---
## \#30 Posted by: xsynatic Posted at: 2019-03-10T14:46:40.303Z Reads: 39

```
Thats why i like the hobbywing ESC where if you are faster than 3km/h nothing happens.

But ok, reverse is not a must but would be cool. But I'll lay it on ice for now. Thanks for the help!
```

---
## \#31 Posted by: Andy87 Posted at: 2019-03-10T15:16:54.948Z Reads: 37

```
It’s similar with vesc. Faster than 3km/h round about and your wheels will not spin backwards, even if you hit full negative throttle.
```

---
## \#32 Posted by: Dirt_Bag Posted at: 2019-03-10T19:48:41.521Z Reads: 27

```
make sure your board has some sort of load. some vescs spin up to max rpm if the wheels are not on the ground and experiencing some sort of resistance
```

---
## \#33 Posted by: xsynatic Posted at: 2019-03-12T12:22:12.265Z Reads: 24

```
@Jarno @Friskies I got it to work and it feels pretty good. But guess what. The Magnet retaining Ring came loose. So, no riding for me for a while.
```

---
## \#34 Posted by: Andy87 Posted at: 2019-03-12T12:28:39.877Z Reads: 25

```
what was the issue? how did you fix it?

about the retaining ring, just battle harden the bell.
better than directly from both.

https://www.electric-skateboard.builders/t/ice-crusher-16ply-holypro-4w-chain-drive-mtb-4x-6374-170kv-aps-quad-escape-steering-damper/65823/119?u=andy87
```

---
## \#35 Posted by: xsynatic Posted at: 2019-03-12T12:34:30.139Z Reads: 26

```
The issue was the non adjusted throttle curve and that i tested it with no load. I still reach full throttle before the end but its much nicer now. I've contacted support already. Not sure if i have that much trust in my skills to do it. Would be pretty nice though.
```

---
## \#36 Posted by: Andy87 Posted at: 2019-03-12T12:39:37.544Z Reads: 26

```
Oh i just see it was a tb motor, if it was a new one thsn i‘m sure they will work something out for you.
```

---
## \#37 Posted by: xsynatic Posted at: 2019-03-12T12:54:48.270Z Reads: 23

```
I've had it for 1 1/2 Months now but used it the first time 4 days ago.
```

---
