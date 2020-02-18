# Esk8.de FOC, any problems?

### Replies: 14 Views: 1069

## \#1 Posted by: fraannk Posted at: 2017-05-24T14:33:39.465Z Reads: 183

```
Hi, I've been riding with a VESC from esk8.de on my [iBoard Junior](https://www.electric-skateboard.builders/t/the-iboard-junior-mini-deck-sk3-6382-168kv-10s-lipo-vesc-83mm-wheels/18042/7) in BLDC mode for almost a year now, and it works great. But after researching about FOC and watching videos of the epic silence, I'm eager to try it out... Anyone had any problems with these VESC's? And any tips i should know before switching? 

Thanks
//fraannk
```

---
## \#2 Posted by: XIII Posted at: 2017-05-24T17:00:23.886Z Reads: 166

```
I have been using the FOC on esk8.de for over a year now. 
And it works great

I had 2 times a DRV ERROR's on the slave vesc. Every time I took a sharp corner. After disabling the traction control ( I run dual carvon V2) I have not run in any trouble. 
I think I rode 500km+ without killing a vesc
```

---
## \#3 Posted by: fraannk Posted at: 2017-05-24T17:41:30.654Z Reads: 157

```
Nice. Mine is a single drive, so the problem with traction control won't affect me. Thanks for the answer!
```

---
## \#4 Posted by: Bataleon Posted at: 2017-05-24T18:02:44.367Z Reads: 148

```
From what I've read, how successfully FOC works is very dependent on the motor you use. Hub motors seem to be ideal due to their lower kv rating (although I could be wrong on this one). I wouldn't risk FOC with a relatively high kv outrunner.

Has anybody here used FOC mode, over the long-term, with a high kv (>170) outrunner?
```

---
## \#5 Posted by: XIII Posted at: 2017-05-24T18:08:39.455Z Reads: 134

```
esk8.de ran his mountainboard brushless motors in FOC. Don't know the exact kv but could be 200. He gave garanty on the vesc running in foc with those motors
```

---
## \#6 Posted by: fraannk Posted at: 2017-05-24T18:14:20.581Z Reads: 128

```
I use a SK3 168kv, so the KV is not THAT high, might try it in the weekend, I'll wait for a little more answers :)
```

---
## \#7 Posted by: fuelre Posted at: 2017-05-25T11:46:01.216Z Reads: 107

```
Just do what esk8.de tells you how to setup the board and you are good to go!
```

---
## \#8 Posted by: Paulf Posted at: 2017-05-25T12:56:12.717Z Reads: 103

```
I do have enertion 4.12 Vesc but I have the exact same motor you have (on a vanguard too ;))  168kv Sk3 and I have been using foc without any issue for a few hundred kilometers 
My only advice would be : avoid spinning your motor on the bench without any load as much as you can, this is where the motors starts stuttering when it reaches high rpms without load 
I've now switched back to bldc (even though the foc silence is absolutely amazing) because I do like when people hear me coming and aren't surprised and also because of the little extra speed in bldc
```

---
## \#9 Posted by: fraannk Posted at: 2017-05-25T17:43:24.782Z Reads: 95

```
I've looked at their website, but I can't seem to find any FOC related tutorials. Was it the setup of the board in general you were talking about? Thanks
```

---
## \#10 Posted by: fuelre Posted at: 2017-05-26T05:50:43.921Z Reads: 84

```
write him an email, or give him a call
```

---
## \#11 Posted by: Maxid Posted at: 2017-05-26T05:58:29.921Z Reads: 82

```
Or - you know - just ask him here: @esk8
```

---
## \#12 Posted by: fuelre Posted at: 2017-05-26T05:59:36.269Z Reads: 85

```
yes thats also a good solution!
```

---
## \#13 Posted by: esk8 Posted at: 2017-05-26T17:07:39.038Z Reads: 73

```
Hi,
im testing our Vesc in al my Boards with FOC, and you have al time a litle
risiko to blow out your DRV.
That´s what if find out, was that FOC mode working very good by Hub motors.
You don´t hear in FOC mode the motor, also not at higher speed.
But by outrunner motors was the different not so high.
When you driving with higher speed you also hear the Motor.
There was not big different.
We have many E-Bike customers, there build the vesc in there Bike´s
and they drive al in FOC mode.
We don't hear any problems, not even at 12S, but there drive al under 80KV Motors.
Thats the problem, high KV Motors and 12S killing the DRV.
You can killing your DRV when you don't make the Vesc on and you push the Board.
Than can the Vesc loosing the motor detection and when you make the Vesc on
you drive without motor detection.
And we testing al Vesc in FOC mode only with Motors with Sensor.
Without we don't use the Vesc in FOC mode, there was the risk to big.
```

---
## \#14 Posted by: esk8 Posted at: 2017-05-26T17:27:02.126Z Reads: 67

```
I don't like the SK3 Motors,
i killing 3 Vesc with SK3 Motors.
I have self the Carvon setup and i driving the Board in FOC mode
but only with 8S.
Jerry have build my Carvon setup with 6364 SK3 Motors with 245KV,
the KV was to high for 10S so i using with 8S.
I think the way what going Dude was the better way, to using 
6374 motors.
I have here 4 PCS 6374 motors the same what using Dude
but with Hal Sensors and 90KV.
I thinking that was the best combination for his System.
Our 6374 motors have 13,5Nm by 170KV
```

---
