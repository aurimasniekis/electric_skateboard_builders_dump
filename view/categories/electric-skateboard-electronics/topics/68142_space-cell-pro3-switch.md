# Space Cell Pro3 Switch

### Replies: 13 Views: 273

## \#1 Posted by: Esrapp21 Posted at: 2018-09-15T20:50:38.973Z Reads: 96

```
I have a space cell pro 3 on my board. I hadn't ridden the board in almost a year, and decided to get back on. I pulled it out of the closet to find the rocker switch had broken. I opened it up to see the wiring and realized it was a 2 prong switch, not 3. I’m wondering whether I should replace it with another two prong or a three prong switch. I don’t know how I would wire a three prong with the BMS though. It would be great if I could get some specific suggestions too. Thanks
```

---
## \#2 Posted by: mmaner Posted at: 2018-09-15T20:52:03.632Z Reads: 90

```
Get a 2 pin switch from any auto parts store and your good to go.
```

---
## \#3 Posted by: Esrapp21 Posted at: 2018-09-15T20:55:44.119Z Reads: 84

```
Ok thats what I thought, didnt know if not having a ground was a hazard.
```

---
## \#4 Posted by: mmaner Posted at: 2018-09-15T20:59:42.348Z Reads: 82

```
The switch connects to the BMS, it simply completes a circuit that tells the BMS to release power. The switch doesn't actually have any power running through it.
```

---
## \#5 Posted by: Jake2k17 Posted at: 2018-09-16T05:26:36.174Z Reads: 52

```
@mmaner
This is somewhat off topic but is there any way to connect a LED switch to the bms e switch?
```

---
## \#6 Posted by: Trdolan03 Posted at: 2018-09-16T07:00:32.431Z Reads: 47

```
@Jake2k17  I have tried this without success
```

---
## \#7 Posted by: Acido Posted at: 2018-09-16T07:43:11.882Z Reads: 41

```
If you want the lights it a bit more complicated because they are on much lower voltage

Switches just close the circuit, just find a diagram for your switch and solder on the 2 wires to the correct terminals
```

---
## \#8 Posted by: mmaner Posted at: 2018-09-16T12:51:35.212Z Reads: 35

```
This is how I've done it in the past. 

![latching%20switch%20-%20how%20to%20wire%20v3%20022718|690x433](upload://zzcMWwwzNcfaQ1PC4ZLLhDp4wMH.jpg)
```

---
## \#9 Posted by: mmaner Posted at: 2018-09-16T15:05:47.334Z Reads: 22

```
There is also this one where the positive and negative from the switch connect to the positive and negative of the spare vesc ppm header. 

![latching%20switch%20-%20how%20to%20wire%20v2%20110617|603x500](upload://duBulb9kdkEJ5QDAIrcGJSvQRe5.JPG)
```

---
## \#10 Posted by: Jake2k17 Posted at: 2018-09-16T15:41:09.511Z Reads: 13

```
Sorry on the second one I don’t understand...the positive and negative go to the power leads?
```

---
## \#11 Posted by: mmaner Posted at: 2018-09-16T15:43:06.328Z Reads: 15

```
You can use the POS & NEG from the PPM header in the slave VESC to power the LED. Essentially when you push the switch it powers in the BMS with supplies power to the VESC which supplies power to the LED.
```

---
## \#12 Posted by: Jake2k17 Posted at: 2018-09-16T15:45:09.859Z Reads: 13

```
Ok that makes more sense :slight_smile:
Thanks so much!
```

---
## \#13 Posted by: J0ker3366 Posted at: 2018-09-16T15:48:46.083Z Reads: 13

```
NC= normally Closed, which means its a closed circuit, which means always on till you it switch. NO= Normally Open, which means it an open circuit, which means always off to you hit switch. Hope that helps
```

---
