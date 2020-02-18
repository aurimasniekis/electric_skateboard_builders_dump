# DRV fault over temp focbox

### Replies: 27 Views: 522

## \#1 Posted by: Joris97 Posted at: 2018-06-18T13:55:24.462Z Reads: 121

```
i get this error as seen in the screenshot, got this after update, was riding well before.
Does anyone know how to fix this?
![dsdsdsddsss|690x388](upload://hYBhfz8ca5PxyRbnLmEtQaZrdkQ.png)
```

---
## \#2 Posted by: banjaxxed Posted at: 2018-06-18T14:20:07.900Z Reads: 113

```
http://www.electric-skateboard.builders/t/vesc-over-temp-fet/9134
```

---
## \#3 Posted by: Joris97 Posted at: 2018-06-18T14:26:39.661Z Reads: 102

```
cant find a solution there have the right software and didnt change max voltage
```

---
## \#4 Posted by: banjaxxed Posted at: 2018-06-18T14:31:42.427Z Reads: 100

```
http://www.electric-skateboard.builders/t/vesc-over-temp-fet/9134/8?u=banjaxxed

http://vedder.se/forums/viewtopic.php?t=164
```

---
## \#5 Posted by: Joris97 Posted at: 2018-06-18T14:46:30.176Z Reads: 94

```
![26|375x500](upload://zyuJDX7xKYXFBkXs920z0SAXe7I.jpeg)
```

---
## \#6 Posted by: banjaxxed Posted at: 2018-06-18T14:54:39.669Z Reads: 91

```
Yeah it should be R1, but maybe try reflashing to Enertion firmware as they will not support a flashed Focbox....oops too late
```

---
## \#7 Posted by: Blasto Posted at: 2018-06-18T15:07:28.214Z Reads: 86

```
Can you screenshot the Firmware page?
```

---
## \#8 Posted by: Joris97 Posted at: 2018-06-18T15:28:35.992Z Reads: 84

```
![15293356899865801822757749812608|666x500](upload://7NnKuSkdCTsI3ULx51RS4cD2ptp.jpg)
```

---
## \#9 Posted by: JohnnyMeduse Posted at: 2018-06-18T15:32:04.092Z Reads: 80

```
HW should be 412 not 48, that is the wrong firmware..... That why I hate these new vesc tool that too easy to screw up.
```

---
## \#10 Posted by: briman05 Posted at: 2018-06-18T15:54:35.524Z Reads: 79

```
You flashed the wrong firmware it should have done the 410 411 412 file.  You possibly fried it so I would send it in to @JohnnyMeduse to get fixed
```

---
## \#11 Posted by: Blasto Posted at: 2018-06-18T15:57:33.243Z Reads: 75

```
Nah it’s not fried, just need to re-upload the proper fw in the custom fw tab... give me 10mins i’ll show you
```

---
## \#12 Posted by: Joris97 Posted at: 2018-06-18T15:58:02.953Z Reads: 76

```
I thought that when I did the first update I saw the current hw was 48. So chose 48. Guess I need to get a sl link to change it to 412, bootloader is also broken....
Thanks for the help!
```

---
## \#13 Posted by: briman05 Posted at: 2018-06-18T16:00:05.272Z Reads: 76

```
the most of the vesc we use for eboards are 4.12 hardware so you just need to do the correct firmware.
```

---
## \#14 Posted by: Joris97 Posted at: 2018-06-18T16:01:06.478Z Reads: 70

```
Broke the bootloader when desperately trying to fix the problem. Soo stupid 😅
```

---
## \#15 Posted by: Blasto Posted at: 2018-06-18T16:01:53.673Z Reads: 68

```
[quote="Joris97, post:14, topic:59276"]
Broke the bootloader
[/quote]

Re-upload it in the bootloader tab
```

---
## \#16 Posted by: Joris97 Posted at: 2018-06-18T16:02:49.854Z Reads: 69

```
That's what I did, and why it broke I think ...
```

---
## \#17 Posted by: Joris97 Posted at: 2018-06-18T16:06:05.120Z Reads: 69

```
Because it still says 48 when I upload 412
```

---
## \#18 Posted by: Blasto Posted at: 2018-06-18T17:18:26.427Z Reads: 72

```
so just to re-iterate

- uploaded bootloader in bootloader tab
![image|690x415](upload://yfSQXpdOcw9YYmkkU92kNv87saj.png)

-Downloaded the [ 4_12 firmware from vedder's github](https://github.com/vedderb/vesc_tool/tree/master/res/firmwares/410_o_411_o_412)

-Navigate and select "VESC_default.bin" in the 410_411_412 folder and upload it

![image|690x421](upload://eS7XmmxQxirbM85pMzgtcvcYUk6.png)
```

---
## \#19 Posted by: Ebisane9 Posted at: 2018-06-18T18:13:00.721Z Reads: 65

```
not with @ackmaniac he only defaults for hardware 410 411 412 . to access the rest, you have to click a button that says "show non-default firmwares". I guess same with the regular vesc tools?
```

---
## \#20 Posted by: trancejunkiexxl Posted at: 2018-06-18T18:14:48.181Z Reads: 67

```
worse comes to worse u can get a team viewer session with someone who knows whats up, might be worth waiting so you dont break stuff like i did :joy:
```

---
## \#21 Posted by: Joris97 Posted at: 2018-06-18T20:32:54.135Z Reads: 57

```
i cant get the new software on it because boot loader is bad. A friend of mine has a st link , wilt try flashing new boot loader .. thanks for the help, now i know whats wrong
```

---
## \#22 Posted by: CarlCollins Posted at: 2018-06-18T21:57:00.932Z Reads: 53

```
@Joris97

I would love to assist you with this problem via team viewer
you don't need ST-Link to flash it, just get the right firmware file and re-upload it.

I am available now, DM me if you need an assistance now :slight_smile:
```

---
## \#23 Posted by: Joris97 Posted at: 2018-06-19T07:29:54.362Z Reads: 38

```
If u can solve it , then we can do that :slight_smile:
But I'm pretty sure I already tried to upload the right software this time, but it doesn't change..
```

---
## \#24 Posted by: CarlCollins Posted at: 2018-06-19T07:51:34.569Z Reads: 39

```
@Joris97
Lets give it a try
```

---
## \#25 Posted by: Joris97 Posted at: 2018-06-19T08:01:32.137Z Reads: 39

```
I'll send u a dm
```

---
## \#26 Posted by: CarlCollins Posted at: 2018-06-19T08:01:51.216Z Reads: 40

```
Sure, waiting for it
```

---
## \#27 Posted by: Joris97 Posted at: 2018-06-21T14:30:12.979Z Reads: 31

```
I flashed with st Link, now have version 412 on it. But now it gives drv error...
```

---
