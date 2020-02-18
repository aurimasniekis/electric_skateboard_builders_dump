# Unable to accelerate/get power into motors via remote control

### Replies: 12 Views: 262

## \#1 Posted by: r3vilo Posted at: 2018-10-30T07:50:13.429Z Reads: 80

```
Hi.

I have some weird behavior since the last fw update. Everything worked fine before with version 3.38. I updated to 3.40. Did a new Motor Setup and Input Setup Wizard in VESC Tool. And after that I had this:

https://www.youtube.com/watch?v=tSbszHjG26k

I push the remote all the way up and it does almost nothing. The wheel moves with 1 rpm or what this is. I did firmware updates before, so it's not new to me and I know what I'm doing. Did the settings like everytime. Maybe with fw 3.40 there are more values and something which is stock differs from before, idk?

I have the "Dual Beast" from eskating.eu. 

It's 12S5P 30Q in FOC mode with 2 x 6355 motors (each 3510 W).

I also ran the setup for BLDC mode with and without sensors it's always the same. Using VESC Tool 0.92 instead 0.95 (newest) for downgrading back to fw 3.38 suceeded but after that I had the same behavior. Normally it has to be like before if it was a software issue, right? Because eveytime I reset the settings to default.

I don't remember but I think it is correct when VESC Tool shows HW 410 when connected to a FOCBOX 4.12. I think it does that. Or should it show 412? I think it was 410 always. Actually you can only choose 410 & 411 & 412 when updating the firmware.

As you can see in the video, doing the motor setup wizard it spins up the wheel normal. That means the VESCs can send power to the wheels. If I do with the remote later, I get almost nothing. What could this be? I thought when the electronics can control the motor like normal it could only be the receiver or the remote. That's why the video description.

But after thinking again this could not be, because the input setup wizard where I configure the remote shows normal results. Throttle from 0% to 100% and brake from 0% to -100%. I applied the values (phaselength) and it should work fine. And if in VESC Tool the remote is recognized as usual and the bars are moving every milimeter I move the throttle/brake on my remote then also the receiver and the remote are working fine, right? ... So, I don't get what went wrong. What is causing this behavior.

The hardware should be ok. Receiver, remote, VESCs, all wires etc. because VESC tool spins up the wheels in the setup. Also my values for the remote in input setup showing correct results.

What is it then? Anybody else had this issue before? I'm on the end of my knowledge.

And one more thing: Because I have the Landyachtz Evo deck and the board came with angled riser pads I changed these to normal risers before the fw update, because I wanted to have the normal geometry of the board/deck. It doesn't make sense to me to "destroy" this with angled risers. Unfortunately I did not test before the fw update. OK, I only removed the trucks and changed the risers. Then tightened everything again. ... And like I said above, it could not be that I damaged a wire here while doing this because VESC Tool is able to spin up the wheel, right? Only thing now what I haven't had before is, that in motor setup, when measuring flux linkage I have to change the "D" value from 0.5 to 0.3. If not it fails. With 0.3 is succeeds, shows eveything green and I can go on. Is this a hint to an issue?

Thanks for helping and sorry for the long text. I want to ride that thing again so bad! Thx.

EDIT: If you wont scroll down, heres a video of the complete setup:

https://youtu.be/2p5lPpnjxpc

**UPDATE!!!**

**PART 3 - BLDC mode sensorless**

https://www.youtube.com/watch?v=jHvcNFOILQ0

**BLDC with no sensors works!** :D 

Detection also fails. I get on the bottom right a "Bad Detection Result Received" and in the main window it says "Detection failed" (as before) but if I go on by pressing "next" it says setup is complete and I should go on with App Setup. No warning, nothing.

Looks like I can ride again, even if in BLDC mode with no sensors. Only thing I worry about is, that with going further by clicking "next" the default values of

Cycle Integrator Limit (62,00) and
BEMF Coupling (600,00)

will be applied. I don't know if this could have an negative effect or damaging even more. Obviously these values should be calculated in detection and because of failing I don't have the correct values here, right?

Can someone confirm that these two values don't do nothing what can cause damage to the motors or even the battery? Fire or something? Blocking wheels that I will fall off suddenly?

The help text says the following:

Cycle ingegrator limit. This is how much area will be integrated under the back EMF after a zero crossing before doing a commutation. A too low value will cause a too early commutation, and a too high value will cause a too late commutation. A too late commutation will cause more problems than too early commutations.

BEMF coupling. Roughly describes how much of the input voltage is seen on the BEMF at low modulation. Compensating for that at low speed helps the startup al lot.

Nontheless it seems my sensors have a problem or are damaged? If I try BLDC with Hall Sensors, detection fails as expected. When I skip here also with "next" and complete the setup, afterwards, when I press the throttle on remote it only beeps. Maybe because the sensor settings are Hall Table [0] -1, Table [1] 1, Table [2] 3, Table [3] 2, Table [4] 5, Table [5] 6, Table [6] 4 and Table [7] -1, becaue that's default and don't matching with my sensors/motors.

So for now I'm using BLDC sensorless. Seems to work.

Any tips for my problems? If my sensors are defective do I need new motors? Is it ok to ride in BLDC sensorless mode then? What are your suggestions to do now?

Thanks.

**UPDATE: Riding doesn't work** :( :( :frowning:

**Just wanted to ride but it doesn't move with wheight on it. It tries to but has not enough torque or power to do. If I lift it up it spins like in the last video. I think specific values still have to be edited.**
```

---
## \#2 Posted by: taz Posted at: 2018-10-30T08:03:44.697Z Reads: 61

```
If possible take a video of you setting up the input wizard, start to finish.
```

---
## \#3 Posted by: taz Posted at: 2018-10-30T08:11:30.354Z Reads: 60

```
Now that I think about it. Do the same for the motor wizard.
My guess is you have not applied the settings at some point.
```

---
## \#4 Posted by: Andy87 Posted at: 2018-10-30T08:14:38.274Z Reads: 62

```
what he :point_up_2: said
plus make sure your remote is charged.

I don´t know about the D value, but maybe try to set up in BLDC and look if there your remote is working.
Than you know if it´s the problem or not.
```

---
## \#5 Posted by: r3vilo Posted at: 2018-10-31T06:14:29.297Z Reads: 41

```
OK, thank you so far. And my remote is working fine, at least in the setup. I will make a video of the complete process.
```

---
## \#6 Posted by: Winfly Posted at: 2018-10-31T08:42:22.126Z Reads: 40

```
Make sure you hit that write app setting.
```

---
## \#7 Posted by: r3vilo Posted at: 2018-11-01T09:37:35.180Z Reads: 36

```
https://youtu.be/2p5lPpnjxpc

OK, here's the complete setup. Remote was fully charged, the board at 92%.

I applied the values after each test and wrote everything to the VESC afterwards. I did that also before, but that's the proof. Configuring as BLDC instead if FOC gives the same result.

So my question is: Why is the VESC in the motor setup able to spin the wheel up and if I give throttle with the remote it barely moves? As you could see in Input setup the remote works fine.

And sorry for sound and lightning, I was in my basement because my wife was sleeping.
```

---
## \#8 Posted by: r3vilo Posted at: 2018-11-03T11:07:26.951Z Reads: 36

```
**UPDATE!!!**

**PART 3 - BLDC mode sensorless**

https://www.youtube.com/watch?v=jHvcNFOILQ0

**BLDC with no sensors works!** :D 

Detection also fails. I get on the bottom right a "Bad Detection Result Received" and in the main window it says "Detection failed" (as before) but if I go on by pressing "next" it says setup is complete and I should go on with App Setup. No warning, nothing.

Looks like I can ride again, even if in BLDC mode with no sensors. Only thing I worry about is, that with going further by clicking "next" the default values of

Cycle Integrator Limit (62,00) and
BEMF Coupling (600,00)

will be applied. I don't know if this could have an negative effect or damaging even more. Obviously these values should be calculated in detection and because of failing I don't have the correct values here, right?

Can someone confirm that these two values don't do nothing what can cause damage to the motors or even the battery? Fire or something? Blocking wheels that I will fall off suddenly?

The help text says the following:

Cycle ingegrator limit. This is how much area will be integrated under the back EMF after a zero crossing before doing a commutation. A too low value will cause a too early commutation, and a too high value will cause a too late commutation. A too late commutation will cause more problems than too early commutations.

BEMF coupling. Roughly describes how much of the input voltage is seen on the BEMF at low modulation. Compensating for that at low speed helps the startup al lot.

Nontheless it seems my sensors have a problem or are damaged? If I try BLDC with Hall Sensors, detection fails as expected. When I skip here also with "next" and complete the setup, afterwards, when I press the throttle on remote it only beeps. Maybe because the sensor settings are Hall Table [0] -1, Table [1] 1, Table [2] 3, Table [3] 2, Table [4] 5, Table [5] 6, Table [6] 4 and Table [7] -1, becaue that's default and don't matching with my sensors/motors.

So for now I'm using BLDC sensorless. Seems to work.

Any tips for my problems? If my sensors are defective do I need new motors? Is it ok to ride in BLDC sensorless mode then? What are your suggestions to do now?

Thanks.

**UPDATE: Riding doesn't work** :( :( :frowning:

**Just wanted to ride but it doesn't move with wheight on it. It tries to but has not enough torque or power to do. If I lift it up it spins like in the last video. I think specific values still have to be edited.**
```

---
## \#9 Posted by: Sebike Posted at: 2018-11-03T14:44:40.333Z Reads: 34

```
If you haven't done it already... Check if sensor wires are connected properly. Unplug and plug in and check for visible wire damage all the way from motors to vesc. Recheck all wires going to /from vescs. Then try detecting hall sensors again.
```

---
## \#10 Posted by: r3vilo Posted at: 2018-11-08T07:29:52.109Z Reads: 32

```
Thanks. Sensor wires are connected. I already tried without (disconnected) and in sensorless mode. ... And I already checked all wires but I will do again.
```

---
## \#11 Posted by: taz Posted at: 2018-11-08T08:24:25.426Z Reads: 29

```
I did not watch the whole video but at 1:45 in your first video you input 60 cells to calculate the battery cutoff. This leads to 186V :open_mouth: cutoff.
Redo the procedure using 12 cells.
```

---
## \#12 Posted by: r3vilo Posted at: 2018-11-26T11:14:00.052Z Reads: 28

```
@taz You were right. Today, after weeks of no riding or working on the board I just edited the battery cutoff again. This time to 12 cells and afterwards, it worked again! Thank you so much! ... Not that I tried not before. I think I wrote it somewhere above or under the YT-videos but without success. I always try everything before I create a post somewhere or ask a question. ... I don't know why it did not work before.

It makes sense, when it should shutdown the system at a voltage of 186V and below and it's only getting 50V. But I'm 100% sure I also tried 12 cells in the setup. I tried it definitively after you posted this over 2 weeks ago. Nothing happend.

I switched wires again of everything, tried every Focbox with every motor in Single mode only and so on. I don't know why... it didn't work, I had the same behavior etc. etc.;

Now, 2-3 weeks later I just connected it again to my laptop, made a new setup with 12 cells battery cutoff and it passed every step in the setup. You couldn't image how happy I was when I saw the green fields after flux linkage measuring :smiley:
 
OK, I must admit I also changed  Battery Max. from 40/10 to 60/10. Don't know what this did. In Motor setup it speeded up much faster than usually. With more power if you want. Then detection succeeded.

OK, anyways. I'm fine now. Thank you for your help.

Because I don't have a Bluetooth module I had to dismount my enclosure all the time. I destroyed one hex screw (made it round on the inside). But hey, I learned a lot because of that issue :slight_smile: Bluetooth module will be the next purchase.

Thanks everyone.
(PS: Deleted the videos)
```

---
