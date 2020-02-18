# Brakes failing at high speeds

### Replies: 16 Views: 1085

## \#1 Posted by: Strawbs Posted at: 2017-12-20T20:07:10.576Z Reads: 188

```
Hi all,  hoping to get some help with my brakes

Setup - Enertion dual motor kit with VESC and PRO4 battery pack

My problem comes when I am braking at high speeds.  The breaks completely shut off for about 2-3 seconds and the board wont respond to any input.  Braking at low speeds seems to be fine.

I'm wondering if this can be a simple fix in my VESC settings?  brake limit cut-off or something?

Any help would be appreciated.  Thanks!
```

---
## \#2 Posted by: Battosaii Posted at: 2017-12-20T20:39:42.967Z Reads: 173

```
What's high speeds? 25mph 35Mph?
```

---
## \#3 Posted by: krloz Posted at: 2017-12-20T21:29:18.227Z Reads: 161

```
does the vesc reset when this occurs?
```

---
## \#4 Posted by: onepunchboard Posted at: 2017-12-20T22:01:52.895Z Reads: 148

```
prob too much stress on vesc.
1. u can increase abs current 
2. increase regen current
3. increase gear ratio
4. make sure vesc is cool with air flow
5. get lower kv motor
```

---
## \#5 Posted by: Namasaki Posted at: 2017-12-20T22:41:37.657Z Reads: 130

```
Post screen shots of your Vesc settings so we can have a look.
```

---
## \#6 Posted by: Achmed20 Posted at: 2017-12-20T23:02:18.119Z Reads: 122

```
if you run it in FOC, disable that. doesnt run well on all VESCs out there.
mine fails especialy with breaking.
```

---
## \#7 Posted by: dg798 Posted at: 2017-12-20T23:06:53.761Z Reads: 116

```
Make sure you don’t limit your erpm with negative torque.
```

---
## \#8 Posted by: Strawbs Posted at: 2018-01-22T02:36:51.921Z Reads: 75

```
Here are my VESC settings.  Seems pretty standard from what i've been searching.

Does anything on here jump out?

![image|690x445](upload://9HUgOX33FJtdKibMnv2128QxBNA.png)
```

---
## \#9 Posted by: Martinsp Posted at: 2018-01-22T02:40:15.924Z Reads: 70

```
The problem is you changed the maximum input voltage, put it back to 57V and your brakes will work all the time.
```

---
## \#10 Posted by: Strawbs Posted at: 2018-01-22T02:40:26.571Z Reads: 69

```
I don't think its the VESCs overheating.  It happens immediately when starting the board cold.  For example... (Turn on board, run motors, hit breaks... the breaks cut out even when not standing on the board)
```

---
## \#11 Posted by: Strawbs Posted at: 2018-01-22T02:41:20.988Z Reads: 69

```
Thanks, I'll try this
```

---
## \#12 Posted by: Martinsp Posted at: 2018-01-22T02:42:30.309Z Reads: 69

```
Further explanation is that when you brake there is a voltage spike due to the motor generating power when braking, this triggers the VESCs protection and forces it to reset that explains the 2-3 seconds which the VESC does not respond to any input because it is going through a power cycle. After it boots up it works until you brake again.

EDIT: this does not happen at low speeds mostly due to the voltage not crossing the threshold for the VESC to reboot.
```

---
## \#13 Posted by: Strawbs Posted at: 2018-01-22T02:43:40.728Z Reads: 68

```
That's it exactly.  Simple fix.  It looks like I'm up and running again.

Thanks friend!
```

---
## \#14 Posted by: Martinsp Posted at: 2018-01-22T02:44:11.552Z Reads: 67

```
No worries.
```

---
## \#15 Posted by: scepterr Posted at: 2018-01-22T03:42:48.278Z Reads: 61

```
Hey I was setting up a couple vescs the other day....and I was thinking; is there ever a reason to change max input voltage? I couldn't think of one.
```

---
## \#16 Posted by: Martinsp Posted at: 2018-01-22T08:16:33.301Z Reads: 47

```
I dont think there is, at least for esk8 applications. Maybe it is there so that if someone wants to push the limits they can increase it or something. 

I have never encountered a situation where I had to change it
```

---
