# Help! dead vesc, what did i do wrong!?

### Replies: 5 Views: 1015

## \#1 Posted by: AdsGudz Posted at: 2017-03-20T18:21:46.165Z Reads: 103

```
While setting up my vesc it suddenly startet to smoke and died.


Vesc: Maytech 2.18
Motor: Turnigy sk3-6364-245kv
Kontroller: nunchuk
Batteries: 2X Turnigy 5S 5000 mah 20-30C

Following a vesc setup tutorial, rebooting after every setting I changed, I managed to set my vesc up for bldc with a nunchuck kontroller and all worked fine! 

Then I tried to to set my vesc up in FOC mode for a smother ride. Following the tutorial I First red default config, reboot and then started the "MEASURE R AND L" test. All worked fine. Applied the results. Rebooted. Started the next test and cal CC after that, applied and then reboot.

Then I tested to accelerate with cruisecontroll pressed in. The motor started to turn slowly but when I let go of the accelerator the motor started to turn fast back and fourth faster and faster and the vesc started smoking and i pulled out the battery as fast as i could but then damage was already done and the VESC is dead.

These were the settings I runned when it happend and some realtime data. Please help me to find the problem or wrong setting.

<img src="/uploads/db1493/original/3X/f/7/f78fddac5681e54adbe0ec5286fab00fcae9e6e0.png" width="690" height="368"><img src="/uploads/db1493/original/3X/1/6/16f2e4dfa71a6f407df0b10a5539f1abdf1e792d.png" width="690" height="368"><img src="/uploads/db1493/original/3X/1/f/1f7bccc079a8859a976bd331d7ac589b60732781.png" width="690" height="367"><img src="/uploads/db1493/original/3X/9/8/9819bd097c7e713d77c9df6bc3c72368fb1531a5.png" width="690" height="367"><img src="/uploads/db1493/original/3X/a/8/a8fc6bd8e87afaa8024103f93a41cc790418d40b.png" width="690" height="368">
```

---
## \#2 Posted by: treenutter Posted at: 2017-03-20T18:35:54.626Z Reads: 87

```
Sorry to hear it @AdsGudz. Running 10S w a 245KV motor creates the potential to exceed the RPM limit of VESC and overheat your DRV chip.  I see that you had ERPM set in the nunchuck app, but not on the motor config tab for FOC. Was the ERPM limit in the nunchuck app applied when you  had the problem? Between the two, I'm not sure which takes a higher order (i.e. I'm not sure which limit is honored with they are different). If you take a photo of your VESC and post it that will help. DRV replacements are possible, so you're VESC is revivable if that is the problem. Right now your screenshot shows no Fault Code, is this before or after the event?

A few tips: with a 10S battery and VESC use ~190KV motors. When you switch from BLDC to FOC mode, re-install the firmware to wipeout all past settings from BLDC mode. IMO (which is controversial haha) nunchuck is just not a good solution for control, a GT2B w a mod is more reliable.
```

---
## \#3 Posted by: AdsGudz Posted at: 2017-03-20T18:45:09.108Z Reads: 84

```
Ok!Thanks! I thought it was ok with the nunchuk erpm limit 

<img src="/uploads/db1493/original/3X/c/1/c13a00bb787ec61fd81054027aed2f58ddbd9378.jpg" width="666" height="499">

As you can see DRV is cracked. WHERE is it possible to get these repairs? The nunchuck erpm was engages when the problem accured. Why do think it was going forward and backwards when the nunchuk was in "neutral"? This was after the event but I pulled out all the cabels when it started to smoke. Does that have a inpact of the foult codes?
```

---
## \#4 Posted by: AdsGudz Posted at: 2017-03-20T18:47:45.632Z Reads: 78

```
I really like the cruise-control option on the nunchuk tho :stuck_out_tongue:
```

---
## \#5 Posted by: tilmnater Posted at: 2017-03-21T01:47:45.412Z Reads: 59

```
@JohnnyMeduse should be able to help you out depending on where you are located. If you don't want to buy a new motor, just make sure to adjust your max erpm. I also set soft rpm limits to 58k start and 60k end. Read [this thread](http://www.electric-skateboard.builders/t/vesc-settings-for-maximum-potential-8s-260kv/10678) for more info:
```

---
