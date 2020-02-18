# Motor Has Been Sluggish

### Replies: 24 Views: 726

## \#1 Posted by: MaroonArcher Posted at: 2018-05-08T16:41:58.690Z Reads: 136

```
Hey guys, so I've been riding my DIY Board for almost a year now. I use it to get to work and around my college campus. The board runs great but the board has gotten sluggish. I am running a single belt driven motor, 10s2p battery, with a VESC. As far as the motor slowing down I've had trouble going up hill on my campus and getting good speed on the flats. The only thing I can think of is that my motor is starting to go out. I have no idea how long motors last but I use mine every day. If you guys have any suggestions let me know I've tried reprogramming my vesc to see if it was that, my connections are solid, nothing is wrong with my remote. My motor is a 6355 190kv torque board motor
```

---
## \#2 Posted by: Colson003 Posted at: 2018-05-08T16:45:38.407Z Reads: 134

```
Has your ranged decreased noticeably? It could also be the battery.
```

---
## \#3 Posted by: aigenic Posted at: 2018-05-08T16:46:46.844Z Reads: 126

```
Where did you get the battery? What cells is it made of?
```

---
## \#4 Posted by: MaroonArcher Posted at: 2018-05-08T16:51:05.242Z Reads: 117

```
Range has not decreased still getting normal usage out of it. I also just recently changed the battery pack to a custom 10s2p battery, I've been running this battery for maybe 3 months
```

---
## \#5 Posted by: MaroonArcher Posted at: 2018-05-08T16:51:50.962Z Reads: 113

```
I made the battery myself out of Samsung 25r Cells
```

---
## \#6 Posted by: E1Allen Posted at: 2018-05-08T16:54:08.398Z Reads: 108

```
What battery pack did you have prior.  And what battery Max settings are you using on your vesc
```

---
## \#7 Posted by: dg798 Posted at: 2018-05-08T16:55:59.562Z Reads: 107

```
Yeah u should double check ur vesc settings. My vesc once randomly reset all the values and I noticed it because I was going slower. Good thing I found out because I could’ve killed my batteries as the cutoff was really low.
```

---
## \#8 Posted by: E1Allen Posted at: 2018-05-08T17:01:42.489Z Reads: 101

```
I've had that happen as well.  It doesn't seem like the motor is the issue though.  Considering he said it keeps getting slower sounds like battery or vesc
```

---
## \#9 Posted by: MaroonArcher Posted at: 2018-05-08T17:12:41.821Z Reads: 101

```
Prior to my custom 10s2p I had a 12s lipo zippy 5,000mah pack connected in series. I've already checked and reset my VESC settings twice and checked remote settings
```

---
## \#10 Posted by: MaroonArcher Posted at: 2018-05-08T17:13:08.398Z Reads: 100

```
I've already checked my VESC twice
```

---
## \#11 Posted by: E1Allen Posted at: 2018-05-08T17:13:44.347Z Reads: 118

```
What's battery Max
```

---
## \#12 Posted by: dg798 Posted at: 2018-05-08T17:13:54.856Z Reads: 119

```
Take a look at this guide:
To program your VESC for the first time. I’d recommend checking this tutorial here which briefly goes over the key parts which you should do - https://www.youtube.com/watch?v=dxDXUrk-7ek.

You can plug in any voltage up to 12S. You do not need to plug in a lower voltage.

Installing The VESC BLDC Tool

Install the VESC BLDC Tool Software - www./vesc-bldc-tool-download-link/
If your on Windows - you’ll want to check to see if you have the proper drivers and your computer can see the VESC.
Your VESC will have to be powered by your battery pack or a power source. It will also need to be plugged into your motors. It does not have to be plugged into your remote controller.

Connect To Your VESC through your Computer

The first step is to connect to the VESC. You can do that on the top right and select connect on the bottom right hand corner.

If you cannot connect to the top right. I would suggest doing the following:

Check your drivers.
Check your Mini USB cable.
Try a different USB Port.
Try a different USB Cable.

What settings to change on the VESC!

The first thing is to set your VESC up in BLDC mode. BLDC mode is the easiest to setup properly. There are three modes which we recommend. BLDC mode, FOC mode, FOC Sensored mode. There is a more technical description for these modes but to keep things simple. I’m only referring to the general idea for each mode and not the actual technical term or description.
BLDC mode - The most basic and easiest mode to setup. Will have a slightly higher top speed, slightly less efficient but nonetheless the best and easiest option to use and setup which I recommend.
FOC mode - Silent, more efficient and slightly less top speed. This setup is also great and silent if your looking for a more stealthy setup. FOC is a great option to try in the future.
FOC Sensored mode - Same features as FOC mode. Sensored allows the setup to use the hall sensors which are included within all of our motors. You’ll need the VESC Sensor Wires to plug in your sensored wires from your motor to the VESC. It’s definitely a great option especially if you want a sensored setup. Sensored setup will perform much smoother than BLDC or FOC. The hardest to setup but not all that hard once you know how to setup BLDC mode and FOC mode. Only a small additional step is required.

Recommended Motor Settings in BLDC Mode.

The following below are the settings for Motor Configuration > Motor section.

Motor Configuration > Motor > Motor Type
BLDC - Select BLDC (We typically don’t use DC for ESK8. If using FOC, you would change to FOC).

Motor Configuration > Motor > Current Limits
Motor max = 80A
Motor max setting would be dependent on the max amps that your motor can handle. Ideally, you can keep it a bit lower to limit the amount of amps that your motor can handle.
If you are using our 6355 or 6374 motors. I would recommend 80A.
If you are using our 50mm motors, I would use 60A.
For hub motors, the setting for this would be lower 30-60A typically.
Motor min (regen) = -70A to -80A
Motor min is your brake setting. How strong you want your brakes.
You can use a -60A to -80A range whichever suits you best. I like to use -70A on a dual motor setup.
Batt max = 30A to 60A
Battery max is the max amps that you want to pull from your battery pack. I’d say a 30A to 60A setting is ideal.
If you're using one of our battery packs this setting doesn’t matter so much since we have a Battery Management System (BMS) which will prevent the battery from discharging more amps than necessary. However, doesn’t hurt to use this setting as well.
60A option for a Single Motor Setup.
40A option for a Dual Motor Setup.
Batt min (regen) = -6A to -12A
Battery min (regen) is regenerative braking. How much energy should go back into your battery when you apply brakes.
You don’t want an extremely high regen rate -12A+ unless your batteries can take the charge rating.
I’d keep it at about -6A for a single motor and -12A for a dual motor setup.
The other settings, you can leave as the current default.

Motor Configuration > Motor > RPM Limits (BLDC Only)
Limit ERPM with negative torque = leave this unchecked. If selected, this will apply brakes when you reach your ERPM max setting.
Min ERPM = -60000
Max ERPM = 60000
The other settings, you can leave as the current default.

Motor Configuration > Motor > Voltage Limits
Minimum input voltage = 8v
This is the minimum amount of voltage you can connect to the VESC. Keep as default.
Maximum input voltage = 57v
This is the maximum amount of voltage you can connect to the VESC. Keep as default.
Battery cutoff start = Battery in series * 3.6V
Ideally, the start you can adjust to what you prefer. A typical lithium ion cell and lipo cell useable voltage range is 4.2v (highest) to 3.0v (lowest). For Lithium Ion, you can go a bit lower but it’s typically not worth going any lower. You could also use 3.6v start and 3.4v end which is what I prefer. If you want more capacity out of your pack a 3.4v and 3.0v is ideal.
Simply switch 12S with 5S, 6S, 8S, 10S, etc. depending on the battery pack you are using with your setup.
12S battery setup is 12 * 3.6v = 43.2v
10S battery setup is 6 * 3.6v = 36v
6S battery setup is 6 * 3.6v = 21.6v
Battery cutoff end = Battery in series * 3.0V
12S battery setup is 12 * 3.4v = 40.8v
10S battery setup is 6 * 3.4v = 34v
6S battery setup is 6 * 3.4v = 20.4v

That’s pretty much it for Motor Configuration > Motor settings for BLDC Mode.

Don’t forget to hit Write configuration on the bottom left hand corner to make sure you’ve saved your settings properly.

Motor Detection is the next step.

Navigate to Motor Configuration > BLDC
In this section, you’ll run motor detection which is an automatic procedure which will make sure that your motor will be setup properly for your setup.

Motor Configuration > BLDC > Sensor Mode
Make sure “Sensorless” is selected.

Motor Configuration > BLDC > Detect Parameters
Select start detection.
Your motor should spin up. You want to make sure that your motor is fixed onto something that way it doesn’t go rolling around everywhere.
You should get a range of values if your motor detection is successful.
Select Apply which should change your settings on the top right in Motor Configuration > BLDC > Sensorless - Commutation Mode.
Once that’s done, you want to hit Write Configuration.

Double check your Motor Configuration > Advanced settings.

There are only a few options which you’ll need to check in this section.

Motor Configuration > Advanced > Current control

Startup boost (BLDC only) = .05 to .09
For the startup boost this will control your startup boost from a standstill. The higher the number the more power.
For 63mm motors I’d recommend using .05 to .07.
.08 and .09 should be used for Hub Motors.

Motor Configuration > Advanced > Backoff and ramping (DC and BLDC only)
Max current ramp step (at 1kHz) = .04
Their was a previous bug with this particular setting showing up at as .40 instead of .04. I would simply just double check to make sure the value on your VESC is .04.
If you wanted to get more performance, you can set this from .04 to .08.
If this is your first time using the VESC start by using only .04.

Don’t forget to hit Write configuration on the bottom left hand corner to make sure you’ve saved your settings properly.
Setting your remote control settings
You want to navigate to App Configuration > General. We typically recommend using our 2.4ghz Mini Remote or our 2.4ghz Nano Remote.

I would suggest having both VESCs connected using our XT90 Parallel Connector and CAN bus connector.
XT90 Parallel Connector - The XT90 Parallel Connector will connect two of our VESCs in Parallel that way they will share the same power source.
CAN bus Connector - The CAN bus Connector will connect the two VESCs to each other that way the second/slave VESC can transmit data to the master VESC.

How to program App Configuration settings for both VESCs.
Simply, just turn on power to both VESCs with XT90 Parallel and CAN bus connectors connected.
Start with Master VESC first and plug in the mini usb cable and connect to it through the VESC BLDC Tool.
Program the master VESC based off the settings below and repeat the same process for the slave VESC.

If you're using a single motor setup.

App Configuration > General
Controller ID = 0
Send status over CAN = Uncheck
App to use = PPM
For a single VESC = Select PPM
App Configuration > PPM
Control Mode = Current no reverse with brake
Multiple ESCs over CAN = Uncheck both Multiple ESCs over CAN and Enable Traction Control

If you’re using a dual motor setup.
App Configuration > General
Controller ID
For master VESC = 0
For slave VESC = 1
Send status over CAN
For master VESC = Uncheck
For slave VESC = Checked
You want to transfer the data to master VESC over CAN
App to use = PPM
For master VESC = Select PPM
For slave VESC = Select No app
App Configuration > PPM
Control Mode
For master VESC = Current no reverse with brake
For slave VESC = Disabled
Multiple ESCs over CAN = Uncheck
For master VESC = Select both - Multiple ESCs over CAN + Enable Traction Control (current mode only)
For slave VESC = Select both - Multiple ESCs over CAN + Enable Traction Control (current mode only)

Don’t forget to write configuration and afterwards you should be good to go.
What’s next?
Connect the male to male connector to the master VESC.
Bind the Mini Remote or Nano Remote to the receiver.
Turn your setup on and test your remote to see if the wheels spin.
```

---
## \#13 Posted by: aigenic Posted at: 2018-05-08T17:19:18.653Z Reads: 86

```
I guess this is a bit off topic :confused:
```

---
## \#14 Posted by: MaroonArcher Posted at: 2018-05-08T17:32:09.439Z Reads: 81

```
Battery max is set to 75
```

---
## \#15 Posted by: E1Allen Posted at: 2018-05-08T17:44:27.709Z Reads: 80

```
I think you're smoking your batteries. Which can handle maybe 40a
```

---
## \#16 Posted by: linsus Posted at: 2018-05-08T17:49:48.167Z Reads: 80

```
Electrical Motor dsnt have an expirydate. The bearings in the motor might wear out eventually, but you should hear that difference quite noticeably.

Gut says its your battery. Logging your ride will tell you whats going on
```

---
## \#17 Posted by: MaroonArcher Posted at: 2018-05-08T17:51:13.853Z Reads: 80

```
Sorry motor max is at 75 my battery is at a max of 35
```

---
## \#18 Posted by: dg798 Posted at: 2018-05-08T18:01:05.726Z Reads: 79

```
Try redoing a motor detection.
And type faults into the terminal
```

---
## \#19 Posted by: E1Allen Posted at: 2018-05-08T18:52:41.957Z Reads: 74

```
Possible bad parallel group with the pack.  Not likely but maybe
```

---
## \#20 Posted by: MaroonArcher Posted at: 2018-05-08T21:46:31.983Z Reads: 67

```
If it was that my voltmeter wouldn't be reading right and the pack wouldn't discharge properly and it wouldnt charge properly
```

---
## \#21 Posted by: E1Allen Posted at: 2018-05-08T22:07:31.066Z Reads: 65

```
Check all the solder joints.
```

---
## \#22 Posted by: MaroonArcher Posted at: 2018-05-08T23:18:22.458Z Reads: 59

```
I didnt solder I spot welded it together
```

---
## \#23 Posted by: E1Allen Posted at: 2018-05-08T23:49:35.370Z Reads: 53

```
Battery to the vesc to the motor. All of them
```

---
## \#24 Posted by: Scoo_B_SK8 Posted at: 2018-05-09T00:57:01.885Z Reads: 48

```
Screen shot your current settings used.  I know you’ve mentioned a bunch but would be easier for others if it was all in one post (pic’s are worth a 1k words 😉)
```

---
