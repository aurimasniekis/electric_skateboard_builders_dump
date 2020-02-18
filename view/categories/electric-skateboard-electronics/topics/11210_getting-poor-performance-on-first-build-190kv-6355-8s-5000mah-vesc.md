# Getting poor performance on first Build 190kv 6355 8s 5000mah VESC

### Replies: 16 Views: 1176

## \#1 Posted by: Bimmox Posted at: 2016-10-16T02:12:15.203Z Reads: 154

```
Hey guys
So I just set up everything on my first build and everything looks fine except when I got on it, it will barely climb a small hill (10% incline). Its max speed on flat is probably 10-15 mph, but when I checked on the calculator my estimated speed was around 20-25 mph with 70% efficiency
Maybe I'm missing some settings on the BLDC tool?  Something has got to be wrong...
Also Im only 140lbs
Any help would be very helpful :sweat:
Thanks in advance
Pablo
```

---
## \#2 Posted by: Smorto Posted at: 2016-10-16T02:13:56.610Z Reads: 152

```
Im not sure how to help you but I am interested to see since my build is going to be with pretty much those exact specs
```

---
## \#3 Posted by: Bimmox Posted at: 2016-10-16T02:15:57.551Z Reads: 150

```
I have probably done something wrong... but I was so excited to get it running and it was fun but quite decepointing it couldn't even get up a hill...
```

---
## \#4 Posted by: Blasto Posted at: 2016-10-16T02:18:31.629Z Reads: 148

```
Post pics of your setup, that will help. And some screen shots of your settings if your are unsure
```

---
## \#5 Posted by: roamin Posted at: 2016-10-16T02:27:03.736Z Reads: 143

```
With 8S, you should be getting good performance! Definitely sounds like you need to modify BLDC. Hope someone on the forum has reccommended settings for a 190 kV 6355 8S configuration.
```

---
## \#7 Posted by: Hillso Posted at: 2016-10-16T03:34:23.482Z Reads: 128

```
low amp limit?
```

---
## \#8 Posted by: Bimmox Posted at: 2016-10-16T03:40:58.111Z Reads: 126

```
<img src="/uploads/db1493/original/3X/1/8/185692b3aa7814be88ce858a2d90427e034d723c.jpg" width="374" height="500"><img src="/uploads/db1493/original/3X/5/e/5ef1a892e86aa74779098649c19205f12adf62c7.jpg" width="374" height="500"><img src="/uploads/db1493/original/3X/b/7/b774c68a9e0f3f0052d59286af04bffa3490e07a.jpg" width="374" height="500">
```

---
## \#9 Posted by: Bimmox Posted at: 2016-10-16T03:58:00.887Z Reads: 115

```
My motor amp limit is set to 60 :/
```

---
## \#10 Posted by: lox897 Posted at: 2016-10-16T07:39:45.286Z Reads: 108

```
What gearing?
```

---
## \#11 Posted by: Jinra Posted at: 2016-10-16T07:49:41.192Z Reads: 109

```
What's your battery cutoff? Pics of VESC settings would be useful.
```

---
## \#12 Posted by: Bimmox Posted at: 2016-10-16T11:10:14.227Z Reads: 100

```
16/36T
83 mm wheels
```

---
## \#13 Posted by: Bimmox Posted at: 2016-10-16T13:16:36.767Z Reads: 97

```
I believe my battery cut off is at 30-33, realised it should be lower. This is probably why it was slughish, it must've sensed the battery was too low when it was around 60% charge and that is why its been so slow, going to change these settings as soon as I get home, unfortunately stuck at work for a few hours.
Let me know if that could possibly be the issue!
```

---
## \#14 Posted by: saul Posted at: 2016-10-16T16:05:01.604Z Reads: 89

```
yes thats exactly what it is. once the low voltage kicks in you have limited power, so very low top speed and slow...

8s is only 33v when full, so I would use about 28/29v 8*3.5  which will have the packs around 3.7 resting...

youre going to want to strap everything down a bit more for full power! :sunglasses:
```

---
## \#15 Posted by: Bimmox Posted at: 2016-10-16T16:54:36.326Z Reads: 82

```
Oh of course!
Also i had to remove all the temporary strapping for you guys to see the actual setup. Also need to locktite the motor mount. This all makes sense now, I guess I was so impatient to try it out that I didnt think of battery cut off yesterday. Ill change the settings and let you know, but I have a feeling I found the issue.
Thanks again y'all for the help!
```

---
## \#16 Posted by: Bimmox Posted at: 2016-10-16T19:23:43.135Z Reads: 73

```
I confirm that the low voltage cutoff was the issue! Charged my batteries fully and changed the values of the cutoff, it now works like a beast!!! Wow that thing is way more powerful than I thought it would be! I feel like I could go up a 30% incline with... Although not for too long haha
Thanks again for all of you!!!
```

---
## \#17 Posted by: Smorto Posted at: 2016-10-16T19:26:08.086Z Reads: 74

```
Sweet! Good to know for my build
```

---
