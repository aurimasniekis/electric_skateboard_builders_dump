# SOLVED Board accelerates when signal is lost

### Replies: 8 Views: 1499

## \#1 Posted by: crameur Posted at: 2016-08-13T09:49:49.310Z Reads: 161

```
Hi,

I finished my build 2 days ago, and I love it ( 12s, 33inch kebbek board). I'm soon going to make a build thread but I have an issue, when I turn off the remote before the board, it accelerates, I am using a vesc in PPM mode and changing "brake current when signal loss occurs" doesn't do anything, can you guys help me ?
```

---
## \#2 Posted by: Iceni Posted at: 2016-08-13T10:18:46.179Z Reads: 161

```
If you are using a standard RC remote you'll probably need to set the failsafe on the reciever, I had the same behaviour on mine.
Look it up in the manual how to set it up, should be a fairly easy procedure.
```

---
## \#3 Posted by: crameur Posted at: 2016-08-13T10:21:18.561Z Reads: 160

```
I'm using a Nano remote, the same one that  @Kaly sells. I'll look up for instructions but if someone knows how to, help will be apreciated :)
```

---
## \#4 Posted by: Iceni Posted at: 2016-08-13T10:25:29.406Z Reads: 172

```
I'm not familiar with that one unfortunately.
Hopefully someone around here will have an idea.
```

---
## \#5 Posted by: crameur Posted at: 2016-08-13T10:27:49.670Z Reads: 167

```
Found the solution,

as @Kaly says : 
" Today i encountered 2 issues with the remote

First the remote comes already bind to the receiver, but in some instances the binding process need to be repeated, this is because of the fail safe feature of the receiver that needs to be calibrated. This manifest itself in this situation:

With the board On, if you turn Off the remote, the motors will start spinning without input. This is because the receiver needs to record the NEUTRAL position (mid throttle ) of the remote.

The Binding procedure is as follow:

1).Check and make sure all the wires are connected and that the REMOTE is OFF,insert the bind plug into CH3(Bind) on the RECEIVER.

2).With the REMOTE OFF. Switch on the ESC, to power up the RECEIVER, red LED light will flash.

3).PRESS and HOLD the bind button on the REMOTE and then turn the REMOTE ON.

4).You should notice the REMOTE and RECEIVER LED light go from flashing red to solid red.

5).Once you see a solid red light, the binding process is complete, Then without turning the REMOTE OFF or touching the THROTTLE pull the bind plug out (for the receiver to record the throttle mid point, neutral, to engage the fail safe)

6).Then you can test it again by turning OFF the REMOTE and the RECEIVER LED should flash. By turning the REMOTE ON the RECEIVER LED should go back to solid red.

Before RIDING ,it's better to test the fail safe function in the RECEIVER ,if the motor didn't move,so the fail safe function is in good working condition, if the motor is moving,you have to repeat the step No.1- No.6 above"
```

---
## \#6 Posted by: Skitzor Posted at: 2016-08-13T10:27:50.333Z Reads: 152

```
Have you set your PPM control values, so that it's nicely in the middle?
```

---
## \#7 Posted by: crameur Posted at: 2016-08-13T10:28:47.918Z Reads: 140

```
Yes I did that but the problem was coming from the receiver/remote not the vesc. thank you guys anyways
```

---
## \#8 Posted by: Kaly Posted at: 2016-08-13T12:02:23.805Z Reads: 121

```
For those using the VESC that are having some issues this can help, please follow it in stated order.

- Before connecting it to you board give it a full charge.

- Connect to VESC and configure receiver in BLDC tool.

- Once receiver is configure, take a small screw driver and trim the throttle on the remote to your preference.

- Repeat the binding procedure to ensure proper neutral position.

- Them One more time connect the VESC to the computer and configure the receiver limits again in the BLDC tool.

It seem that the min/max pulse width changes a little bit (in the remote) with the trimming of the throttle.
```

---
