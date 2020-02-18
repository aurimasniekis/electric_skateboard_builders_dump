# Enertion VESC stopped working after first motor detection

### Replies: 14 Views: 4913

## \#1 Posted by: jonathanngkh Posted at: 2016-01-22T10:51:26.250Z Reads: 217

```
Hi, I had my VESC hooked up to a space cell, and VESC to my enertion r-spec motor. BLDC firmware was at 2.8, up to date, so I had no problems connecting the VESC to the BLDC tool. I was following vedder's step by step guide to getting motor detection.

Read configuration, set sensor mode to sensorless, commutation mode to integrate, motor was not carrying a load.
Ran start detection, and the motor got going! It started up super fast VEEEEEE, slowed down for awhile, then suddenly jolted up again VSH and the next thing I know, the VESC disconnected from the BLDC tool, and the blue and green LEDs that usually show the VESC is powered up no longer light up.

I'm not particularly upset about things not working, just kinda bummed cause the motor started spinning and I got so excited thinking I almost had everything in place!

What went wrong, and how can I prevent it from happening again? Could it perhaps happen to be a bad VESC? I've already ordered new ones, one from enertion and one from ollin boards as I'm really excited just to get going and riding.

Here are pictures of the VESC now, I don't have a trained eye to look for defects. Any help would be greatly appreciated, love this community.

<img src="/uploads/db1493/original/2X/9/9aef51d3dccc4c38b91e54b9b3752fbe47ba4441.jpg" width="375" height="500"><img src="/uploads/db1493/original/2X/3/35b54fd0a2f0a130dd8a71deb7a2cd4a77aeff9a.jpg" width="375" height="500">
Could the part in the red box be what's up?
<img src="/uploads/db1493/original/2X/0/02b2b32706f0bb9fd22650e440ec8f978f6af14b.jpg" width="375" height="500"><img src="/uploads/db1493/original/2X/c/c1626cf8d1127a5bbf0e6eff43dd366fdd4d124e.jpg" width="375" height="500">
<img src="/uploads/db1493/original/2X/4/404644fa3f63f85866fb83910b40f0df92cf5c0d.jpg" width="375" height="500">

I'll be more than happy to add more photos if you need a closer look at a specific part!
```

---
## \#2 Posted by: trbt555 Posted at: 2016-01-22T13:09:34.102Z Reads: 190

```
Those bridges in the red box are ok, they're bridged on the pcb too.
Did you type 'faults' in the terminal window of BLDC tool to find out if there had been any errors ?
Have you tried an alternate power supply to the VESC ?
```

---
## \#3 Posted by: chaka Posted at: 2016-01-22T14:18:57.103Z Reads: 190

```
I noticed a few possible bridges, hard to tell from a photo. Also check for bridging on the usb port.

<img src="/uploads/db1493/original/2X/c/c509289f5ba39a9fe370c0b63cd5bd44baa0864b.jpg" width="375" height="500">
```

---
## \#4 Posted by: BigAl Posted at: 2016-01-22T15:47:28.500Z Reads: 183

```
same thing happened to both of mine, good luck getting them replaced.

Al...
```

---
## \#5 Posted by: jonathanngkh Posted at: 2016-01-26T12:06:04.324Z Reads: 168

```
Thanks for the great advice @trbt555 ! It hit me the other day that my SPACE cell has a fuse so if anything happens, that should blow right? So I changed, the fuse, and my VESC lights up again! I tried running motor detection again, and the same crap(motor starts and stops abruptly, VESC no longer lights up) happens. I'm on my last fuse now, and the VESC has lit up again. There must be something I'm doing wrong that's causing it to short everytime??
```

---
## \#6 Posted by: trbt555 Posted at: 2016-01-26T13:29:12.367Z Reads: 172

```
[quote="jonathanngkh, post:5, topic:1076"]
There must be something I'm doing wrong that's causing it to short everytime??
[/quote]

I think it's a 30A fuse so there is definitely something wrong, you shouldn't be blowing it.

Unfortunately Enertion [does not test their VESC under load][1] before shipping it to customers so it's basically a hundred dollar gamble.
I speak from [personal experience][2] and the forum is littered with similar stories. 
It's a pity, the VESC is getting a bad name this way.
But let's not jump to conclusions just yet.

Where you trying to RUN the motor or where you trying to DETECT it ?
(Enertion's VESC's should already have the correct parameters for your R-SPEC so you wouldn't need to detect it)

Before you do anything else, set the *Batt max* current limit in BLDC to a value way below the fuse rating, say 10A.
Do the same with the *Absolute Max* value. That way you hopefully won't lose power to the VESC.

Now try to run the motor from the BLDC tool (up/down arrow keys) and if the VESC cops out, type "faults" in the terminal to find the faults since last boot, report back.

  [1]: http://www.electric-skateboard.builders/t/failed-vesc-help/426/34?u=trbt555
  [2]: http://www.electric-skateboard.builders/t/enertion-vesc-failure-closed/812
```

---
## \#7 Posted by: chaka Posted at: 2016-01-26T17:10:19.654Z Reads: 165

```
Be careful setting the battery max too low. Some VESC's have burned up the drv8302 from doing this. I am not sure exactly what has happened with them but I do know they were working perfectly before setting the battery max to a lower setting while still outputting 80 amps.
```

---
## \#8 Posted by: cmatson Posted at: 2016-01-26T17:15:55.219Z Reads: 169

```
Check out the recommended space cell settings(in the vesc faq section), and change your settings to match those before doing another motor detection. Also check for faults as @trbt555 said.
```

---
## \#9 Posted by: jonathanngkh Posted at: 2016-01-27T08:44:48.366Z Reads: 172

```
Okay, great news! I tried my best to follow all of your instructions.

> @trbt555 Were you trying to RUN the motor or where you trying to DETECT it ?

I was trying to detect it. I AM using the enertion r-spec motors, so I guess I'll skip on motor detection and not take the risk with blowing my last fuse!

This time, with my 3rd unblown fuse, I followed @cmatson's advice to use the recommended space cell settings. While typing in the changes to the numbers, I hit an arrow key and the motor spun up! I then found that using the arrow keys to control the motors worked fine, so that's great!

However, when I plugged in my nyko receiver using the JST connector, it doesn't work properly. What I did exactly:
1) connect VESC to bldc tool
2) read configuration, change settings, read configuration then write configuration
3) motor runs with arrow keys
4) plugged jst connected wiiceiver to appropriate ports, wiiceiver lights up and nyko controller connects to receiver, can tell from solid red light
5) changed app configuration from 'no app' to nunchuk, write configuration, reboot connection between vesc and bldc tool
6) moving the analog stick on the nyko controller does not work or affect the motor. Using the arrow keys also does not move the motor

Unplugging the receiver makes everything work again with the arrow keys. Any ideas on what's up? Also, should I change over to a different thread for this? It could still be vesc related though.

Also, I ran 'faults' in the terminal, and this is what it said:

The following faults were registered since start:

Fault            : FAULT_CODE_OVER_TEMP_FET
Current          : 14.7
Current filtered : 26.6
Voltage          : 37.58
Duty             : -0.00
RPM              : -1.2
Tacho            : -236
Cycles running   : 0
TIM duty         : -3
TIM val samp     : 1618
TIM current samp : 3718
TIM top          : 4200
Comm step        : 5
Temperature      : 251.99

Thanks a lot you guys! I'm moving forward one step at a time thanks to your help
```

---
## \#10 Posted by: elkick Posted at: 2016-01-27T09:40:53.584Z Reads: 157

```
[quote="jonathanngkh, post:9, topic:1076"]
2) read configuration, change settings, read configuration then write configuration
[/quote]


It might be not the solution for your problems (the temp fault is irritating), but the second "read configuration" in your step 2 is definitely bad idea. It switches values back to default and afterwards you're writing only the default and not your changed settings. So just omit the second "read config" and the values should be written correctly.
```

---
## \#11 Posted by: trbt555 Posted at: 2016-01-27T11:22:23.710Z Reads: 160

```
As @elkick pointed out, you may be re-writing the default settings.

Steps:

 - connect VESC to BLDC
 - App Configuration Tab
 - READ CONF
 - General tab: App to use : nunchuck
 - Nunchuck tab: control mode current
 - WRITE CONF
 - Reboot VESC
 - Reconnect VESC to BLDC
 - Tick "Display"in the App configuration/Nunchuck tab
 - Thumb the joystick and verify the signal is being received, under the "Display" tickbox you should see the bar move in sync with the joystick.

If that doesn't work, re-check your receiver-to-VESC wiring :
<img src="/uploads/db1493/original/2X/e/ea43a13722c878c33a812a3d20fb2efbba59af28.PNG" width="690" height="403">

The temperature fault (251 ° ???) is disconcerting, this may be interfering with the VESC operating correctly.
Check if this fault is coming back consistently.
```

---
## \#12 Posted by: jonathanngkh Posted at: 2016-02-01T13:00:19.720Z Reads: 153

```
I double checked all of the controller wiring, and the wiiceiver lights up when connected, and blinks when z and c buttons are pressed, but with display checkbox checked I don't see the bar moving with movement of the analog stick.

The temperature fault consistently turns up after awhile, although usually it hovers around 95-100, that one time it was a 250 was an anomaly.

I'm getting this now, it means there's a spoilt driver motor chip or something right?

The following faults were registered since start:

Fault            : FAULT_CODE_DRV8302
Current          : 5.6
Current filtered : -0.3
Voltage          : 37.58
Duty             : 0.00
RPM              : 6.4
Tacho            : 17
Cycles running   : 3
TIM duty         : 263
TIM val samp     : 10
TIM current samp : 26384
TIM top          : 52747
Comm step        : 6
Temperature      : 95.13

Fault            : FAULT_CODE_OVER_TEMP_FET
Current          : 38.0
Current filtered : 36.3
Voltage          : 37.56
Duty             : 0.00
RPM              : 2.9
Tacho            : 21
Cycles running   : 0
TIM duty         : 3
TIM val samp     : 10
TIM current samp : 2110
TIM top          : 4200
Comm step        : 4
Temperature      : 100.62

So I guess it wouldn't be wrong to say that I had bad luck with the VESC I received?
```

---
## \#13 Posted by: OGP Posted at: 2016-02-14T21:56:39.066Z Reads: 136

```
I've been following this for a little while and was curious if you had any new developments?
```

---
## \#14 Posted by: jonathanngkh Posted at: 2016-02-28T11:29:32.760Z Reads: 131

```
I ordered a new VESC from enertion since everything seemed to be so wonky, but still very doubtful about whether or not it's my fault (bad soldering, wrong wiring etc).

It arrived a few weeks ago, and I've just got it to work today! It worked straight out of the box, awesome stuff, and nice to know that I didn't do anything wrong.

Going to unscrew everything from the motor mount and re-screw it on with loctite this time! And then maybe buy a new penny board to put everything on since I have nice memories with the current one lol.
```

---
