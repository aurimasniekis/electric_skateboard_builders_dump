# Litech BMS wiring diagram&hellip; I don&rsquo;t get it

### Replies: 7 Views: 158

## \#1 Posted by: piepolitb Posted at: 2019-10-11T20:38:43.559Z Reads: 44

```
Hi everybody
I just got the HCX-D596LI12S80A-02, you can see the specs [here](https://litechpower.com/product-detail/HCX-D596LI12S80A.html).

I need to connect it to my configuration with 2 6s battery pack in series, here is the connection diagram from litech website, but I don't really get it: I'm no expert....
![image|690x434](upload://57APi06iKIJHq6cS0Sy4LoX2HJZ.jpeg) 

In my understanding this is what I need to do
![image|690x386](upload://6v7V3YndZ1zaKEYLIlzLKcp7Cpt.jpeg) 

Can anyone please confirm or correct it ?
thanks
Giuseppe
```

---
## \#2 Posted by: Tinp123 Posted at: 2019-10-11T21:18:15.456Z Reads: 38

```
To me, it looks all good. Take look on my post on news forum, exactly same case like yours:

https://forum./t/connecting-bms-to-batteries/8715/6?u=tinp123
```

---
## \#3 Posted by: piepolitb Posted at: 2019-10-12T10:01:03.641Z Reads: 32

```
Thanks. Do you also think that charger and ESC connections are right ?

These two bother me a lot...
```

---
## \#4 Posted by: Tinp123 Posted at: 2019-10-12T10:07:49.892Z Reads: 28

```
Yes, looks good. I have drawn thick yellow lines where you should use thicker wires, like 12awg. Thickness of wires to charging port depends on charging current, but 18 or 20 awg should be enough.

![IMG_20191012_120343|690x386](upload://jPS4rfkmWWJpHHNhYfzSt64HRvd.jpeg)

Edit: also 12 awg between two 6s batteries, forgot to draw that
```

---
## \#5 Posted by: piepolitb Posted at: 2019-10-12T10:11:12.982Z Reads: 22

```
Ok,  makes sense

Max charging current is 3A, I don't think I need too much large wiring here. 
But it would be just a couple of cm more... Better safe than sorry :)
```

---
## \#6 Posted by: Tinp123 Posted at: 2019-10-12T10:15:24.375Z Reads: 21

```
For 3a you can use even 24 or 26 awg. It wont hurt if you use thicker wire than necessary
```

---
## \#7 Posted by: piepolitb Posted at: 2019-10-27T17:06:14.180Z Reads: 18

```
ok I finally had some spare to time to work on it.

I made all the connections right,  I didn't blow up but it is not working.

I tested connections with a multimeter, I bypassed the BMS switch connecting the two wires, but nothing: 
I got no power on the ESC and measured no Volts between + and - on the ESC or the charger port.

I also bypassed the BMS directly connecting batteries with the ESC, and I got power. So Is it the BMS ? 

what do I need to check ?
```

---
