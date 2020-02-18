# Dual Motor BLDC Configuration

### Replies: 7 Views: 1532

## \#1 Posted by: DreJ Posted at: 2017-06-12T17:51:12.658Z Reads: 133

```
Hi everyone. I've had some good answers from my previous post and [this](http://www.lp-electronic.com/vesc/connect-two-vesc-via-can-bus/) helped me a lot. Although I still need some help with configuring the Dual vescs.

* Firstly, in the tutorial I linked above, it states "Connect battery negative from each VESC together at one point". I don't really understand what this means. I don't have the circuit properly connected when configuring my vescs? I am connecting two batteries in series into an on/off switch which is what the XT90 dual vesc connector will plug into. How can I only connect the negatives to my vesc if it is an XT90 connector that plugs straight into another XT90 connector? Or can I just configure it in the normal circuit.


* I'm really having trouble about configuring both vescs in the BLDC tool. I was told that because I'm using two vescs, some parameters need to be halved? If so, which ones? I will basically tell you all I know and you can tell me if it's right or wrong, and if it's wrong, this is what I will do in order. 

1) Connect **master vesc** into the BLDC tool and **give it ID '0'.** **Put the 'App to use' at PPM**. I will NOT select 'Send status over CAN' but I will select **'Multiple ESCs over CAN'.**

2) Connect the **slave vesc** into the BLDC tool and **give it ID '1'**. **Put the App to use at 'No App'** and **tick 'send status over CAN'**

3) Connect the vescs with the CAN bus.

4) Connect the **master vesc** into the BLDC tool. Go to the PPM tab in App configuration and tick 'Display'. Pull the trigger on my receiver with control mode on 'disabled' and use the number to edit the maximum pulsewidth. Same with the minimum pulsewidth. Write configuration. Set control mode to 'Current no reverse with brake'.

5) In Motor configuration, motor tab, leave minimum and maximum input voltage at default. Set 'Battery Cutoff Start' to 35V, set 'Battery Cutoff End' to 33V.

6) Go to BLDC tab in motor configuration, press start detection. Change integrator limit to the nearest 5 and change BEMF coupling to nearest 50.

7) I do not know what to change Motor Max, Motor min (regen), Batt max, Batt min (regen) and Absolute max to. Can someone please help me?

That is everything I'd do once I know how to complete step 7. Is that all I need to do to completely configure both vescs? 



Batteries: Two 5000mAh 5S 40C LiPos connected in series.
Motors: Two 6355 190KV motors.


Sorry for the long post and thanks for all the help guys.h
```

---
## \#2 Posted by: Jinra Posted at: 2017-06-12T17:58:27.050Z Reads: 122

```
There's no need to create a new thread about this when you still have your old thread. Can you post there instead?

http://www.electric-skateboard.builders/t/help-with-dual-vescs/25172/7
```

---
## \#3 Posted by: DreJ Posted at: 2017-06-12T19:35:23.639Z Reads: 108

```
._. What I've written is completely different. I'd just like some clarification about if my steps are correct. I wasn't getting my answers on my previous thread so I thought I'd create a new one containing new questions as well and the steps that I'll take.

I'm sorry if that's not what I'm supposed to do but I don't think it's hurting anyone. Thanks for all your help so far man. I appreciate it. I can delete this thread if you really think its necessary.
```

---
## \#4 Posted by: t0m_r1dd1e Posted at: 2017-06-12T19:41:24.673Z Reads: 97

```
I'd ignore that first bullet point. I think it just means make sure both of your VESCs are commonly grounded. 

For your second bullet, your battery values need to be halved, so battery max and battery min. As far as I can remember, everything else should be fine.
```

---
## \#5 Posted by: DreJ Posted at: 2017-06-12T19:51:42.924Z Reads: 92

```
And how do I know what to set the parameters at that I addressed in no. 7?
Thanks
```

---
## \#6 Posted by: Jinra Posted at: 2017-06-12T19:59:41.657Z Reads: 87

```
I answered that one in the previous thread
```

---
## \#7 Posted by: t0m_r1dd1e Posted at: 2017-06-12T20:40:30.272Z Reads: 83

```
You did indeed.
```

---
