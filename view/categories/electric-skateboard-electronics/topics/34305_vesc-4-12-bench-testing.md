# VESC 4.12 bench testing

### Replies: 9 Views: 1295

## \#1 Posted by: skyblaster Posted at: 2017-09-29T19:04:50.103Z Reads: 100

```
I don't have a battery pack as of yet, but would like to configure my VESC connected to a 6364 motor.

If I'm just running this on the bench with no load, can I use a 50VDC 1.5A supply? I suspect 75W is plenty to spin the motor with no load, but just wanted to check here first so I don't blow anything up.
```

---
## \#2 Posted by: scepterr Posted at: 2017-09-29T19:25:45.172Z Reads: 91

```
You need to setup vesc with battery that will be used, otherwise you'll just have to do it again.
```

---
## \#3 Posted by: Martinsp Posted at: 2017-09-29T19:30:06.132Z Reads: 90

```
That is not entirely true. You can use a power supply, in fact it is recommended because it provides a current limiting feature. You can use any voltage does not need to be the voltage of your battery. However if you set your voltage limits (low voltage limits) in the VESC and you  have them for example set to 30V cutoff end, the vesc will give you an under voltage error and will not work until you raise voltage or change the limit. Hope it makes sense
```

---
## \#4 Posted by: skyblaster Posted at: 2017-09-29T19:37:16.321Z Reads: 86

```
I appreciate the answers. I have an old HP 6226B at my disposal and just want to get comfortable with the BLDC software.
If this is the **tutorial** everyone mentions in VESC threads, I'm not sure why it's not a pinned post: http://www.electric-skateboard.builders/t/new-vesc-user-read-this-complete-walktrough-of-the-vesc/2980
```

---
## \#5 Posted by: SilentException Posted at: 2017-09-29T19:47:33.702Z Reads: 81

```
I started to configure my FOCBOX using bench PSU. But haven't actually done motor detection on it. I thought 5A weren't going to cut it so didn't even try. Would be good to know numbers needed to do motor detection, of course it is going to differ by the motor but even ballpark figures would be better than nothing. I got the Turnigy 7-in-1 meter recently so I might use it to get some numbers, just need to find the time... :)
```

---
## \#6 Posted by: scepterr Posted at: 2017-09-29T20:33:40.647Z Reads: 68

```
Bench supply is recommended for newly soldered vesc setup. I have never seen the same detection results on bench psu that I do with battery. (28 vesc at this point)

If you're running a vesc with results achieved from bench psu and it fries....now you know
```

---
## \#7 Posted by: Martinsp Posted at: 2017-09-29T20:35:47.795Z Reads: 61

```
I usually refer people to this tutorial, in my opinion it is easier to understand the video that just reading text. It is pretty well explained.
https://www.youtube.com/watch?v=5HLZaMcYRuY
```

---
## \#8 Posted by: scepterr Posted at: 2017-09-29T20:38:05.764Z Reads: 59

```
I trust @chaka
  http://www.electric-skateboard.builders/t/vesc-faq-when-to-use-low-voltage-vesc-configuration/1965
```

---
## \#9 Posted by: skyblaster Posted at: 2017-09-29T20:48:43.586Z Reads: 59

```
10-4, sir. I totally understand and certainly don't mind running through everything a second time once my battery is built.
```

---
