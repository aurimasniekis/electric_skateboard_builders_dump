# Throttle is reversed

### Replies: 29 Views: 1539

## \#1 Posted by: craj1031tx Posted at: 2017-12-25T05:35:02.919Z Reads: 173

```
Hey guys, first post after doing quite a bit or lurking. Building out my board using a Vedder 4.10 VESC from Hobby King (Turnigy) and a remote/receiver I got off of Banggood: [pics here](https://www.banggood.com/2_4GHz-Radio-Remote-Controller-Receiver-Transmitter-For-Electric-Skateboard-p-1125575.html?rmmds=search&cur_warehouse=CN)

My issue is that the throttle appears to be reversed, and I can't find a software setting to remap it. I saw some other posts about there being a switch on some remotes; mine does not appear to have a throttle reverse hardware switch on it. 

In app configuration, I have it set to PPM and think I have the PWM tuned in nicely, but it's just flipped. When the trigger is in its middle rest position, it reads at being at 50 percent (got there by using the throttle trim wheel on the remote itself), and then when I pull the trigger in I can get it to 0pct; pushing it out gets me to 100 pct. 

However, the motor engages when the trigger is pushed away from your body, outwards, and the brake appears to engage by pulling the trigger in towards you. I would like to have this flipped if possible - does anyone know of a way? 

Thanks!
```

---
## \#2 Posted by: Exiledd_Top Posted at: 2017-12-25T06:00:49.843Z Reads: 160

```
I don't remember but motor rotation rotate it , mine is "reversed"  from normal but am using esc but I think the vesc there is a setting for motor rotation aswell in the settings if you can't rotate the remote rotation.
```

---
## \#3 Posted by: Idle Posted at: 2017-12-25T06:05:20.041Z Reads: 160

```
Yeah it's the phase wires need to be switched. 
Pick two wires and swap them. 
Do the two that would benefit routing wise..

Wow I remembers something.
```

---
## \#4 Posted by: scepterr Posted at: 2017-12-25T06:09:23.361Z Reads: 152

```
Lol @Exiledd_Top @Idle
Two swings, two misses 😋

The throttle on his remote is backwards, not motor rotation

Unfortunately I don't know how to correct that, try different channel?
```

---
## \#5 Posted by: Namasaki Posted at: 2017-12-25T06:10:27.578Z Reads: 137

```
[quote="scepterr, post:4, topic:41862"]
The throttle on his remote is backwards, not motor rotation
[/quote]

 Ladies and Gentlemen we have a winner!!!!!!

@scepterr  Any Idea what causes this, I am still scratching my head over this.
```

---
## \#6 Posted by: E1Allen Posted at: 2017-12-25T06:11:16.454Z Reads: 131

```
[quote="Idle, post:3, topic:41862"]
Yeah it's the phase wires need to be switched. 
Pick two wires and swap them. 
Do the two that would benefit routing wise..
[/quote]

He means pick two of the three wires that go from the ESC to the motor and switch them. Your motor will spin the opposite direction. Just trying to help if you weren't sure which were the phase wires.
```

---
## \#7 Posted by: Namasaki Posted at: 2017-12-25T06:11:56.512Z Reads: 125

```
As @scepterr said, motor rotation is not the problem,
The remote is signaling backwards.
Motor spins when trigger is pushed forward and brakes apply when trigger is pulled back
```

---
## \#8 Posted by: scepterr Posted at: 2017-12-25T06:13:51.619Z Reads: 123

```
The only way I can think to "fix" it is swap the wires on the throttle

@craj1031tx did you try to rebind the remote?
```

---
## \#9 Posted by: Namasaki Posted at: 2017-12-25T06:14:54.585Z Reads: 124

```
You think it could be a factory defect?
```

---
## \#10 Posted by: Namasaki Posted at: 2017-12-25T06:15:30.496Z Reads: 120

```
what position do you have the white knob at? It should be around 2:00
```

---
## \#11 Posted by: pat.speed Posted at: 2017-12-25T06:16:11.677Z Reads: 118

```
What is happening is when he pushes the trigger outwards (to where full brake normally is) the motor spins and when he pulls it inwards (to where full throttle should be) it brakes. @craj1031tx you have setup your remote throttle range right? You could also try what @scepterr said and swap the pots wires around
```

---
## \#12 Posted by: Mikenopolis Posted at: 2017-12-25T06:22:53.376Z Reads: 114

```
If using VESC use the Ackmaniac Firmware  you can switch direction with that program
```

---
## \#13 Posted by: Idle Posted at: 2017-12-25T06:22:53.913Z Reads: 112

```
Well 💩
Maybe I try reading a bit slower🤓
```

---
## \#14 Posted by: craj1031tx Posted at: 2017-12-25T06:30:50.525Z Reads: 113

```
Hey all, yes, the issue isn't with the motor spinning the wrong way, which can easily be switched by swapping two of the VESC output leads. I almost do think that it could be some sort of factory defect/error. Would be easily solved with a reverse switch, but of course this cheap remote doesn't have one... again, just to reiterate: the issue is that the motor is engaged when the throttle position is 'out' from your body, which is just an uncomfortable way to control it. 

And no, I have not yet tried re-binding the remote. That does seem like something I should try though.

Throttle trim is at 11 oclock. I started at 2 oclock as per videos I saw online, but during tuning in BLDC Tool it was necessary to move it to 11 to get a neutral throttle position to read as 50 pct in the tool.


I'm guessing switching two of the 3 leads coming from the receiver to the esc would be a bad idea, right? Keeping ground where it is and swapping the other two? Since it's PWM I guess it won't make a difference. 

Any other input is appreciated!
```

---
## \#15 Posted by: Namasaki Posted at: 2017-12-25T06:33:48.778Z Reads: 107

```
[quote="craj1031tx, post:14, topic:41862"]
I'm guessing switching two of the 3 leads coming from the receiver to the esc would be a bad idea
[/quote]


Yes bad idea because the middle wire is the signal wire. The other wires are 5v+ and ground.

The trim knob should be at 2:00 not 11:00.
When you calibrate to the vesc, you dont use the trim knob to get neutral in the center.
You simply get the full positive and negative reading and apply them and the neutral should automatically move to center when you write configuration.

Here is a good video showing the proper way to do it:
https://youtu.be/OtuofrQr3F8
```

---
## \#16 Posted by: craj1031tx Posted at: 2017-12-25T06:38:30.627Z Reads: 97

```
Pat, I tried originally following these steps when pairing my remote control:

https://www.youtube.com/watch?v=OOplk52R4no&t=257s

but from what I've read, these procedures are unnecessary when working with VESCs - is that right? Does that throttle range need to be calibrated? I thought using the pwm settings inside of the BLDC tool essentially took care of this.
```

---
## \#17 Posted by: craj1031tx Posted at: 2017-12-25T06:42:02.667Z Reads: 93

```
So when I moved minimum pulsewidth to 1.15 (which seemed to be the correct value to get a 0 pct reading when bottoming out my throttle [pulled towards me, which I want to be 100 pct!]), the neutral level would go from 50 pct to 43 pct. The only way to get the neutral back to ~50 was to move through trim on the remote itself from the 2 oclock position to its current 11 oclock. Moving it back doesn't have an impact on anything.

Why is the 2 oclock position the 'right' position for this style of remote? I know I have seen that number used in more than 1 video, but they never gave an explanation.
```

---
## \#18 Posted by: Namasaki Posted at: 2017-12-25T06:48:02.104Z Reads: 89

```
According to Torqueboards who was the first to offer these remotes, The 2:00 position works best.
I have been using them for a long time on ESC's and Vescs and found the 2:00 position to work best.
Please watch the video I posted above and try following that procedure with the trim at 2:00.

this may or may not solve the problem but it's a start in the right direction.
If the remote was wired wrong by mistake at the factory, then I would do as @scepterr said and go inside and switch the wires.
```

---
## \#19 Posted by: craj1031tx Posted at: 2017-12-25T06:58:02.116Z Reads: 86

```
When I originally set up the tool I had the trim tab in the 2 oclock position and this problem was still present. I will come back and rebind tomorrow morning + try doing it in the 2 oclock position again as well. It's getting a bit late and I don't want to run into Santa :slight_smile:


Thanks for the help so far!
```

---
## \#20 Posted by: PredatorBoards Posted at: 2017-12-25T08:56:05.199Z Reads: 83

```
I'm going to assume you are using **PPM control**. Go to Motor General and set invert motor direction to **'True'**. <img src="/uploads/db1493/original/3X/7/4/74fc597218076b6ab9a58ba234f95fecfec35531.png" width="690" height="388">

Go to PPM (under app settings) and set the control type to **'Current'**
<img src="/uploads/db1493/original/3X/9/e/9ec2e14d01564f6c890c5d776aece5e0abd98c63.png" width="690" height="388">

For everybody suggesting flipping the phase wires. You should all get into the habit of reversing the motor direction via software. If you use hall sensors, the motors will always spin in one direction after re-calibration. Flipping the phase wires will simply cause the motors to cog, forcing you to re-calibrate, and return you back to square one.

Edit: I think your remote is fucked... for whatever reason. However the instructions I made should serve as a temporary fix until you find a better remote.
```

---
## \#21 Posted by: scepterr Posted at: 2017-12-25T08:59:27.927Z Reads: 71

```
Soo much time wasted solving a problem that doesn't exist 😂🤣😂🤣

@PredatorBoards the only fix is in the remote, the motor is spinning the right way
```

---
## \#22 Posted by: PredatorBoards Posted at: 2017-12-25T09:29:57.789Z Reads: 74

```
I'm aware of that. I'm just offering a temporary solution. @Ackmaniac it would be pretty cool to have a setting that allows us to essentially flip the PPM signal. So basically the VESC would interpret the PPM signal's reverse as forward, and forward as reverse.
```

---
## \#23 Posted by: scepterr Posted at: 2017-12-25T09:49:02.054Z Reads: 73

```
Right but he doesn't need to change motor rotation direction. It would be nice to implement that into v2.xx firmware if possible and add ppm reverse to both V2 and v3 firmware
```

---
## \#24 Posted by: maki Posted at: 2017-12-25T10:06:12.076Z Reads: 73

```
Guys I had the same problem with the same remote, after ordering my 4th one, it came reversed.  We are talking about the PPM signal from the transmitter being reversed and no solution that I can think of with out taking the remote apart and perhaps changing the wires on the throttle regulator.

Good 2.4 transmitters have a revers channel option, which is the way to solve this.

I just got another transmitter sent by the seller.
```

---
## \#25 Posted by: wafflejock Posted at: 2017-12-25T10:43:50.294Z Reads: 68

```
If the 5v and gnd going to the potentiometer (inside the controller) get reversed this will happen.  Typically swapping the two outside pins on the potentiometer the trigger moves around will correct this, don't swap the receiver wires though that'll do you no good.
```

---
## \#26 Posted by: GrecoMan Posted at: 2017-12-25T12:12:57.096Z Reads: 66

```
I never had a single problem with my mini from @JLabs
```

---
## \#27 Posted by: i2oadsweepei2 Posted at: 2017-12-25T13:41:25.854Z Reads: 62

```
There could be a difference then between the ones that are sourced on our behalf and the ones for $13CAD banggood. I have a couple servo signal reversers. It's just a wiring harness from hobbyking. I used to use it for four wheel steering on my rc crawlers. https://hobbyking.com/en_us/turnigy-servo-signal-reverser-long.html
```

---
## \#28 Posted by: Sebike Posted at: 2017-12-25T14:10:00.416Z Reads: 63

```
Let's just repeat the solution again. Swap 2 of the 3 wires coming off the potentiometer in the remote, usually the two outer wires. 🐷 Got the same issue with my gt2b when modding it.
```

---
## \#29 Posted by: MrCheatak Posted at: 2019-02-19T09:09:47.761Z Reads: 23

```
I had exactly the same issue after modding torque boards mini. 
I tried swapping + and —, but it was giving some weird signal. 
But throttle is basically a potentiometer as it was noted here. This means swapping polarity won't do anything, while swapping one of the power wires with the blue one will do the trick. And it worked for me.
Also misconnecting won't do any harm to the trigger, since its a resistor. Only high current would damage it.
```

---
