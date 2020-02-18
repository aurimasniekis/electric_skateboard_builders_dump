# Help with Dual VESCs?

### Replies: 10 Views: 1840

## \#1 Posted by: DreJ Posted at: 2017-06-12T13:32:37.667Z Reads: 229

```
Hi guys. This is going to be my first build and it's going to be a dual motor build. I have everything set. I'll connect both VESCs together with this [Vesc Can bus Conncetor](diy-electric-skateboard-kits-parts/vesc-canbus-connector/). I'll then connect both vescs into this [Dual Vesc XT90 Connector](diy-electric-skateboard-kits-parts/dual-vesc-xt90-parallel-connector/) which will then go into my on/off switch and so forth.

My issue here is with configuring both VESCs. I've watched and read every tutorial I can find but I'm still not quite sure about the dual vescs. So here are my questions:

* 1) How do I select which VESC is master and which is slave. In the BLDC tool? Where is the option?

* 2) Should the master vesc be the one that is connected to my receiver by my [male to male servo connector](diy-electric-skateboard-kits-parts/male-male-servo-connector/)?

* 3) Does it matter which vesc is master and which is slave?

* 4) Which settings should I select in the BLDC tool to configure both vescs? Should "Send status over Can" be ticked on both vescs? Should "Multiple ESCs Over Can" be ticked on both vescs?

* 5) Should my settings in the BLDC tool be identical for both vescs?


If necessary, can you please tell me the steps I need to take to get both vescs running together and correctly? Thanks.





I think that's all. Please be specific and **slow** with your answers :blush: I'm still new.



Thanks for the help guys. Glad to be part of this community.
```

---
## \#2 Posted by: TarzanHBK Posted at: 2017-06-12T13:43:33.206Z Reads: 207

```
1 - http://www.lp-electronic.com/vesc/connect-two-vesc-via-can-bus/
2 - Yes everything like ppm and bluetooth should be connected to master
3 - no
4 - see 1
5 - all settings should be the same except the master/slave settings. You also have to run motor detection on every vesc for its own
```

---
## \#3 Posted by: Jinra Posted at: 2017-06-12T13:44:34.359Z Reads: 200

```
1. The master vesc should have "Multiple escs over can" checked while the slave should have "send status over can". The other should not have the option checked.

2. yes

3. no

4. see 1

5. Not required but i recommend it. Keep in mind some settings may have to be halved, such as battery regen, since you're running two vescs
```

---
## \#4 Posted by: DreJ Posted at: 2017-06-12T13:51:59.015Z Reads: 182

```
Thanks for the replies guys. This will help a lot. @Jinra is the 'Batt min (regen)' the only option that has to be halved. Also, now that we're on the topic, how do I know what to enter in the Motor Max, Motor min (regen), Batt Max and Batt min (regen). I can configure the rest, the voltage limits and the PPM but I'm not sure what to set those at. Any help?

Thanks guys.


I found this on a thread from over a year ago. Is it still correct? Should I follow these steps? : 

Connect master to BLDC, give the master ID 0, configure the PPM settings (write conf) for your receiver and test to see if your motor runs. Don't connect the slave to the master yet. Put your transmitter aside.
    Connect the slave to BLDC and give it ID 1 and tick " send status over CAN" - (write conf).
    Disconnect the slave from BLDC.
    Connect both VESC's with the CAN bus cable.
    Cycle the power on both VESC's off an on.
    Reconnect the master to BLDC and tick "CAN Fwd" on the upper right of your screen, enter ID 1 To receive data from slave.
    Goto the realtime data tab, tick "activate sampling" and verify there's data coming back from the slave. You should see the graphs move. If they don't, there's no communication.
    Now take your transmitter and pull the trigger to see if both motors spin.
```

---
## \#5 Posted by: DreJ Posted at: 2017-06-12T13:58:49.107Z Reads: 148

```
Thanks man. For that first link you sent, I'm assuming that I should configure each vesc first without connecting them by the CAN bus connector? Only once they are both configured do I connect them?

Also, do I configure them in the completely normal circuit just without them connected by CAN BUS? For example, both my vescs will be plugged into this [XT90 dual vesc parallel connector](diy-electric-skateboard-kits-parts/dual-vesc-xt90-parallel-connector/). This will then plug into my [on/off switch](diy-electric-skateboard-kits-parts/electric-skateboard-on-off-power-switch/). The switch will then be plugged into my [4m HXT series connector](diy-electric-skateboard-kits-parts/4mm-hxt-series-connector/) which is connected to both my batteries in series. 
Is this the correct circuit to set up my vesc? I don't understand what it means in the link you sent where it says "Connect battery negative from each VESC together at one point.".

Thanks for the help man.
```

---
## \#6 Posted by: Jinra Posted at: 2017-06-12T14:51:12.480Z Reads: 149

```
For motor limits, you'll need to play around with what works for you. For dual motor builds, this typically falls around 40-60a per vesc. For battery max it depends on what your battery can output. 18650 cells used in esk8 typically have 15-20a discharge per cell. For a 4p pack this equates to about 60-80a discharge on the pack, which should be halved for dual vescs for 30-40a per vesc.

Configure each motor without can or ppm signal then connect to test.
```

---
## \#7 Posted by: DreJ Posted at: 2017-06-12T15:28:51.830Z Reads: 134

```
I have two 5000mAh 5S 40C LiPo batteries. So what should I put my battery max at? 

Also how do I know what to set my Motor min (regen) at and my Batt min (regen) at.

Sorry about the questions, I'm still learning.

So when I first get my vesc I guess I'll just leave the motor max at somewhere between 40 and 60 and adjust accordingly. 

Thanks for the help. I appreciate it.
```

---
## \#8 Posted by: Jinra Posted at: 2017-06-12T15:39:59.734Z Reads: 135

```
With that much headroom you can leave the battery max at the same value as motor max.

The motor min is the braking current, inversely proportional to the motor max. I usually set it this to the same value as motor max, but with a negative value. The battery min is the regen current of the battery. You typically want 1c on this, which in your case is 5a (2.5a per vesc). I think lipos can handle more though.
```

---
## \#9 Posted by: Jc06505n Posted at: 2018-02-14T18:03:21.960Z Reads: 83

```
[quote="TarzanHBK, post:2, topic:25172"]
2 - Yes everything like ppm and bluetooth should be connected to master
[/quote]

Question: Does Bluetooth have to be on master, could it not work on slave?
```

---
## \#10 Posted by: bevilacqua Posted at: 2018-02-14T21:02:22.734Z Reads: 81

```
Witch Module are you using? I would recommend setting it up on the slave vesc if you are using the metr.at module. 

But theoretically it shouldnt matter witch VESC you use.
```

---
