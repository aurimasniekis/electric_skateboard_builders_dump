# HELP, the DRV8302 is getting extremely hot just from turning the board on

### Replies: 10 Views: 257

## \#1 Posted by: buildityourself Posted at: 2019-05-21T00:01:01.000Z Reads: 86

```
So about a week ago I stepped on my board to test it and it budged and then refused to function. So now the vesc blinks red in bursts of 3 and there is no response from the motor when the trigger is pulled. I plug the loop key in and somehow I get massive amount of heat from the DRV chip. So much so that I can't even keep my finger on it.

I have a 192kv motor and a 10s5p with 60/-60amp motor max/min and 40/-12 batt max/min. 

Any help or ideas is appreciated greatly, thanks!!
```

---
## \#2 Posted by: briman05 Posted at: 2019-05-21T00:22:36.126Z Reads: 82

```
It sounds like your drv has a fried. What vesc do you have.
```

---
## \#3 Posted by: buildityourself Posted at: 2019-05-21T00:29:56.352Z Reads: 78

```
I have a Flipsky FSESC 4.12 i think. If the DRV is fried, would it still be getting this hot? Any ideas on preventing this from happening once I replace the chip? thanks
```

---
## \#4 Posted by: briman05 Posted at: 2019-05-21T00:32:54.397Z Reads: 75

```
Did you run it on foc or bldc.
```

---
## \#5 Posted by: Pavlo_H Posted at: 2019-05-21T00:42:57.043Z Reads: 75

```
The same thing happened to me. After my DRV died, the DRV started to get really hot even from me just plugging in the battery and letting it sit there. Also you should have a fault code inside the VESC Tool.
```

---
## \#6 Posted by: buildityourself Posted at: 2019-05-21T21:05:45.785Z Reads: 45

```
BLDC (10char)
```

---
## \#7 Posted by: buildityourself Posted at: 2019-05-21T21:10:04.043Z Reads: 44

```
I plugged the board into my computer and ran the vesc tool, just not sure exactly what to press to trouble shoot and get those error messages. Also, once you replaced the chip how did you prevent it from becoming fried again? I have seen on another thread that it is caused from a spike in voltage. Does my vesc set up values look alright?
```

---
## \#8 Posted by: Pavlo_H Posted at: 2019-05-21T21:25:49.298Z Reads: 40

```
Not really sure how to prevent it from happening again. I just replaced my VESC and haven’t had a problem since. Maybe to prevent it start with fixing the voltage spikes with a TVS diode. @Pryside shows a way of fixing this in his video by using a TVS Diode between the negative and positive terminals. https://youtu.be/C8n8ceZM9qY Here is a way of how to attach it to the VESC. https://www.electric-skateboard.builders/t/3d-printed-boosted-board-killer/88803/104
```

---
## \#9 Posted by: briman05 Posted at: 2019-05-21T21:32:18.597Z Reads: 38

```
You go into the terminal and type in fault
```

---
## \#10 Posted by: Pryside Posted at: 2019-06-10T16:45:38.095Z Reads: 20

```
Add the TVS diode I mentioned in the video, the P6KE56CA and you can also add a low ESR cap directly onto the pcb for example the EEUFR1J681L.
Thats the way I recommend it to friends who run their old 4.12 HW vescs on 12S and they havent had any issues since
```

---
