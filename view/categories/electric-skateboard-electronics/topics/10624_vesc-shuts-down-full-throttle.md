# VESC shuts down&hellip;full throttle

### Replies: 24 Views: 2531

## \#1 Posted by: ra.rend Posted at: 2016-10-04T16:48:33.304Z Reads: 266

```
Here's what happened: I quickly accelerate to about 10ish mph after a little push (basically full throttle after kick push), then my vesc  just cuts power few seconds into hill climb. I started from relatively flat ground, then hill grade increases gradually. If I don't accelerate too quickly, it can climb that hill at about 15mph without losing power or overheating. 

Here's a video showing the hill (this was recorded a while back). I start at the same spot shown in the video around 2:49, then power cuts off around 2:53
https://youtu.be/ZWeKIrteulk?t=2m49s
VESC cuts power around 0:11 shown below
https://youtu.be/tEt3twaNV0Y
My setup:
- r-spec 6355 190kv 
- space cell 3
- vesc 4.12 hw 2.18 fw
- 83mm wheel, 15/36 gearing

My VESC settings: 
FOC mode
Motor max: 60.00 A
Batt max: 40.00 A

Why does it do this?

EDIT: 
Fault            : FAULT_CODE_ABS_OVER_CURRENT
Current          : 214.7
Current filtered : 126.9
Voltage          : 31.71
Duty             : 0.59
RPM              : 33177.3
Tacho            : 163671
Cycles running   : 29347
TIM duty         : 4932
TIM val samp     : 5
TIM current samp : 8398
TIM top          : 8400
Comm step        : 0
Temperature      : 38.30
```

---
## \#2 Posted by: chinzw Posted at: 2016-10-04T16:54:10.752Z Reads: 245

```
Any recorded faults? When this happens you should keep the board powered on and connect it to a computer and check for faults.
Try with BLDC and check if the same happens, i bet it doesn't. I had my board shut down when braking and FOC.
```

---
## \#3 Posted by: ra.rend Posted at: 2016-10-04T17:09:17.984Z Reads: 243

```
Does the fault code go away if I power it down? I'll have to check for faults. 

It only happens when I accelerate really hard. It can climb that hill no problem as long as I don't go full throttle from start.
```

---
## \#4 Posted by: chinzw Posted at: 2016-10-04T17:15:24.032Z Reads: 232

```
If you power down you wont see the faults, they get cleared at boot time.
```

---
## \#5 Posted by: ra.rend Posted at: 2016-10-04T17:27:43.536Z Reads: 223

```
i got the fault code:

Fault            : FAULT_CODE_ABS_OVER_CURRENT
Current          : 214.7
Current filtered : 126.9
Voltage          : 31.71
Duty             : 0.59
RPM              : 33177.3
Tacho            : 163671
Cycles running   : 29347
TIM duty         : 4932
TIM val samp     : 5
TIM current samp : 8398
TIM top          : 8400
Comm step        : 0
Temperature      : 38.30
```

---
## \#6 Posted by: makevoid Posted at: 2016-10-04T17:33:42.566Z Reads: 212

```
Is your "max voltage in" value set to 57V? (Vesc config)
```

---
## \#7 Posted by: ra.rend Posted at: 2016-10-04T17:38:26.067Z Reads: 213

```
it's set to 43v.
```

---
## \#8 Posted by: makevoid Posted at: 2016-10-04T17:39:35.981Z Reads: 212

```
Put it to 57v, it will probably fix your issue

http://www.electric-skateboard.builders/t/battery-voltage-and-max-input-setting/7589/6?u=makevoid
```

---
## \#9 Posted by: ra.rend Posted at: 2016-10-04T17:40:53.815Z Reads: 207

```
Will I get the same fault code if I set to 42v and fully charge it?
```

---
## \#10 Posted by: makevoid Posted at: 2016-10-04T17:43:58.017Z Reads: 205

```
Anyway it seems a bit strange that a voltage spike could range 10V, it could be another problem but you may want to try this setting first

Other things to check, connections between battery and vesc and battery itself
```

---
## \#11 Posted by: ra.rend Posted at: 2016-10-04T17:46:29.566Z Reads: 201

```
I will try that. thanks
```

---
## \#12 Posted by: ra.rend Posted at: 2016-10-04T17:48:54.226Z Reads: 198

```
sorry, max input voltage is actually set to 57V.
<img src="/uploads/db1493/original/3X/0/3/03b1eb4d2e367cb8edca5d0c39adcbed6846e9e5.png" width="690" height="460">
```

---
## \#13 Posted by: makevoid Posted at: 2016-10-04T17:55:14.992Z Reads: 187

```
Then there may be an issue on the vesc, battery to vesc connection or battery itself, I would say it's probably the vesc but I don't know for sure.
```

---
## \#14 Posted by: Jinra Posted at: 2016-10-04T18:00:08.732Z Reads: 188

```
217a current is very high, sounds like a hardware issue
```

---
## \#15 Posted by: ra.rend Posted at: 2016-10-04T18:02:40.620Z Reads: 185

```
@Jinra There's a Bluetooth module connected to the VESC and a 5v fan connected to the receiver. Will that cause problems? I can accelerate hard on flat ground, but it only shuts down when quickly accelerating into that hill area.
```

---
## \#16 Posted by: treenutter Posted at: 2016-10-04T18:12:08.618Z Reads: 182

```
@ra.rend Are those the right battery cutoffs for your setup?
```

---
## \#17 Posted by: ra.rend Posted at: 2016-10-04T18:24:45.008Z Reads: 173

```
I'm not really sure. Is the battery cutoff end too low?
```

---
## \#18 Posted by: ra.rend Posted at: 2016-10-04T18:34:31.658Z Reads: 176

```
Is there like a problem with my setup? In other words, a short, loose connections, bad settings? Or is it just not capable of what I'm pushing it to do?
```

---
## \#19 Posted by: Blasto Posted at: 2016-10-04T18:37:16.411Z Reads: 175

```
you could try to up you max absolute current to 135-140A (this could blow stuff up), but i think you are asking to much for a single 6355
```

---
## \#20 Posted by: treenutter Posted at: 2016-10-04T18:40:26.730Z Reads: 174

```
@ra.rend The SPACE Cell is a 10s battery so I think your cutoffs should be Start:35 End:33

I don't think this is affecting the issuer directly but it's still good to correct.

 <img src="/uploads/db1493/original/3X/5/c/5c399cba287cef4ffa3c8bb2a695d53f6f00adcf.png" width="586" height="196">

(credit to @Jinra for posting this chart a long time ago)
```

---
## \#21 Posted by: DougM Posted at: 2018-06-19T04:53:55.799Z Reads: 92

```
So I had the same problem tonight - I was towing a friend back and we hit a hill, so I gave it full throttle and about halfway up the hill it cutoff completely.  I was using a dog lead as a tow rope, so he was very close and when it cut out he went down.  Minor scrapes and bruises.

Unfortunately I did not keep it on so I can't check the fault.

This is 10S5P on VESC6 running a single 6374-168 in FOC.
![image|690x438](upload://urMFZguItaE6w5ryCmRrVEH4ZNv.png)

Battery cutoff is 34/31

Please let me know if you see any suspect settings or if you want me to post more info.

Thanks,
```

---
## \#22 Posted by: ra.rend Posted at: 2018-06-19T05:38:03.302Z Reads: 85

```
I'm not sure about your settings, but your single-motor setup can't handle that much.
```

---
## \#23 Posted by: DougM Posted at: 2018-06-19T14:46:17.386Z Reads: 68

```
 I know - I wasn't expecting to actually make it to the top of the hill.  I've hit steep hills before not towing and it gracefully slowed to a stop with no drama.  

So I'm surprised that in this case it just shut down completely with no warning.  

It would be really nice if the VESC stored the last N error messages until you manually cleared them rather than clearing on power up.  

It looks from the VESC Tool interface that they've done a lot of work on making ABS Overcurrent errors shut down gracefully so I assume it's not that.  That just leaves low voltage in the pack, but you'd think I would have felt it roll back as it went below 34.

Which leaves an unexpected error.  I'm a little loath to try to repro the problem but it would be nice to know what caused it.
```

---
## \#24 Posted by: PeterdB Posted at: 2019-04-19T19:29:38.882Z Reads: 34

```
I![Vesc%20sensored%20setting|690x388](upload://xbkLpYJEyTyWl1jejxhcKWAF0vb.png)  have had the same problem, "beginner here" just finished my first board.
For me the solution was to activate the sensor mode for the motor, for some reasen it dit not wrote the original config down. Now its working properly...
```

---
