# Recommended voltage for MayTech 50A Dual ESC

### Replies: 9 Views: 178

## \#1 Posted by: ZachTetra Posted at: 2019-01-15T04:10:24.055Z Reads: 44

```
I just purchased the MayTech 50A Dual ESC and 2 MayTech 6355 170kv and am about to purchase a battery.  How many lipo cells in series should I use?  The descriptions are rated up to 12s so I'd assume that that is the best but I don't know if these start to fail at 12s in which case I'll probably use 11s.

I'm flattening the lipo pack so configuration is irrelevant, if there are extras then I will keep the as backup if a cell goes bad.  Also the RPM doesn't matter because sprockets come in all sizes

Also, what fuse rating should I use?  The motors are rated for 65A max, but is that continuous or burst?
```

---
## \#2 Posted by: AdamE3399 Posted at: 2019-01-15T04:40:03.286Z Reads: 39

```
For 170kv, if you want the best speed and torque I would recommended pairing with 12s, which is also more efficient than 10s and will get your further. Also I have used 12s on 4.12 vescs and they seem to work fine for me as long as your batt max and motor max aren't too high.
```

---
## \#3 Posted by: ZachTetra Posted at: 2019-01-15T04:46:12.750Z Reads: 36

```
Do you mean the max voltage setting through the ESC?
```

---
## \#4 Posted by: AdamE3399 Posted at: 2019-01-15T04:47:43.642Z Reads: 36

```
I mean to make sure you set your batt max to 30 amps and motor max to 60, as some people go over this with 4.12 hardware and that's when things start to break, but I think it should be able to handle 12s no problem
```

---
## \#5 Posted by: ZachTetra Posted at: 2019-01-15T04:50:25.164Z Reads: 33

```
Why would the motors have a higher amp limit than the battery?  shouldn't it be something like 60 amps battery and 30 amps per motor?
```

---
## \#6 Posted by: AdamE3399 Posted at: 2019-01-15T05:03:46.584Z Reads: 31

```
No
10char 10char
```

---
## \#7 Posted by: ZachTetra Posted at: 2019-01-15T05:04:58.069Z Reads: 30

```
Why do the motors need a amp limit if its more than the battery?
```

---
## \#8 Posted by: AdamE3399 Posted at: 2019-01-15T05:05:51.865Z Reads: 30

```
Its for the vesc to make sure it isn't handling more current than the components can handle, it not a matter of what the battery or motor can handle, its what the vesc can handle
```

---
## \#9 Posted by: mynamesmatt Posted at: 2019-01-15T08:01:20.225Z Reads: 26

```
[quote="ZachTetra, post:7, topic:80926, full:true"]
Why do the motors need a amp limit if its more than the battery?
[/quote]

basically, what is comes out of the battery is related to the voltage coming from the battery. the esc's job is to change its output voltage to the motor according to load. essentially if a motor is ramping up speed, the esc is ramping up the output voltage. So the motor max (motor maximum current) is just the maximum current the motor can pull irrespective to the voltage. it's difficult to explain but that's the gist im 98% sure
```

---
