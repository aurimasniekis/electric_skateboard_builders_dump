# Using can bus to update firmware dual Vesc

### Replies: 16 Views: 1155

## \#1 Posted by: Jyrofpv1 Posted at: 2018-03-14T12:59:10.353Z Reads: 140

```
Cant find any direct info on this After alot of searching. It looks possible but can't figure out the exact process through the bldc tool. My Vesc's are sealed up, setup and everything is currently using bldc mode. First I'm going to set up Foc mode when i learn how to select the Vesc's independently . I think the process will  be similar in terms of controling the vesc through can bus. It looks like I uncheck multiple esc's over can bus then use can fwd to select the Vesc's independently.

Any Help would be much appreciated
```

---
## \#2 Posted by: Exiledd_Top Posted at: 2018-03-14T16:17:22.832Z Reads: 138

```
First what vesc are you, post a picture u said sealed up you sure its not a ESC most vesc have a micro USB port or old USB port and trying to run foc you have to be carefull because not a lot of vesc can run foc without frying   
What motors you using ,battery ,vesc
```

---
## \#3 Posted by: Deckoz Posted at: 2018-03-14T16:31:47.152Z Reads: 136

```
I'm gonna write instructions for VESC tool... Which is the same as bldc but without wireless

Setup Master a CAN 0 slave as Can 1

Connect to vesc vis usb or tcp bridge(I used wireless TCP bridge over uart)

Enable can FWD 1. Flash the slave with a default config that has "send status over can" enabled. After it's flashed you cannot connect to the slave because it is now CAN 0 default, which is also what the master is. Disable can FWD and set the master to ID 1. Renable CAN FWD 0 and you are connected to the slave. Set CAN ID back to one and save.

Disable can fwd. Update the firmware on the master, reenable multiple vesc over can and set the master to ID 0.

You've now updated firmware over can without having to unbolt the enclosure.
```

---
## \#4 Posted by: DeathCookies Posted at: 2018-03-14T16:40:16.097Z Reads: 120

```
Is it really possible? 

I had the following Problem and i think that the can Connection is the Problem (vesc6):
Two vescs connected by can. Only one is connected to the battery. Update Firmware on the connected one. After uploading it tries to restart the vesc. after restarting it does not have the new Firmware just the old one...

The Problem is that you power the second vesc through the can. Thus the second vesc blocks the first one from restarting for a correct Flash and sticks to the old firmware. I could be wrong... but that were my experiences
```

---
## \#5 Posted by: Deckoz Posted at: 2018-03-14T16:42:57.931Z Reads: 114

```
I've never had issues doing it... Vescs can restart independently just fine with a firmware flash or config change(setting app ie ppm & uart) that requires reboot.
```

---
## \#6 Posted by: DeathCookies Posted at: 2018-03-14T16:59:07.643Z Reads: 112

```
[quote="Deckoz, post:5, topic:49084, full:false"]
Vescs can restart independently just fine with a firmware flash
[/quote]

Even if the two vescs6 are connected by can? Did you test that?
```

---
## \#7 Posted by: Deckoz Posted at: 2018-03-14T17:00:21.377Z Reads: 107

```
I don't have two vesc6 from trampa

But I've done it on the following with canbus plugged in and both escs powered  on... Can shouldnt be connected if only one esc is powered
4.12
FOCbox
Stewii ESCape(6.4 vesc with custom BOM)
```

---
## \#8 Posted by: Jyrofpv1 Posted at: 2018-03-14T17:25:14.152Z Reads: 100

```
Thanks Deckoz thats exactly what I was looking for.

Just to understand it better for example doing motor detection. 

Can Fwd box unchecked would be on master and can Fwd box checked with a 1 would connect to the slave vesc assuming master is id-0 and slave is id-1 correct
```

---
## \#9 Posted by: Ixf Posted at: 2018-03-14T17:34:43.801Z Reads: 93

```
I just recently done this on my board.
The only slightly tricky part is when you flash your FW.  ID will revert to 0 (default setting).  You'd just want to make sure you don't get in that state where you have multiple 0s, otherwise out comes the can opener and off comes the enclosure

Starting State (Master ID=0 Slave ID=1)
Set Master ID to 2 (Master ID=2 Slave ID =1)
Can forward to ID1 (Master ID=2 Slave ID =1)
Flash Slave (Master ID=2 Slave ID =0)
Set ID to 1 (Master ID=2 Slave ID =1)
Turn off can forward to connect back to master (Master ID=2 Slave ID =1)
Flash Master (Master ID=0 Slave ID=1)
You are done, motor detect\setting as needed.
```

---
## \#10 Posted by: Deckoz Posted at: 2018-03-14T17:42:47.919Z Reads: 87

```
That's correct.


And @Ixf nice clean layout...mine was messy lol..
```

---
## \#11 Posted by: Jyrofpv1 Posted at: 2018-03-14T17:46:41.644Z Reads: 82

```
Yes very helpful thanks. Do i use cam fwd I'd for  Independent Motor detection?
```

---
## \#12 Posted by: Deckoz Posted at: 2018-03-14T18:00:10.431Z Reads: 82

```
Yes exactly as you stated if 

Master is 0 and slave is 1 and your USB or Bluetooth is plugged into master

Connect, can fwd disabled on connection tab, your on master, run motor detection

Connect, can fwd 1 enabled on connection tab. Your in slave, run motor detection.


Remember APP and motor config are Read and Saved separately. And you must READ the configs when changing can fwd so you don't accidentally overwrite the each with the other escs data.
```

---
## \#13 Posted by: banjaxxed Posted at: 2018-03-14T18:17:34.028Z Reads: 80

```
Good one ☝️ [quote="Ixf, post:9, topic:49084"]
out comes the can opener
[/quote]
```

---
## \#14 Posted by: Jyrofpv1 Posted at: 2018-03-14T18:25:09.970Z Reads: 76

```
Good stuff thanks
I'm trying to understand controller ID compared to Can fwd

Controller I'd for master slave settings and setup
Can fwd for sending commands to slave VESC

Is this correct
```

---
## \#15 Posted by: Deckoz Posted at: 2018-03-14T18:31:10.923Z Reads: 67

```
Controller ID is the CanBuS ID.

controller ID is set inside of the App configuration General tab.

Send status over can(for slave) is also on that page

Master use multiple esc over can is set on the app configuration -> control type tab (ie ppm or nunchuckcontrol ext)


CanFWD is on the main connection tab next to firmware tab
It's to tell the tool which canbus ID to connect to when can forward is enabled. So you can change the settings.

Make sense?
```

---
## \#16 Posted by: Jyrofpv1 Posted at: 2018-03-14T22:46:53.677Z Reads: 61

```
Makes sense thanks, i like to have a better understanding before  making adjustments to minimize casualties.
```

---
