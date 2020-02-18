# Torque 190kv motor issue, need advise!

### Replies: 14 Views: 573

## \#1 Posted by: dotruongq Posted at: 2017-06-01T23:42:17.593Z Reads: 72

```
Hi all community
I just bought the whole set up include new motor and VESC, i ran into a weird issue when my motor seem to brake ( or not spinning all of the sudden ), when running at slow speed, it shakes a lot and not spin at all, cause me to fall off the board. it happens a lot of time, i included a video below. Sorry for my english, any advise would be highly appreciated !

https://youtu.be/1hgiuhxGHxY
```

---
## \#2 Posted by: JLabs Posted at: 2017-06-01T23:44:28.396Z Reads: 66

```
Did you run motor detection on the vesc and apply the values?
```

---
## \#3 Posted by: dotruongq Posted at: 2017-06-01T23:47:07.018Z Reads: 61

```
Yes i did Jlabs, i applied them and tried again, still have same issue
```

---
## \#4 Posted by: dotruongq Posted at: 2017-06-01T23:48:55.377Z Reads: 60

```
https://youtu.be/knvxLN1vAQw
```

---
## \#5 Posted by: JLabs Posted at: 2017-06-01T23:54:46.734Z Reads: 54

```
Post some screenshots of your Motor Config, BLDC, App Config, and PPM tabs (helps us help you).
```

---
## \#6 Posted by: dotruongq Posted at: 2017-06-01T23:55:31.366Z Reads: 55

```
<img src="/uploads/db1493/original/3X/e/9/e94d40d9382e346811e827f86901885abde6db8a.png" width="690" height="415">
```

---
## \#7 Posted by: dotruongq Posted at: 2017-06-01T23:55:52.678Z Reads: 51

```
<img src="/uploads/db1493/original/3X/0/f/0f803d7e7c636e338c08e7c430bacf8bbf9545c6.png" width="690" height="413">
```

---
## \#8 Posted by: dotruongq Posted at: 2017-06-01T23:56:12.646Z Reads: 52

```
<img src="/uploads/db1493/original/3X/7/5/75d2d9dd0880f85d6e0c1aa83bd48fc8bcb23aaf.png" width="690" height="417">
```

---
## \#9 Posted by: dotruongq Posted at: 2017-06-01T23:56:36.717Z Reads: 49

```
<img src="/uploads/db1493/original/3X/e/5/e5cc206a75b9ddb0eb5abb2312578428de5a1fe2.png" width="690" height="420">
```

---
## \#10 Posted by: JLabs Posted at: 2017-06-02T00:00:35.601Z Reads: 48

```
Looks like your using @Ackmaniac's too. You'll want to change to watt control no reverse with brake in the PPM tab. 

When you run motor detection you have to follow these steps, it may throw off your results if you dont:

1. Select disabled in the PPM tab
2. Reboot the VESC & reconnect when its done rebooting
3. Run motor detection
4. Select  watt control no reverse with brake in the PPM tab
5. Reboot the VESC & reconnect when its done rebooting
```

---
## \#11 Posted by: dotruongq Posted at: 2017-06-02T00:10:13.204Z Reads: 47

```
so i follow those step and i dont see it happens as much as before but still sometime, but i notice the issue will happen when :  pull the  throttle too fast ( from 50% to 100%) it will likely happen, if i slowly go up then it wont,
```

---
## \#12 Posted by: JLabs Posted at: 2017-06-02T00:11:43.546Z Reads: 47

```
You wont do that while riding and bench test dont provide an accurate acceleration curve anyway. Should be normal when riding. Your settings look pretty good to me.

Also, what is your battery chemistry and voltage? Your cutoff is a bit high.
```

---
## \#13 Posted by: dotruongq Posted at: 2017-06-02T00:19:32.252Z Reads: 45

```
JLabs, 
the battery is graphene 10000mah 6S 15C, waht should i set my cutoff too, i changed it to the wattage mode like u said, i will go to field test it and comeback with result !
```

---
## \#14 Posted by: JLabs Posted at: 2017-06-02T00:25:00.055Z Reads: 45

```
You can go to 3v per cell with a lipo minimum. Not sure if it's the same for grahpene or not.
```

---
