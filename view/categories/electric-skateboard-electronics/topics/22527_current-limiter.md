# Current limiter

### Replies: 28 Views: 1695

## \#1 Posted by: NilsS Posted at: 2017-05-06T15:12:47.437Z Reads: 165

```
Hi, so i am basically building a 7S10P pack with a discharge of 56A. I am doing a super cheap build not using a Vesc. So I'm looking for a way to limit the current to 50A.

So I found this on eBay: http://www.ebay.com/itm/12V-24V-10-40V-50A-DC-Motor-Speed-pwm-Controller-Current-Limiting-regen-brake-/182310748346

Will this work as a 50a current limiter, and or are there any other options for limiting the Current?
```

---
## \#2 Posted by: Namasaki Posted at: 2017-05-06T15:48:42.326Z Reads: 152

```
The item description says that it is for brushed motors. 
Eskate uses brushless motors.
```

---
## \#3 Posted by: NilsS Posted at: 2017-05-06T15:57:43.972Z Reads: 145

```
Yes but as a simple limiter to the esc
```

---
## \#4 Posted by: Duffman Posted at: 2017-05-06T17:51:26.307Z Reads: 124

```
This is a brushed / DC motor ESC. You can only use it if you are planning to use a brushed / DC motor for your low cost build.
```

---
## \#5 Posted by: NilsS Posted at: 2017-05-06T18:26:45.929Z Reads: 107

```
You clearly don't know much about brushed motors.
```

---
## \#6 Posted by: Print3r Posted at: 2017-05-06T18:54:13.206Z Reads: 102

```
I know the difference between brushed and dc motors and cannot see how this board works, but seems like the specs are fine but brushed motors' speed is altered by changing voltage and current in a brushed motor is dependant on the load put on it (if you pinch the shaft of a brushed motor the amp draw will increase because short circuits). Hence, I could see you using this to alter voltage and thereby current (if resistance is constant) but not any other way. Please let me know how you were planning to use this board.
```

---
## \#7 Posted by: NilsS Posted at: 2017-05-06T19:17:48.498Z Reads: 100

```
This board spits out DC at a fixed max amperage, the pwm control will decrease the voltage. This is also how the current limiter works, it decreases the voltage when the limit is reached.
```

---
## \#8 Posted by: sl33py Posted at: 2017-05-06T19:21:57.865Z Reads: 97

```
[quote="NilsS, post:5, topic:22527, full:true"]
You clearly don't know much about brushed motors.
[/quote]


And *you* clearly don't need anyone to help you.

Being ungrateful to folks who are responding and trying to help - is a great way to get zero help. 

Seems like you know what you are doing - so do it.  Let us know how it goes.
```

---
## \#9 Posted by: NilsS Posted at: 2017-05-07T14:26:15.629Z Reads: 88

```
Sorry but I got frustrated, when you tried to explain something clearly wrong to me. I am sorry, if I acted in a way you found disrespectful.
```

---
## \#10 Posted by: saul Posted at: 2017-05-07T23:59:37.433Z Reads: 75

```
That might work. But probably not. 
Spend like $10 more and get BMS.

Don't understand why you'd try to repurpose anything else...
```

---
## \#11 Posted by: saul Posted at: 2017-05-08T00:01:22.054Z Reads: 75

```
Just realized it's 10p! And only 56a. Meaning they are probably recycled cells aka shit. Don't bother at all there have enough people wasting time on cells that won't survive and give enough current, especially for a non vesc build....
```

---
## \#12 Posted by: chuttney1 Posted at: 2017-05-08T03:01:18.835Z Reads: 72

```
Why do have the need to buy a current limiter if the VESC has a setting for putting a 50 amp current draw limit? I assume you understand that a device will draw the current it only needs to run based upon the total resistance of the circuit.
```

---
## \#13 Posted by: Rollbrett Posted at: 2017-05-08T05:22:42.824Z Reads: 67

```
He is on a budget and not using a vesc. He wants to use a DC Motor instead of a brushless one. 

It's not common but I don't see why it shouldn't work.

If it hasn't been done yet, take one fo the team and just give it a try! Other people will profit from your experience
```

---
## \#14 Posted by: chuttney1 Posted at: 2017-05-08T05:35:23.487Z Reads: 64

```
Miss read that one detail.
```

---
## \#15 Posted by: Nordle Posted at: 2017-05-08T05:51:26.737Z Reads: 63

```
1simple word:
**fuse~**
```

---
## \#16 Posted by: Rollbrett Posted at: 2017-05-08T06:22:48.636Z Reads: 54

```
A fuse is definitely not an bad idea but he does need something to regulate his speed/power as well. That's what the DC speed controller is for.

@NilsS what kind of cells are you using? Even with 10p, 50A might be to much for cheap cells.
```

---
## \#17 Posted by: NilsS Posted at: 2017-05-08T07:46:23.628Z Reads: 52

```
I  am using this board http://r.ebay.com/E9inxt.
i am using a 10S7P battery rated 56Amp. 
so i was looking for a way to limit the circuit to a maximum of 50amps.
but i dont want it to completely shut down when the limit is reached, like with a fuse.
the ideal thing was that it dropped the voltage enough for it to stay at 50amps.
so i found this circuit
```

---
## \#18 Posted by: NilsS Posted at: 2017-05-08T07:46:47.816Z Reads: 51

```
sorry 10P7S
```

---
## \#19 Posted by: NilsS Posted at: 2017-05-08T07:47:17.465Z Reads: 49

```
Dual 6354 motors
```

---
## \#20 Posted by: NilsS Posted at: 2017-05-08T07:56:29.387Z Reads: 49

```
another thing to note, is that in a pc these cells deliver a constant 5amp load without becoming hot.
```

---
## \#21 Posted by: Rollbrett Posted at: 2017-05-08T08:00:19.590Z Reads: 49

```
Ok my bad, I did totally misunderstood you.
```

---
## \#22 Posted by: NilsS Posted at: 2017-05-08T08:01:44.530Z Reads: 48

```
do you know something i could do to limit the current?
```

---
## \#23 Posted by: Rollbrett Posted at: 2017-05-08T08:46:25.269Z Reads: 49

```
You want to connect the current limiter between your battery and ESC. So you'll set the duty cycle of that device to a maximum and adjust the current limit to 50A. Is that correct?

Sounds like it could work but I'd rather try something different first:
Depending on the remote you're using you might be able to adjust your max duty cycle and that will also limit the current draw. Set it as low as possible and install a fuse (maybe 48A) between your battery and ESC. Make sure your battery is fully charged and go for a ride, if the fuse doesn't blow increase the max duty cycle a tiny little bit and go for another ride. repeat until the fuse eventually blows. 
Then swap the 48A fuse with a 50A one, it should not blow but is nice to have if you change the settings by accident.
```

---
## \#24 Posted by: NilsS Posted at: 2017-05-08T09:15:48.176Z Reads: 43

```
That was a great idea, only problem is that I don't think I can change the remote, ( I'm going to have a look inside when I come home). The only thing I can change is from beginner to advanced. But how much current do you think a 55kg person would draw?
```

---
## \#25 Posted by: smurf Posted at: 2017-05-08T09:19:51.210Z Reads: 41

```
http://1.bp.blogspot.com/-ba0UFvL02-o/TuOLJfzCTKI/AAAAAAAAALg/wgHS-2cajCg/s1600/IC+317+Power+Supply%252C+Simplest.png
```

---
## \#26 Posted by: NilsS Posted at: 2017-05-08T09:47:07.573Z Reads: 40

```
This circuit would work?
```

---
## \#27 Posted by: jmasta Posted at: 2017-05-08T18:03:15.153Z Reads: 34

```
So you want to spend $30 on hardware you don't need... to save money? Just put that money toward a VESC
```

---
## \#28 Posted by: dominic Posted at: 2017-05-08T20:36:16.276Z Reads: 27

```
When limiting amps comes to my mind, i think of snap action breakers. They are like fuses but they reset themselves after they cool off. They are calibrated to amperage by heat, so if you hit 50 amps it wont shut  off automatically, only after a couple seconds when it heats up. After it cools back down, it will go back to normal and complete the circuit. 

Not sure if it wold be good for esk8 cause it might shut off when you dont want it too.
```

---
