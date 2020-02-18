# VESC settings for 12S 6374 170kv motor

### Replies: 6 Views: 2078

## \#1 Posted by: Tonto2k Posted at: 2017-01-02T10:47:52.091Z Reads: 262

```
Hi could you guys have a look at my vesc settings please?
I have been following guides from this site but just wanted to be sure?

My board is up and running I just want to know what people think/give advice about my settings?

I don't know what my Int Limit ERPM should be? Do I just leave it as is?
What should "Max ERPM" be set to?

I am running ackmaniacs Extended BLDC-TOOL with Watt Control Mode firmware with watt control mode.

<img src="/uploads/db1493/original/3X/d/9/d9de3b01d6729861375871cc02a5e29daddb3697.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/0/3/03ee5f97ecbe832afeeb5cfbc31a8ef41bac8cac.JPG" width="666" height="500">
```

---
## \#2 Posted by: Ackmaniac Posted at: 2017-01-02T23:07:54.259Z Reads: 219

```
If you have a LiPo battery you should set the cutoff start to 3.6V a cell (43.2) and the cutoff end to 3.4V a cell (40.8V).
If you have a Li-Ion battery you should set the cutoff start to 3.0V a cell (36V) and the cutoff end to 2.8V a cell (33.6V).
With these values ou would be on the safe side and don't stress the cells when they are close do completely discharged.
IF you have a single vesc you should set the battery max amps to not more then 50A at the beginning. And if you have 2 Vescs then don't go higher then 40A for battery max at the beginning. 
max ERPM of 60000 is perfect. You won't reach those ERPM speeds when riding. Only on the bench with no load it would be possible.
And you should set the integrator limit to 105 accourding to your motor detection. Or simply run the motor dectection and press the apply button afterwards and then write the settings.
When you drive in watt mode then you should set the max watts to 3.6V * 12S * battery max = max watts
e.g for 40A battery max
3.6V * 12S * 40A = 1728 watts
```

---
## \#3 Posted by: PXSS Posted at: 2017-01-02T23:36:46.096Z Reads: 205

```
Agree with all but the very last bit. Max power should be at 4.2V as that is fully charged.
```

---
## \#4 Posted by: Ackmaniac Posted at: 2017-01-02T23:39:43.825Z Reads: 196

```
Of course not 4.2V because there is a voltage sag :grin:
I just want that for most of the ride the remote is usable for all the throttle range. And to explain that it gets too far here. So I simply recommend this calculation and you will be fine.
```

---
## \#5 Posted by: Tonto2k Posted at: 2017-01-03T12:01:44.498Z Reads: 176

```
Thanks for the replies guys I have applied them settings :slight_smile:
```

---
## \#6 Posted by: sukurity Posted at: 2017-06-02T21:25:31.121Z Reads: 146

```
Hey man!

I'm currently building a esk8 with pretty much the same specs as your as was just wondering how these setting are doing for you?
```

---
