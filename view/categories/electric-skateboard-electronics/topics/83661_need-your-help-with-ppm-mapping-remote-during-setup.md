# Need Your Help with PPM Mapping Remote during Setup

### Replies: 7 Views: 444

## \#1 Posted by: silverfox56 Posted at: 2019-02-09T00:58:04.772Z Reads: 98

```
System:

Batteries: Ownboard 2P10S XT-60 42V full charge

Motors: Torque 6355

Switch: XT-90 Loop

Input: RC Car Pistol Grip Transmitter and Receiver

My eBoard worked until one of the two diyelectricskateboard ESCs shorted out. I had set up the board using vesc-tool and had no problems.

Now I'm using a flipsky Dual FSESC4.20

Plugged everything in and noticed the remote worked to spin the motors before running the vesc-project tool. Very promising!

Ran the entire motor wizard without a problem. I can spin the motors, brake, etc. while connected using the computer inputs. I did set it up as BLDC not FOC.

Ran the input wizard using ppm remote. Nothing but the Messages: "Applying Pulselengths Failed" & "Please activate RT app data and measure Pulselengths first". I see no signal from the remote on vesc-tool.

So the remote worked before I tried the input wizard but not after.

Same remote as on my previous setup.  In fact everything is the same except the dual ESCs. Remote is definitely paired to the receiver. I've tried other channels besides channel two, which worked before. Nothing.

To be honest, I bought an oversized Dual FSESC6.6 and hooked it up and had the same problem! I thought the remote input to that dual ESCs was faulty. So I bought the better sized Dual FSESC4.20.

Now I realize I've done something wrong! I don't know what.

ANY SUGGESTIONS WOULD BE MOST APPRECIATED!

Cheers
```

---
## \#2 Posted by: Andy87 Posted at: 2019-02-09T03:04:03.942Z Reads: 73

```
Is the ppm cable plug in the receiver in the right order?
Red 5V, Black ground, white signal?
```

---
## \#3 Posted by: nuttyjeff Posted at: 2019-02-09T03:08:59.788Z Reads: 72

```
Check if you are setting PPM from the master VESC. On the FESC6.6, the ppm cable comes out from one side, make sure you program PPM from that side.
```

---
## \#4 Posted by: ShutterShock Posted at: 2019-02-09T05:06:35.521Z Reads: 64

```
IDK bro I had this problem with my flipsky 4.12's on a client build too...

Couldn't figure it out for the life of me why it wouldn't work.  I then decided to roll back to the firmware that was delivered with the VescTool 0.87 and it worked fine there.. Who knows man.

Gt2b on 10s
```

---
## \#5 Posted by: silverfox56 Posted at: 2019-02-12T01:51:29.032Z Reads: 49

```
You are my new best friend! Thank you very very much. Cheers, 
Silverfox56
```

---
## \#6 Posted by: Esk8Addict Posted at: 2019-08-31T00:07:42.436Z Reads: 23

```
Did anyone find a solution to this problem?  I bought 4 Flipsky VESC's, 2 - 4.2 and 2 -6.6's and I am unable to map the controllers I use with them with the VESC Tool Input Wizard.  I have never had much of a  problem with other VESC's I have used.  Any help is much appreciated.  Trying to figure out why I can't map my controllers on the Flipsky VESC's is becoming very time consuming!
Many thanks in advance!
```

---
## \#7 Posted by: silverfox56 Posted at: 2019-08-31T18:18:09.386Z Reads: 17

```
Check if you are setting PPM from the master VESC. On the FESC 4.20, the ppm cable comes out from one side, make sure you program PPM from that side. I had this problem too. The above solved it. Good luck
```

---
