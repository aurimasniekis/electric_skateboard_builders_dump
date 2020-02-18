# \[Need help AF\] Drift-trike Vesctool ADC configuration

### Replies: 6 Views: 277

## \#1 Posted by: cathode Posted at: 2019-04-13T14:22:54.489Z Reads: 71

```
Hi.
So first things first, sorry for the incoming potato english.
Allright, i need you guys brain, I made a E-drift trike :  ![IMG_20190316_175454|675x499](upload://iI5cvZI2i6WGeM1bM2kLPSerllL.jpeg) ![IMG_20190316_174331|675x499](upload://5JhUW8hCXpP5XwHEGdQKN8fcQMF.jpeg) ![IMG_20190316_175434|675x499](upload://9r4BhskxYNIqov0pT8t4E3wvThr.jpeg) ![IMG_20190316_175402|675x499](upload://eGIqsBiGOrpDrmhu5MEBmTSO8LO.jpeg) 

And it's working nice and smooth but in order to unlock more possibilites i decided to switch the E-bike ESC for a focbox.
This is when things go bad...
I wired up all three phase, sensors and everything, motor detection and settings went well but i got issue(s?) with the thumb throttle i'm using :frowning: 

Because it's a thumb throttle i'm using ADC control mode mode. So i fellowed these instructions --> https://www.youtube.com/watch?v=KpeA6QRTZg8 But when i go to the mapping tab i see this : 
https://gfycat.com/ShallowOnlyHackee
No matter how hard i wiggle the throttle. 

Using a multimeter i checked all my voltages, I got my 0/+5V between the black/red wire and voltage variation between one of these two cables and the signal/ppm wire when i move the joystick. 

So looks everything's fine so why TF vesc tool's struggling to read a voltage !!!??

I allready asked esk8.fr on FB/Forum. Spent 2 full days trying to make it happend but now I'm really out of solutions so if you guys have some ideas, that's would be awesome :slight_smile:

Thanks for reading me
```

---
## \#2 Posted by: meesie Posted at: 2019-04-14T14:56:57.839Z Reads: 49

```
i suspect there is something wrong with your controller?
```

---
## \#3 Posted by: cathode Posted at: 2019-04-14T15:33:42.209Z Reads: 39

```
Hey @meesie thanks for helping me.
I spent the whole day continuing to  search and test stuff and possible solution.

On the UART port of my 'box and on some videos i noticed there is a ADC2 pin all the way to the top of the slot. So using the +3.3 / ground pins of the same port i plugged the signal wire to this pin.
AND IT WORKED !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
IT
WOR -
FUC***-
KED 
!!!!!!!!!!!!!!!!!!!!!!!!

*Insert Happy dance.gif here*

Calibration went fine, the throttle's working like a charm.
Wow you can't imagine how hard i tried to achive this.

Now my problem is some "ABS_over_current_fault_code"
I have to work on that....
```

---
## \#4 Posted by: meesie Posted at: 2019-04-14T17:10:12.217Z Reads: 32

```
When does it throw the fault code? When doing motor detection or when you throttle up?
```

---
## \#5 Posted by: cathode Posted at: 2019-04-14T17:52:08.908Z Reads: 30

```
Throttle up, even so slightly... weird.
```

---
## \#6 Posted by: cathode Posted at: 2019-04-15T18:42:52.721Z Reads: 16

```
Some tweaking later (raising up current absolut max) BOOM, a perfectly working drift trike !
```

---
