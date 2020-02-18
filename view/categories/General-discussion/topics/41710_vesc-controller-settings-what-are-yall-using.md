# VESC controller settings (what are yall using?)

### Replies: 11 Views: 911

## \#1 Posted by: thatguy614 Posted at: 2017-12-22T17:02:44.742Z Reads: 121

```
Hey guys, I have had my board running for a few months and recently did the badwolf mod to the GT-2B controller. Since then I had to replace my battery due to a charger malfunction so my current setup is a 6s 22.2v configuration with a single VESC running firmware 2.18. 

I have my controller settings all jacked up because the badwolf mod (pictured below) allows for a greater range of motion with the throttle. Right now im having issues with full power (the settings in the screenshots give me full power in reverse but only half going forward). Also i had my controller set to reverse throttle (so the board would actually go forward) so the display for the throttle goes down when i apply forward throttle and up when i push it in reverse. <img src="/uploads/db1493/original/3X/c/c/cccb43bbf73ec96faa1f80df8ddb2ce3f9211cbd.png" width="690" height="404">
<img src="/uploads/db1493/original/3X/9/1/91d5bb1fcf3bd30ec1126518438c6afa7ee56dde.png" width="690" height="305"><img src="/uploads/db1493/original/3X/a/3/a3258e8a660acbabc3dea5d0d1721ba60dd53b99.jpeg" width="375" height="300">

I am mainly interested to hear what settings you are running with the GT-2B remote. I tried FOC for a bit before the mod and it worked well but I dont want to set anything that could damage the vesc. Let me know what yall have!! Thanks!
```

---
## \#2 Posted by: squishy654 Posted at: 2017-12-22T17:45:11.779Z Reads: 109

```
I use the PPM monitor to see the values at the top and bottom and then calibrate it manually so the trigger goes to max in the software, it's simple really..just turn on the "display" and then pull the trigger to max and write down the Pulsewidth to the right, and then enter that into Max, do the same for the bottom of the throttle at full break and enter that number into Minimum. Your Deadband is the like the Null area right in the middle where it does nothing, for safety I widen that a little in-case I nudge the trigger accidentally, and that's about it...I use FOC mode and all the auto config stuff, set it to 40a and go, never had a issue..don't try to set things all up manually and risk frying it, simple auto config does the trick..
```

---
## \#3 Posted by: thatguy614 Posted at: 2017-12-22T17:58:06.058Z Reads: 97

```
ok, that is what im using, however the display meter has been reversed (so when i put on full reverse it goes to 2.5 and then full throttle is around 0.5) I tried reversing the values in the input and it didnt work too well, it would run in reverse at about 1/4 speed and then full throttle would only give about half power.
```

---
## \#4 Posted by: squishy654 Posted at: 2017-12-22T18:06:50.736Z Reads: 94

```
there's a channel reverse switch on the transmitter itself typically to flip that very thing..looks like you have the case mod so you just have to open the case to get to the switch and travel adjust knobs, once they are set no need to open it again..
```

---
## \#5 Posted by: thatguy614 Posted at: 2017-12-22T19:21:36.340Z Reads: 83

```
yeah i have it reversed, so the board goes the right direction but it registers backwards on the BDLC tool, its really weird
```

---
## \#6 Posted by: squishy654 Posted at: 2017-12-22T19:36:47.212Z Reads: 81

```
you could reverse the TX, and then reverse the vesc, it's prolly not a huge deal but might future proof it a little for when you make changes in the future..
```

---
## \#7 Posted by: BigBoyToys Posted at: 2017-12-22T19:49:45.554Z Reads: 78

```
Best solution is for you to update your FW to Ackmaniacs 3.1 ESC tool and then check the invert motor direction on the motor tab. This will reverse the motor direction without having to flip the switch on the remote. It will also fix the power issue you are experieicing which is that you using your brake and regen current settings for forward motion.
```

---
## \#8 Posted by: BigBoyToys Posted at: 2017-12-22T20:18:50.787Z Reads: 76

```
FYI, I often find the motor direction switches when changing from FOC to BLDC control modes. Again the invert motor direction option available in the Trampa VESC Tool or the Ackmaniac ESC Tool are the easiest way to address it.
```

---
## \#9 Posted by: thatguy614 Posted at: 2017-12-23T03:50:46.280Z Reads: 68

```
good to know, I had seen something about more settings being available on the new firmware update. thanks! ill give that a try and see how it goes. Just out of curiosity which do you run your board in, BLDC or FOC?
```

---
## \#10 Posted by: BigBoyToys Posted at: 2017-12-23T04:06:48.026Z Reads: 63

```
I have 3 4wd Hub motor boards, 1 4wd Gear drive board and 1 2wd belt drive board and run high power settings and FOC on all of them.
```

---
## \#11 Posted by: GrecoMan Posted at: 2017-12-23T16:51:10.432Z Reads: 50

```
your a maniac.
```

---
