# Vesc not powering any ppm receiver

### Replies: 5 Views: 821

## \#1 Posted by: Taow Posted at: 2016-10-01T13:59:13.116Z Reads: 89

```
I recently got a vesc and all was going well. I connected it to the computer and my motor, used bldc tool to detect the motor and calibrate the controller and everything that is shown on the YouTube tutorials. I was previously using a cheap trackstar esc so it didn't take long to upgrade to the vesc. 
I got everything working just fine and was really impressed with the vescs smooth acceleration and high startup torque. After about 20 mins of awesome cruising (I wasn't pushing the board very hard either) it suddenly cut out and was unresponsive completely! 
The ppm receiver used to have a little red light on showing it had power but that was gone so I assumed that the receiver was the problem as the vesc had all of its lights on and would still connect to the bldc tool. Also I charged the lipos back to full charge just incase it was some sort of voltage cutoff thing. 
When the new receiver didn't work either I tried changing the cable and I checked that there wasn't a loose connection with a multi metre. 
The only thing that I can think of is the the vesc itself is faulty or I have the wrong settings somehow on the computer (but as I said it was all working great and then suddenly stopped for no reason). 
I've tried measuring the voltage across the ppm pins and there doesn't seem to be any power going to them. Is there meant to be a voltage across any of the pins? I assume there is to power the receiver and that seems to be the problem for me. Anyone got any solutions? Thinking about just getting a kama nunchuck and trying to use that.
```

---
## \#2 Posted by: Jinra Posted at: 2016-10-01T14:06:50.771Z Reads: 80

```
You should be getting 5v from the middle pin. If you're not, then something's up with the VESC
```

---
## \#3 Posted by: Taow Posted at: 2016-10-01T14:40:11.496Z Reads: 72

```
Ah that's sucks, I'm getting like 0.3v. Do you think if I change to the kama nunchuck then it might work? The connector for the nunchuck gives me 3v on one of the pins so it should power a receiver right?
```

---
## \#4 Posted by: Jinra Posted at: 2016-10-01T16:06:32.245Z Reads: 68

```
I'm not sure, i thought most receivers require 5v
```

---
## \#5 Posted by: elkick Posted at: 2016-10-01T17:05:44.183Z Reads: 55

```
The Kama Nunchuk needs 3.3V only. So that should be working.
```

---
