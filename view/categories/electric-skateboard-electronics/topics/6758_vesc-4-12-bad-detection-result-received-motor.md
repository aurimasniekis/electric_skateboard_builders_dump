# VESC 4.12 Bad detection result received (motor)

### Replies: 11 Views: 1890

## \#1 Posted by: Chewyone Posted at: 2016-07-28T11:50:36.871Z Reads: 197

```
No fault code appears, I'm lost as to how this may occur. I am using a TB 6355 motor and APS VESC. I will include a picture of top and bottom of vesc as well as settings, also a video of the motor itself spinning up during the test.
```

---
## \#2 Posted by: Chewyone Posted at: 2016-07-28T11:57:21.679Z Reads: 197

```


<img src="/uploads/db1493/original/2X/9/97cc9e9ab7e3afb9dbc46b59f4ad2e327689a4d2.jpg" width="690" height="388">
```

---
## \#3 Posted by: Chewyone Posted at: 2016-07-28T11:58:31.524Z Reads: 190

```
<img src="/uploads/db1493/original/2X/8/8feae6866fd3c1b17a9108c7a9341dc352eed215.jpg" width="690" height="388">
```

---
## \#4 Posted by: JTAG Posted at: 2016-07-28T12:45:35.438Z Reads: 186

```
Did it work before or does it fail after usage? The First thing I noticed are the 2 missing ceramic caps.
```

---
## \#5 Posted by: chaka Posted at: 2016-07-28T13:14:59.868Z Reads: 187

```
Some of the mosfets look like the pins are shorted. The leds are also placed incorrectly.  

The vesc is going to start getting a bad reputation again with all these poorly manufactured units hitting the market.
```

---
## \#6 Posted by: Chewyone Posted at: 2016-07-28T13:18:27.090Z Reads: 181

```
Well I can control the motor perfectly fine with my GT2B and it spins up and down fine with no errors, it's just the motor detection itself doesn't work which is confusing. I just pulled TB 6355 XML files for it and it worked fine.....
```

---
## \#7 Posted by: elkick Posted at: 2016-07-28T14:00:40.497Z Reads: 174

```
Could be, that Benjamin Vedder had something in mind when he was placing those caps on C37 and C51 (CAP 15u, 100V) on the VESC. Omitting it seems not the best idea, whoever did that should explain it to you.

Even so the motor spins without detection based on a xml file I would never drive it that way. And I agree with @chaka, this poor quality is not adding to a good reputation of the VESC!
```

---
## \#8 Posted by: Hummie Posted at: 2016-07-28T16:09:51.830Z Reads: 157

```
Could just be a small short in the motor.  Or the motor lead disconnected from one of the motor wires internally.   I did that and the motor will run but with less power and a bit louder but won't work on the test
```

---
## \#9 Posted by: Chewyone Posted at: 2016-07-28T17:24:19.128Z Reads: 143

```
I'm also getting ABS_over_CURRENT errors, does this add more pieces to the puzzle?
```

---
## \#10 Posted by: Chewyone Posted at: 2016-07-28T17:28:32.577Z Reads: 137

```
https://www.youtube.com/watch?v=ACZJlQV7_To
```

---
## \#11 Posted by: JTAG Posted at: 2016-07-28T21:59:54.355Z Reads: 121

```
Both the STM and DRV derive bias and reference voltages from their power supply rail, reference voltages are one of the fundamentals for analog to digital conversion. If you have garbage reference you get garbage measurements. Thus if the power supply is dirty by for example bad caps bad measurements could be the result. These omitted caps have a cost of about 3 euro's, there is of course a reason for this cost, they are hard to make. 

I think part of your problems might originate from bad component choices the manufacturer made in the construction. I say might because it could of course also  be something else. 

Be aware that the vesc is already build with minimal cost in mind, reducing the cost by omitting components could make your vesc emit smoke xD.
```

---
