# PPM Setup Problems With Hobbyking VESC And GT2B

### Replies: 8 Views: 333

## \#1 Posted by: Rutherford Posted at: 2018-06-28T00:20:46.140Z Reads: 79

```
Hi, 

I'm trying to set up a hobbyking VESC with a GT2B receiver. The motor setup was fine, but no data is coming through for the ppm setup. I have enabled live data but when I click apply it says failed applying pulse lengths. The receiver seems to be connecting to the tx because when I turn that off the signal light flashes. 

Has anyone else encountered this issue? 

Kind regards, 

R
```

---
## \#2 Posted by: abenny Posted at: 2018-06-28T17:13:12.030Z Reads: 49

```
Are you plugged into the correct channel? I believe it's 2 for acceleration and brake
```

---
## \#3 Posted by: Rutherford Posted at: 2018-06-28T17:28:32.668Z Reads: 46

```
The signal is on a Servo connector with the Vcc so I only have one option for channel. 
I tried a servo in channel 3 and it made a noise when I moved the wheel on the tx so it must be connected, but when I put it in channel 1 or 2 it doesn't respond to any control so I don't think those connect to the throttle.
```

---
## \#4 Posted by: Rutherford Posted at: 2018-06-28T17:37:04.811Z Reads: 43

```
I'm using the tool downloaded from the VESC project website if that helps
```

---
## \#5 Posted by: abenny Posted at: 2018-06-28T17:47:12.294Z Reads: 43

```
Hmm, not sure what would be wrong if it isn't working on channel 2 :confused:
```

---
## \#6 Posted by: Rutherford Posted at: 2018-06-28T18:39:57.643Z Reads: 39

```
I just remembered that Rx is common power rail so I'll try again later with the VESC on 2 instead of the servo :slight_smile:
```

---
## \#7 Posted by: Rutherford Posted at: 2018-06-28T23:38:06.564Z Reads: 35

```
That worked, thanks
```

---
## \#8 Posted by: abenny Posted at: 2018-06-29T03:26:03.227Z Reads: 32

```
glad it worked out for you
```

---
