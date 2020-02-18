# Motor resistance when turned on / no throttle

### Replies: 12 Views: 201

## \#1 Posted by: Cloud_Gnash Posted at: 2018-07-26T01:14:03.884Z Reads: 71

```
I have a Raptor 1 and I just swapped out the tires to ABECS....when i went to ride it just now the board practically could not roll at all (without throttle) when the power is on, but the motor resistance disappears when i power it off. Has anyone encountered this problem before? I'm checking the setting on the VESCs and it all looks fine..
@EnertionSupport

https://photos.google.com/photo/AF1QipNXVKiMAQjLCxhjupVZ8BQKhC_IhnMn-LiqqF8d
```

---
## \#2 Posted by: Cloud_Gnash Posted at: 2018-07-26T03:17:55.331Z Reads: 60

```
OK I realized that I recently also installed a Nano-X onto my board...is there any set up i need to do besides just pairing the receiver?
```

---
## \#3 Posted by: mmaner Posted at: 2018-07-26T03:19:45.153Z Reads: 58

```
You need to do the PPM detection, the resistance is likely brakes because you have a different center than before.
```

---
## \#4 Posted by: Cloud_Gnash Posted at: 2018-07-26T03:29:12.405Z Reads: 55

```
I'm in the BLDC tool right now...can you explain how i do PPM detection? Is it the PPM setting in the 'App Configuration' tab?
```

---
## \#5 Posted by: mmaner Posted at: 2018-07-26T03:32:25.389Z Reads: 50

```
Yes, I do t have it in front of me, or I'd walk you through it. In bed though. 

It's the ppm detection with the live bar showing the ppm input.
```

---
## \#6 Posted by: Sender Posted at: 2018-07-26T03:39:47.855Z Reads: 48

```
Edit: what firmware are you using? This is for 3.x


Go to app tab, under general, set mode to off and write that (so the motors don't move during this process.)

Click on Real Time app data in the right hand side, it should light up green.

Go to ppm tab, go full throttle (motors wont spin due to step 1), that is the max, set that and apply.  Go full brake, set that and apply. Adjust the center as needed.  You will figure it out when you are looking at it.


Go back to app general tab and set back to whatever mode you are using, write. (Now your motors will move again)

I am not looking at it right now. But it is close to this. I am in bed... feeding 5 week old. Ugh.
```

---
## \#7 Posted by: Cloud_Gnash Posted at: 2018-07-26T03:45:21.101Z Reads: 45

```
Sorry, im using firmware 2.18. that may be the confusion. This is very helpful, Thanks!!!!! I will let you know how it goes
```

---
## \#8 Posted by: Sender Posted at: 2018-07-26T03:46:04.960Z Reads: 46

```
I should have guessed that... raptor 1. Its late, I am tired, hope you get it sorted!
```

---
## \#9 Posted by: SeanHacker Posted at: 2018-07-26T03:49:45.152Z Reads: 42

```
Just curious. But have you check the phase wires that lead into the motors? I've had this weird issue with all 4 R-Specs that I own. Just had to run some heatshrink in through the holes to separate them.

Still have a couple that I need to fix because of that issue. 
![IMG_20180714_172600|666x499](upload://eVngD2quXJEJlW0HDIIzEx4szJ6.jpg)
```

---
## \#10 Posted by: Cloud_Gnash Posted at: 2018-07-26T03:53:51.815Z Reads: 38

```
I havent checked the phase wires...I'm honestly not sure how to do that. Im still stuck on setting these remote settings.
```

---
## \#11 Posted by: cypa9904 Posted at: 2018-09-21T00:44:11.128Z Reads: 20

```
Hi. I have got similar problem with my e-mtb. Did you solve it in some way?
```

---
## \#12 Posted by: chrisongtj Posted at: 2018-09-21T01:54:08.035Z Reads: 17

```
I can't answer for the OP's particular scenario but the motors will have high resistance if the motor wires are shorted. However this happens even with the board off though, but worth checking always.
```

---
