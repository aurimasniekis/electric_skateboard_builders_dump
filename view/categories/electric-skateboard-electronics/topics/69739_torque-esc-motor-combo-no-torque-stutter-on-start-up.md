# Torque ESC &amp; Motor combo: No torque &amp; stutter on start up

### Replies: 25 Views: 565

## \#1 Posted by: indyglassman Posted at: 2018-10-01T13:32:57.212Z Reads: 117

```
**Problem:**
After setting up my board I went to test it and found that under load (standing on the board) the motor jitters and has trouble starting.  When not under load it spins just fine.

**My Equipment:**
Torque ESC BLDC ([Link](products/torque-esc-bldc-electronic-speed-controller))
Torque Motor 6355 190KV ([Link](collections/electric-skateboard-motors/products/electric-skateboard-motor-6355-190kv))
12s2p Battery Pack ([Link](products/torque-esc-bldc-electronic-speed-controller))

**Steps I've taken:**
1. Upgraded the VESC firmware.
2. Ran through the motor setup wizard successfully.
3. Ran through the input wizard successfully.

**Parameters in VESC tool**
BLDC Mode
Motor Current Max: 80A
Motor Current Max Brake: -60A
Absolute Max Current: 100A
Battery Current Max: 50A
Battery Current Max Regen: -10A
Max ERPM: 100,000
Max ERPM Reverse: -100,000
ERPM Limit Start: 80%

D 0.20
I 3.00A
w 5000 RPM
P 0.00 degrees
IB 3.00 A
HB 3.00 A

I've read other threads on here and tried some of the suggestions.  Nothing thus far has helped.  This morning I did change one parameter that seemed to help quite a bit, but wasn't sure it's the RIGHT thing to change.  
On the General Menu, Advanced Tab I changed Minimum Duty Cycle from 0.5% to 2.0% which seems to have made a difference (at least with bench testing, haven't ridden yet).

Thanks in advance for any help/suggestions.
```

---
## \#2 Posted by: Andy87 Posted at: 2018-10-01T13:53:56.367Z Reads: 104

```
Off topic, but seems a bit high bat max values for this esc. Plus I would limit my max erpm to +-60000 with 12s 190kv.

If you run through the motor wizard, the hall sensors had a valid result and you also applied this result and downloaded it to the esc?

Did you run the motor detection with belt or without!
```

---
## \#3 Posted by: Sn4pz Posted at: 2018-10-01T14:07:51.988Z Reads: 97

```
youre supposed to do it with or without....? I cant remember which way I did mine and youre making me second guess myself... x)
```

---
## \#4 Posted by: indyglassman Posted at: 2018-10-01T14:10:10.345Z Reads: 93

```
I got the Battery Current Max of 50A from https:// support.  The 100A may be too high indeed.  Prob need to drop that down to 60 or so I'm guessing.
```

---
## \#5 Posted by: indyglassman Posted at: 2018-10-01T14:10:59.777Z Reads: 91

```
Not sure I follow you regarding "With or without."  With or without what?
```

---
## \#6 Posted by: threebysix Posted at: 2018-10-01T14:12:13.555Z Reads: 89

```
I think your battery max current is too high for a 12s2p. 2px15a = 30. So max should be 30A.

Have you tried to kick push first, start the board rolling, then throttle?
```

---
## \#7 Posted by: Andy87 Posted at: 2018-10-01T14:14:12.862Z Reads: 84

```
Suggested to make it without
```

---
## \#8 Posted by: indyglassman Posted at: 2018-10-01T14:14:52.933Z Reads: 82

```
, who is the vendor gave me the battery max value of 50A for that pack.

I can get the board started and yes kick starting will get it going but after reading others using similar components you should not have to do that when it's setup correctly.
```

---
## \#9 Posted by: Andy87 Posted at: 2018-10-01T14:14:55.847Z Reads: 81

```
Without belt
```

---
## \#10 Posted by: Sebike Posted at: 2018-10-01T14:16:52.242Z Reads: 75

```
What battery do you have? Link points to the esc. 
Batt max most probably set too high. 

Jitter sounds like sensor wire is not connected/bad connection, or hall sensor mode not enabled in vesc, or sensor detection not set up, or hall sensors are doa...?
```

---
## \#11 Posted by: Andy87 Posted at: 2018-10-01T14:18:30.999Z Reads: 74

```
Besides the fact that your battery max can output 40a I wouldn‘t run 50a on a hw4.12 vesc without heatsink. Just my suggestion. I know they write 50a on the homepage
```

---
## \#12 Posted by: Sebike Posted at: 2018-10-01T14:21:59.080Z Reads: 68

```
Try running sensor detection again. No problem or error?
```

---
## \#13 Posted by: indyglassman Posted at: 2018-10-01T14:22:14.028Z Reads: 66

```
Andy87 - Thanks!  I ran it with out the first several times, but this last time I ran it with - So, I do need to go back and remove the belt and run again.  

Also, thanks for the suggestion on the max erpm.  I had no idea what to set this number to.

Yes, I have applied the result of the motor wizard after it ran.  I know many people forget that, but I did do that.
```

---
## \#14 Posted by: indyglassman Posted at: 2018-10-01T14:23:48.290Z Reads: 61

```
Battery is 12s2P

I am running in BLDC mode so the sensor wire is not connected.  BLDC vs FOC is new to me but when I talked to diyelectricskateboard support he said that I should run in BLDC with out the sensor wire (in fact he said it won't work with the sensor wire connected).
```

---
## \#15 Posted by: Sebike Posted at: 2018-10-01T14:24:52.689Z Reads: 63

```
Ok. So that's why it jitters.

Push start is your friend then. 

I know it's 12s2p, but what cells? 🙂
```

---
## \#16 Posted by: indyglassman Posted at: 2018-10-01T14:24:52.893Z Reads: 62

```
Ok, I'll drop the max down to 40A and see how it works.   I don't think that's affecting my jitter issue but it may save my ESC.   What should the absolute max current be set to??
```

---
## \#17 Posted by: Andy87 Posted at: 2018-10-01T14:28:06.704Z Reads: 63

```
Just let the absolute how it is. Looks good.
Without sensors it’s normal that it jidders.
Like @Sebike said, give your board a small push and it should run without problems
```

---
## \#18 Posted by: indyglassman Posted at: 2018-10-01T14:28:38.406Z Reads: 65

```
Samsung 30Q.

So are you saying that you would expect a pack that is 12S2P to always require a push start?
```

---
## \#19 Posted by: Andy87 Posted at: 2018-10-01T14:29:29.495Z Reads: 66

```
It’s not the pack. It’s because you don’t use your sensors.
```

---
## \#20 Posted by: Sebike Posted at: 2018-10-01T14:36:42.761Z Reads: 61

```
People run bldc mode with sensors. I don't know why the TB support guy told you otherwise. I don't like stutter, so I'd run with sensors if I were you.

With a 12s2p 30q batt max should be 15 to maximum 20 a per p pack = 30 to 40 for the battery. Has nothing to do with your motor issues though.
```

---
## \#21 Posted by: indyglassman Posted at: 2018-10-01T14:40:29.087Z Reads: 58

```
Thanks everyone for your help!  Great forum and I appreciate the support.

I will order the sensor wire -- I can order for diyelectricskateboard but wondering if there is another option in the US?  I'm not totally happy with them.  If you have suggestions of where else to buy, let me know.
```

---
## \#22 Posted by: Sn4pz Posted at: 2018-10-01T14:45:45.511Z Reads: 56

```
the belt
char
```

---
## \#23 Posted by: Sebike Posted at: 2018-10-01T14:46:01.867Z Reads: 56

```
There's a good chance someone on the forum has one to send for shipping or cheap. Go write in the wanted thread.. 
😊
https://www.electric-skateboard.builders/t/wanted-cheap-or-free-in-progress-requests-only/
```

---
## \#24 Posted by: Andy87 Posted at: 2018-10-01T16:55:16.268Z Reads: 46

```
If you have a solder iron you can always by a 6pin 2mm jst with cables for cheap than cut the small plug from the motor sensor wires and solder the 2mm one on it.

Start with 35a motor max setting and look if the esc becomes hot during your ride. If it stays around 40 degrees you can always adjust it more high after. Motor max i would set between 60-80a. Should be more than enough
```

---
## \#25 Posted by: indyglassman Posted at: 2018-10-02T18:25:58.299Z Reads: 41

```
I got to ride today and I have to say, I like it!   I do have a sensor wire on order and I'll install that and redo the VESC setup once it arrives.  But it felt really good on my quick 3 mile ride.  I appreciate all the help.

I'm going to post in another thread - I have a question specifically about the battery monitor that is onboard my battery.
```

---
