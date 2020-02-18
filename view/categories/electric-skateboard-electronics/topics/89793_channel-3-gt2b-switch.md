# Channel 3 GT2b switch

### Replies: 4 Views: 158

## \#1 Posted by: butt_stallion Posted at: 2019-04-08T12:12:22.804Z Reads: 43

```
 I am trying to add a button to my remote so I can switch the lights on/off with a momentary switch. The remote I am using is a gt2b with a third channel already on it, but I removed the button and signal wire to make it fit into a 3-D printed controller. I need to know how to connect the switch so that it sends a signal through the third channel. I am attaching a picture of the switch I have and the controller internals. The battery runs directly into the positive and negative of channel 3 to power the whole board, I’m just not sure how to utilize the signal part of it.

![20190407_155513|374x500](upload://z2OhVJy0mYdEQ0vKLg7k3QlQIFX.jpeg) 

Thanks for the help!
```

---
## \#2 Posted by: murloc992 Posted at: 2019-04-08T12:18:54.105Z Reads: 32

```
Also be aware that the third channel is a latching input. Meaning that it retains the last value after the press until you press it again. I'd assume the button only shorts either signal with ground or signal with voltage. Could give you a picture and clarification when I come home. 

I might have some fun things in the future, including a 3D printable GT2B case that has 3 buttons, 1 is the original latching channel 3, 2 for channel 2 which are non latching and work as a (bottom button)1250-1500-1750(top button) thumb rocker switch. Planning to hook one output to a scooter horn and another to something else. :smiley:
```

---
## \#3 Posted by: butt_stallion Posted at: 2019-04-08T12:26:14.629Z Reads: 31

```
I am aware it is a latching input.  I'll be using it for an LED light system, so the button will be for on/off.  I actually wired it up real quick last night and shorted signal with ground and that didn't seem to work.  I can try shorting voltage to signal.  I would appreciate a picture.  

That sounds pretty cool!  It's nice to be able to use those channels on the gt2b for accessories.
```

---
## \#4 Posted by: Mich21050 Posted at: 2019-04-08T12:28:26.069Z Reads: 29

```
Maybe this will help: https://www.electric-skateboard.builders/t/pwm-controlled-brake-light-controller-open-source/85588?u=mich21050 \
Thats how I did it. :slight_smile:
```

---
