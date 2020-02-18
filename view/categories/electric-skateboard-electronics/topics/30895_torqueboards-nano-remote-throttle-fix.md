# TorqueBoards Nano Remote - Throttle Fix?

### Replies: 43 Views: 2605

## \#1 Posted by: Veovis Posted at: 2017-08-17T15:39:00.850Z Reads: 198

```
I'm using the Nano remote from diyelectricskateboards, and when I move the throttle it seems like I have maybe 3mm between no power and full speed. I've searched the forums but I can't find any concrete answers as to how I can adjust the throttle.
```

---
## \#2 Posted by: Veovis Posted at: 2017-08-17T15:40:04.191Z Reads: 202

```
Also I did check out the extended bldc tool by @Ackmaniac, but from the comments it seemed like some people couldn't fix the issue with it.
```

---
## \#3 Posted by: Jinra Posted at: 2017-08-17T15:43:36.075Z Reads: 196

```
The remote has to be calibrated between each use (power cycle). Simply throttle all the way forward and all the way back so the remote knows what max/min throttle is, otherwise the slightest movement will result in full throttle/full brake. This is also true on the Enertion Nano-X (raptor 2) remote.

It's an unfortunate design flaw, but I think it comes with the territory for auto-bind remotes.
```

---
## \#4 Posted by: Veovis Posted at: 2017-08-17T15:49:21.654Z Reads: 187

```
So the process is
1. Turn on the remote
2. Press the throttle all the way forward/back
3. Turn on the board/reciever

And then it should be calibrated?
```

---
## \#5 Posted by: Jinra Posted at: 2017-08-17T15:51:45.535Z Reads: 177

```
Yea you can do it that way. For me I do this.

1. Turn on board
2. Turn on remote
3. Very quickly throttle up and down (takes less than half a second) before it pairs
4. Remote pairs

The only thing you have to be mindful of is not have the throttle anywhere other than neutral when the pairing actually happens (light goes from blinking to solid). Otherwise you're neutral will be wherever you had the throttle when it paired.
```

---
## \#6 Posted by: Veovis Posted at: 2017-08-17T15:54:37.566Z Reads: 159

```
Thanks! I tried it out and the last 30% of the forward throttle is still full power, but that's better than what I had before. If I have to do this pairing setup every time, I might get rid of my anti-spark loop and just get a vedder switch
```

---
## \#7 Posted by: Jinra Posted at: 2017-08-17T15:56:23.384Z Reads: 149

```
What does your remote have to do with your power switch :thinking:?

Keep in mind when using current/watt control your throttle does not directly control your speed, but rather your acceleration.
```

---
## \#8 Posted by: Veovis Posted at: 2017-08-17T15:59:41.975Z Reads: 149

```
Well when I tried that process, it was just kind of a pain to pull the key in and out to restart the process if I didn't get the calibration right. But if I just have to flick a button then it wouldn't be as much of a hassle.

Maybe I'm making excuses to get an actual switch lol
```

---
## \#9 Posted by: Jinra Posted at: 2017-08-17T16:03:05.785Z Reads: 143

```
Ah gotcha. Yea I find my push button to more elegant, though I prefer flip switches myself.
```

---
## \#10 Posted by: Veovis Posted at: 2017-08-17T16:03:53.220Z Reads: 144

```
Do you have a recommendation for one that's reliable? I keep hearing about people blowing their vedder switches
```

---
## \#11 Posted by: Jinra Posted at: 2017-08-17T16:06:20.609Z Reads: 144

```
I use the torqueboards switch. I've heard of people blowing those as well, but mine has lasted nearly a year of constant use and I've been fine. You could try one with direct fets as they may last longer. The ones that blow tend to have their fets blown to a always on/off position.

http://www.electric-skateboard.builders/t/new-directfet-anti-spark-switches-with-onboard-led-circuit/18762
```

---
## \#12 Posted by: Veovis Posted at: 2017-08-17T16:08:56.977Z Reads: 132

```
Good to know, that's probably the one I'll go with
```

---
## \#13 Posted by: SilentException Posted at: 2017-08-17T20:37:17.652Z Reads: 125

```
One possible fix or workaround would be to implement option for stick arming on the (V)ESC, like quadcopters flight controllers have. You would be unable to start the motors before some stick movement up and down, basically calibrating remote. That would require modifying (V)ESC firmware and not many people are able to do that. I proposed it in Ackmaniac's thread because he is doing a great job on the modified firmware but there were no replies. I started some work myself but there is simply no time for everything :)

https://www.electric-skateboard.builders/t/extended-bldc-tool-with-watt-control-mode-ppm-cruise-control-individual-throttle-curve-and-android-app/12286/1310
```

---
## \#14 Posted by: SORRENTINO Posted at: 2017-08-17T20:51:12.975Z Reads: 119

```
You can permanently bind the remote to the receiver so you dont have to calibrate anymore. Ill try to find the link with instructions on how to do this.
```

---
## \#15 Posted by: SilentException Posted at: 2017-08-17T20:55:04.522Z Reads: 114

```
Probably thinking of v1 Nano and not v2. But if yo do mean v2, that would be awesome :)
```

---
## \#16 Posted by: SORRENTINO Posted at: 2017-08-17T20:56:37.639Z Reads: 111

```
Yea it is for the V2 Nano. Both my Buddies did it with theres.
```

---
## \#17 Posted by: SilentException Posted at: 2017-08-17T21:07:33.716Z Reads: 107

```
Hell yeah, if you find the instructions I'll finally switch from v1! Only for the shape, v2 is nicer :)
```

---
## \#18 Posted by: SORRENTINO Posted at: 2017-08-17T21:10:18.010Z Reads: 102

```
So you basically jump the ground and signal pins on the receiver pins on the bind channel. Then power board up. Hold channel 2 button in and power up the remote. Wait for lights to go solid and Center the throttle with a spring flick ( pull back to full brake then let go ). Pull bind pin to set failsafe. Turn off board and remote. Adjust endpoints in bldc software if you have to and you're good to go. @Deckoz is this correct?
```

---
## \#19 Posted by: Deckoz Posted at: 2017-08-17T21:12:16.138Z Reads: 103

```
yea...basically the only reason i say spring flick to let it recenter is it allows the spring to naturally center. once it naturally centers, pull the bind pin and it sets the failsafe.

you should have self healing(recovery) of failsafe which wont require rebooting the board to rebind like autobind requires as well
```

---
## \#20 Posted by: Jinra Posted at: 2017-08-17T21:25:23.567Z Reads: 102

```
omg if this works, Imma love you.
```

---
## \#21 Posted by: SilentException Posted at: 2017-08-17T21:26:36.158Z Reads: 99

```
So basically you just do the similar binding/failsafe procedure as you would normally do on v1. FFS, why haven't I tried that before :) Hope it works! Thanks so much!
```

---
## \#22 Posted by: Deckoz Posted at: 2017-08-17T21:37:57.366Z Reads: 106

```
Yes basically its the manual bind procedure.

Fixes range to be 400ish ft vs 35
Fixes failsafe self healing
Fixes drop outs
Fixes needing to reboot the board when turning the remote off but not power cycling the board
And it sets the true failsafe ppm value for your specific throttle actuators natural spring resting place

Make sure to set your ppm center points and endpoints too
Ie hold full throttle set ppm max to the value the vesc is reading, same for center and full brake
```

---
## \#23 Posted by: Veovis Posted at: 2017-08-18T00:03:23.787Z Reads: 104

```
I might need these instructions in ELI5 format... :joy:
```

---
## \#24 Posted by: Deckoz Posted at: 2017-08-18T01:13:08.214Z Reads: 100

```
@Veovis

Plug in bind plug(short the ground and signal wire on the receiver on the bind slot)
Plug in board
Receiver should be flashing red

Hold the pinky button on the remote(do not let go)
Turn on the remote, continue to hold pinky button
After a few moments the LEDs on both the receiver and remote turn solid, you can now release the pinky button

Not necessary but I like to pull the throttle back and swiftly let go allowing the spring to center the throttle. This allows a natural spring center. Once satisfied with the throttle in center dont touch any buttons or the throttle, pull the bind plug. Pulling the bind plug sets the failsafe ppm value.

Your now bound and can power off the remote and board.
You can test failsafe by turning the remote off and back on with the board on, it should now self heal.

Before testing the failsafe centering. Go into the VESC on the PPM tab with Motor control disabled. The green bar at the bottom has a numerical output

-put the throttle on the remote to full - read the value on the green bar. Put that value in PPM max pulse width
-put the throttle on the remote to full break - read the value on the green bar. Put that value in ppm Min pulse width
-allow the throttle to center by spring, read the value on the green bar. Put that in ppm center

Write the configuration, re-enable motor control. Push the throttle to make the motors spin and turn the remote off while holding the throttle. The wheels should coast, not break or accelerate more. If they coast your failsafe center is set properly.

Is that good enough?
```

---
## \#25 Posted by: Jinra Posted at: 2017-08-18T01:24:35.305Z Reads: 89

```
Just to confirm the bind slot is the first (top) row of pins right?
```

---
## \#26 Posted by: Veovis Posted at: 2017-08-18T01:30:16.078Z Reads: 92

```
Hmmm I'm not sure. My failsafe seems like it's always been working, but my main concern was just fixing the throttle sensitivity and giving myself more range between stopped and full speed. I had tried adjusting the values in the PPM tab earlier this week but nothing really changed.
```

---
## \#27 Posted by: Deckoz Posted at: 2017-08-18T02:11:10.576Z Reads: 94

```
Yep top row of pins


@veovis once you do this it should fix it. Just always turn on the remote first then the board when you goto ride
```

---
## \#28 Posted by: SilentException Posted at: 2017-08-18T22:58:29.578Z Reads: 93

```
@Deckoz @SORRENTINO

I don't think this does anything. Or maybe I'm just doing something really wrong. Anyhow, made a video explaining the original issue and then trying manual binding fix, twice, without success. If you could take a look...

https://youtu.be/m1TFuuFRk5M
```

---
## \#29 Posted by: Deckoz Posted at: 2017-08-18T23:02:01.983Z Reads: 90

```
I dunno man. This is what fixed my remote that was ordered about 2 months ago. Maybe they're different versions?

Worst case just turn in remote and move the throttle to full then full reverse then power on the board.
```

---
## \#30 Posted by: SilentException Posted at: 2017-08-18T23:04:06.820Z Reads: 89

```
[quote="Deckoz, post:29, topic:30895"]
Worst case just turn in remote and move the throttle to full then full reverse then power on the board.
[/quote]

But that's exactly the issue I've been hoping to fix :D Anyhow, I don't think binding procedure does anything for the remote or the failsafe. Also got the remote around 2 months ago.
```

---
## \#31 Posted by: Jinra Posted at: 2017-08-18T23:05:13.975Z Reads: 83

```
Do you have to, perhaps, hold the button on the bottom near the power switch down while you turn on the remote?
```

---
## \#32 Posted by: SilentException Posted at: 2017-08-18T23:05:50.040Z Reads: 82

```
Tried it both ways, it was in the video.
```

---
## \#33 Posted by: Jinra Posted at: 2017-08-18T23:06:10.125Z Reads: 81

```
Ah sorry, I only watched up to after the first bind attempt
```

---
## \#34 Posted by: SilentException Posted at: 2017-08-18T23:11:25.093Z Reads: 78

```
Yeah, also opened the remote hoping there would be a hidden binding switch but no.
```

---
## \#35 Posted by: Jinra Posted at: 2017-08-18T23:12:11.440Z Reads: 76

```
Yea, it must be the fact that these things autobind.. Even Enertion doesn't have a solution for their remotes on this.
```

---
## \#36 Posted by: SilentException Posted at: 2017-08-18T23:15:21.490Z Reads: 78

```
So damn annoying. It is simply unsafe to use it like this. If I forget, damn thing will throw me off the board on start or while braking. And if I forget about this while letting my wife or colleagues try the board, it could be even worse.
```

---
## \#37 Posted by: Jinra Posted at: 2017-08-18T23:16:43.337Z Reads: 77

```
Definitely the biggest downside of the remote, but hey it's a LOT better than v1 (winning) remote, where it'll cutout randomly. The v2 has failed to cutout on me a single time so far.
```

---
## \#38 Posted by: SilentException Posted at: 2017-08-18T23:18:07.367Z Reads: 77

```
Funny thing is I am actually using v1 instead of v2 because of this issue. I haven't had any cutouts with either. Guess I was very lucky with my v1 sample.
```

---
## \#39 Posted by: Jinra Posted at: 2017-08-18T23:19:04.764Z Reads: 78

```
I ride in a city with lots of 2.4ghz congestion (among other radio traffic) and I would never, ever try the v1 again.
```

---
## \#40 Posted by: SilentException Posted at: 2017-08-18T23:26:22.635Z Reads: 79

```
Same here, using v1 in the city or outside, made no difference. I do believe v2 is far better and v1 is simply unsafe for most. But I won't switch unless I notice my v1 acting up. Sample variance is a thing in any product. I also think that board thickness and materials do matter a lot for v1, it looks like it is very sensitive to interference.
Now let us hope for the ultimate v3! :)

Does anyone have any contacts for Winning? I'd like to send my feedback and suggestions to them.
```

---
## \#41 Posted by: pshaw Posted at: 2017-08-30T04:30:35.102Z Reads: 74

```
So I actually have to do the calibration as well and never could get the manual bind mode to work so that i wouldn't have to manually calibrate when I turn on remote. @jinra did you ever get it to work correctly? 

I'm almost certain I'm out of autobind too as when i turn the remote off then on again it INSTANTLY rebinds and turns solid green. Like less than a second for sure.
```

---
## \#42 Posted by: Jinra Posted at: 2017-08-30T04:32:36.863Z Reads: 74

```
No I haven't tried yet since I heard it doesn't really work. Also, once it binds it seems to reconnect pretty fast, try leaving it off for a minute or two then turning both back on again.
```

---
## \#43 Posted by: lukeschley Posted at: 2018-03-23T16:57:21.367Z Reads: 54

```
has anyone got to the source of this
```

---
