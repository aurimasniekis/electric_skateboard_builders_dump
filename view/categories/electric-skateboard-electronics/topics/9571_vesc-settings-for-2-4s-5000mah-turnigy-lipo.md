# VESC Settings for 2 4s 5000mah Turnigy Lipo

### Replies: 15 Views: 1545

## \#1 Posted by: jct1212 Posted at: 2016-09-14T05:12:29.110Z Reads: 150

```
Hi, I'm just setting up my VESC in the BLDC tool and just wanted to double check if these values should be ok, since I really don't know what I'm doing! I'm using 2 4s 5000mah Turnigy 20C Lipo batteries in series. I'm especially unsure about motor max and min, and min and max input voltage! Here are my settings:

<img src="/uploads/db1493/original/3X/d/8/d8cac0e8b2a45c79d1a9cef1cf0ce9d25fc9a1a5.png" width="690" height="397">
```

---
## \#2 Posted by: paul775 Posted at: 2016-09-14T05:35:13.325Z Reads: 143

```
Your motor max and batt max should be equal. 40 A works but myself and many others have both at 60 A.

Batt min regen is good. 

Motor min regen can be adjusted by how much braking force you need. So leave it at -40 for now and change it after your first ride if you need less braking force. I personally (single motor setup) only use brakes to slow down since full on braking might rip my belt. So I leave it at -30 A.
```

---
## \#3 Posted by: Jinra Posted at: 2016-09-14T05:38:56.517Z Reads: 140

```
There's generally more current in the motor then what is being supplied by the battery so i have mine about 20a higher than battery.
```

---
## \#4 Posted by: chinzw Posted at: 2016-09-14T05:41:27.156Z Reads: 141

```
[quote="paul775, post:2, topic:9571, full:true"]
Your motor max and batt max should be equal.
[/quote]

This isn't right.
Bat Max should be whatever your battery manufacturer states. For example 5AH lipo with 20C rating, can go to 100A.
Motor Max should also be what's stated by the manufacturer. For example 6364 SK3 192kv has a rating of 80A.

Always having in mind the limits of the VESC. And personal preference, for example, i prefer 40A max on my motor and 20A on my battery. This limits the power and works for me.
```

---
## \#5 Posted by: susplus Posted at: 2016-09-14T07:38:50.036Z Reads: 125

```
ok.

- Voltage limits are set for a 10s there and you need to change settings for a 8s battery. this means:
  - max imput voltage: 4.2v x8s =33.6V
  - Battery cutoff start=3.5v x 8s = 28V
  - Battery cutoff end= 3.4 x 8s= 27.2V

that's it. 

these are my settings also ;)

Also be sure to visit: http://vesc.net.au/
take a look at the 6 small vids on how to setup your VESC and you should be good to go ;)
I agree with chinzw on the motor max and battery max settings. Mine are a bit higher but not by much. and it works just fine.
```

---
## \#6 Posted by: Jinra Posted at: 2016-09-14T08:05:59.592Z Reads: 122

```
setting max input voltage is bad practice and can lead to your board cutting off. No need to change the max input voltage from the default 57v
```

---
## \#7 Posted by: susplus Posted at: 2016-09-14T08:47:19.963Z Reads: 115

```
after 60+ km of testing i have had no cut outs yet. I have followed the instructions given on the Vesc site since i am using the enertion one.
Why would it be bad practice and in the same time advised on the Vesc site? ( i am just trying to understand where the problem is so that i can mend what ever i did wrong )
```

---
## \#8 Posted by: Jinra Posted at: 2016-09-14T09:03:20.249Z Reads: 109

```
If you have full voltage and have a burst of reverse current from braking, you can cause an over voltage cutoff on the VESC. There's no benefit to setting it lower. A couple users on here had issues with their VESC due to changing the setting.
```

---
## \#9 Posted by: susplus Posted at: 2016-09-14T09:14:56.082Z Reads: 112

```
So, as you just stated, it is highly dependent on braking current. So if let's say one would opt to have a faster braking time then that would create the burst of reverse current from braking. But if one does not tamper with Batt min (regen.) and leaves it at a "safe value for recharging on your battery" then it should not create this hick-up right ?
```

---
## \#10 Posted by: elkick Posted at: 2016-09-14T09:18:40.413Z Reads: 107

```
[quote="susplus, post:7, topic:9571"]
I have followed the instructions given on the Vesc site since i am using the enertion one.
[/quote]

Jacob is wrong on that, i tried to explain it to him, he insists on his view, regardless of people having problems with it.
```

---
## \#11 Posted by: susplus Posted at: 2016-09-14T09:24:28.449Z Reads: 102

```
So what would be your recommendation in this case ?
```

---
## \#12 Posted by: elkick Posted at: 2016-09-14T09:25:35.395Z Reads: 100

```
Leave it at 57V. This value defines only the max. voltage the VESC can take, not the battery. The VESC can take 60V, so with 57V you're on the safe side.
```

---
## \#13 Posted by: susplus Posted at: 2016-09-14T09:42:37.931Z Reads: 99

```
yes the Vesc can take that kind of voltage but as i understood Voltage limits are about how the vesc will manage the battery. SO if you put 57V as input voltage for a 10S battery =max 42V than one may destroy the battery sooner than expected. And Li batteries are already to sensitive :)
```

---
## \#14 Posted by: elkick Posted at: 2016-09-14T09:54:13.238Z Reads: 99

```
That's not the way to protect your batteries. The value defines the voltage the VESC can take. 

If the motor produces more Voltage than the battery can handle, you need a BMS to protect your battery (unlikely if the motor is rated for 10s and your using a 10s battery for example).

If you use the VESC for that limit you're always in danger that the brakes could fail downhill when the limits are hit by spikes and the VESCs shuts off!
```

---
## \#15 Posted by: susplus Posted at: 2016-09-14T09:59:30.307Z Reads: 95

```
ok, understood.  Don't have hills around here :( maybe that is why i did not have this issue yet. will make sure to change it ;) Thanks ( Jinra also)
```

---
