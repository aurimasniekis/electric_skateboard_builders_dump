# Loss of brakes. Help!

### Replies: 27 Views: 1786

## \#1 Posted by: joeadams101 Posted at: 2017-07-16T16:54:43.552Z Reads: 80

```
Hello, I have been having an issue when I use the brake, first off it seems it takes forever to brake and second if I keep it long pressed it like stops braking ( you feel the snap) then if you let go of it and brake again it goes back to braking. Anyone has had this issue before?

I am using 

10s battery
190kv motor
Standard enertion vesc


<img src="/uploads/db1493/original/3X/c/c/ccace7679b83be114946252e496a9d388d4b9a4e.png" width="690" height="431">
```

---
## \#2 Posted by: Martinsp Posted at: 2017-07-16T16:59:28.365Z Reads: 70

```
For harder braking you should set your motor min to -60A... that max and min settings on motor are to limit the power that the motor is using to turn "forward" and "backward".
```

---
## \#3 Posted by: SeanHacker Posted at: 2017-07-16T17:02:01.260Z Reads: 72

```
Looks like you need to update some of those settings. You're ERPM values are screwed most importantly. I have a 10s and here are my settings.

Motor max 60 
Motor min -50 (if the brake is too powerful reduce it, if too weak you can go up till -60)
Battery max 30 (if the board is too powerful reduce it. Depending on the type of batteries you can go up.)
Battery min -10 (correct would be -8 but to have some space in times of crisis)
**Min ERPM -60000**
**Max ERPM 60000**
Battery cutoff start 30
Battery cutoff end 28
```

---
## \#4 Posted by: Jinra Posted at: 2017-07-16T17:09:23.930Z Reads: 66

```
His erpm settings aren't screwed up. 100k is default and is fine on good 10s 190kv setup.
```

---
## \#5 Posted by: Sander Posted at: 2017-07-16T17:13:12.044Z Reads: 63

```
Did you brake when your board was fully charged?
```

---
## \#6 Posted by: SeanHacker Posted at: 2017-07-16T17:13:31.450Z Reads: 60

```
Alright. I was always told the 60000 is that max ERPM that should be used. I'm running 10s 190kv. Weird. Guess I'll have to look into it.
```

---
## \#7 Posted by: Jinra Posted at: 2017-07-16T17:17:10.516Z Reads: 56

```
You only need it if your setup exceeds 60k erpm.
42v * 190kv * 7 pole pairs * .95 duty cycle = 53k erpm
```

---
## \#8 Posted by: SeanHacker Posted at: 2017-07-16T17:20:57.052Z Reads: 55

```
Thanks for the info dude!
```

---
## \#9 Posted by: joeadams101 Posted at: 2017-07-16T17:25:17.455Z Reads: 53

```
Hey @Sander it happens at any battery %
```

---
## \#10 Posted by: joeadams101 Posted at: 2017-07-16T17:26:01.628Z Reads: 53

```
Why -? I have never seen people run -60 on motor max. Correct me if I am wrong
```

---
## \#11 Posted by: SeanHacker Posted at: 2017-07-16T17:28:39.817Z Reads: 54

```
At -30 Motor Min your brakes might be relatively weak. I use -45/-50 most of the time with my 83mm wheels. When I put on my MBS 100mm I need to use -60 or the brakes are just too weak.
```

---
## \#12 Posted by: Sander Posted at: 2017-07-16T17:39:32.917Z Reads: 52

```
Maybe it is your remote?
GO on App Configuration then the PPM tab and click on the Display check box?
```

---
## \#13 Posted by: joeadams101 Posted at: 2017-07-16T17:58:00.198Z Reads: 53

```
maybe. I got 83mm as well
```

---
## \#14 Posted by: joeadams101 Posted at: 2017-07-16T17:58:06.756Z Reads: 52

```
Let me try it now
```

---
## \#15 Posted by: joeadams101 Posted at: 2017-07-16T17:59:45.333Z Reads: 51

```
on max throttle its 2.0 and on max brake is 0.62
```

---
## \#16 Posted by: joeadams101 Posted at: 2017-07-16T18:02:51.482Z Reads: 48

```
<img src="/uploads/db1493/original/3X/7/0/701346b16fe2455e9e3df048ab8e9a57e02f6081.png" width="690" height="359">
```

---
## \#17 Posted by: Sander Posted at: 2017-07-16T18:19:11.881Z Reads: 44

```


Does the bar go back to the end of left?
```

---
## \#18 Posted by: joeadams101 Posted at: 2017-07-16T18:20:16.189Z Reads: 43

```
Yes like this.

<img src="/uploads/db1493/original/3X/1/5/156386a192703d7d6c8efe8fa1d2d37ff9baba11.png" width="690" height="111">
```

---
## \#19 Posted by: Sander Posted at: 2017-07-16T18:21:39.404Z Reads: 44

```
Ahh, then I dont know :(
```

---
## \#20 Posted by: joeadams101 Posted at: 2017-07-16T18:22:17.352Z Reads: 49

```
I am going to try changing the motor min and see if that helps! Thanks for the info though! Ill let you know how it goes
```

---
## \#21 Posted by: Martinsp Posted at: 2017-07-16T20:56:44.299Z Reads: 43

```
Of course it does not work... I didnt see it before but now I am like heureka damn it :D 

What you have to do: 
1. connect VESC to BLDC-tool 
2. on the app config tab enable the display option (be sure to set PPM as "disabled" to avoid unwanted motor spin)
3. enable the display option as you did before
4. push your trigger on remote all the way to max brake 
5. next to the line there is a number, put that number into the "minimum pulsewidth (ms)" 
6. do the same for acceleration

What was happening was that you were not using all the range that your remote offers.
```

---
## \#22 Posted by: Martinsp Posted at: 2017-07-16T20:59:14.318Z Reads: 42

```
If you adjusted anything on your remote like the trimming option to achieve 50% in the BLDC-tool before, make sure to set these back. Otherwise you wont get 50% while trigger is in resting position.
```

---
## \#23 Posted by: joeadams101 Posted at: 2017-07-17T00:43:02.159Z Reads: 42

```
I see. So i got to set the minimum instead of 1....to the 0.62 that you saw on the screenshot ? Where its me with full brake on
```

---
## \#24 Posted by: wafflejock Posted at: 2017-07-17T01:04:07.518Z Reads: 45

```
Your full brake and full acceleration ms values the receiver sends to the VESC based on your controller input needs to rest at 50% or idle when you are not pulling the trigger.  Usually the progress bar on Ubuntu shows the actual percentage in there with yours it appears to just be a line basically so will be harder to get the value right.  Full brake should be the minimum ms value though and full throttle should be the maximum, in theory when you let go of the trigger it should go to idle.  If it goes above 50% when you let go then your high is too low or your low is too high (the middle is therefore too high), if it goes below 50% then your high is too low or your low is too high.  You can also adjust the deadband which is a perecentage around the 50% mark that it will consider "dead" or idle, to get it to accelerate or decelerate you need to pull or push the trigger out of the deadband region into the "active" region.
```

---
## \#25 Posted by: lrdesigns Posted at: 2017-07-17T01:13:29.828Z Reads: 45

```
I had this exact issue with a GT2B remote in a baby buffalo case. Which remote do you have?
https://www.electric-skateboard.builders/t/gt2b-baby-buffalo-mod-case-3d-printable-thumb-throttle-case/4694 

The reason is if the brake signal goes past the end point of the PPM setting. The vesc will see this as signal loss and cut out. It comes back when you move the brake back closer to the middle. To fix the issue I had to put a physical stopper on the remote so I could not press it all the way in. Its a work around. To fix it properly I installed @Ackmaniac extended BLDC tool which you can set the end points to match what the remote puts out.  https://www.electric-skateboard.builders/t/extended-bldc-tool-with-watt-control-mode-ppm-cruise-control-individual-throttle-curve-and-android-app/12286
```

---
## \#26 Posted by: Jinra Posted at: 2017-07-17T03:21:34.805Z Reads: 40

```
That's weird since @Ackmaniac's PPM wizard will set the PPM min/max higher and lower (respectively) than my actual values. For example, my remotes actual min is 1.10 and max is 1.96, but the wizard sets it at 1.11 and 1.94
```

---
## \#27 Posted by: lrdesigns Posted at: 2017-07-17T03:27:24.214Z Reads: 39

```
I think just slightly past still works but if its a lot past the vesc will think the signal is lost and cut out. I prefer my remote end points to be just inside the PPM BLDC end points for added safety.
```

---
