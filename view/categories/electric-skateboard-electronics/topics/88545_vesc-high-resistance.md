# VESC high resistance

### Replies: 18 Views: 284

## \#1 Posted by: TheCookieHunter Posted at: 2019-03-28T08:13:11.908Z Reads: 93

```
Hello,
I have a pretty big problem wit my VESC  4.13.I have changed the DRV chip because i have burned it.After the change i ran motor detection on the new VESC Tool and the VESC  with the changed DRV chip had a much higher resistance and a smaller amperage that can go trough.![20190305_185439|374x500](upload://k0W1sH8nzSla0shJjjHRqvHiUTf.jpeg)
```

---
## \#2 Posted by: linsus Posted at: 2019-03-28T09:01:53.498Z Reads: 78

```
Looks normal to me. The current is only what the tool recommends. You can override it if you like.
```

---
## \#3 Posted by: TheCookieHunter Posted at: 2019-03-28T09:14:27.729Z Reads: 76

```
https://youtu.be/bBWIWsZFpyg 

Watch this video. I do not think that the sound from the motor is right.
```

---
## \#4 Posted by: linsus Posted at: 2019-03-28T09:55:40.149Z Reads: 70

```
Which one is the replaced one? the closest?

And wtf happened when it made full halt? Never seen that
```

---
## \#5 Posted by: TheCookieHunter Posted at: 2019-03-28T10:00:18.235Z Reads: 64

```
Yep the closer one is the VESC with the changed drv.Also when i ride and give suddenly full trothel it slowes down suddenly.I don't know what to do.
```

---
## \#6 Posted by: linsus Posted at: 2019-03-28T10:11:58.006Z Reads: 57

```
any red flash from vesc?
I would look over the soldering, did you use a reflow hot air solder station when replacing the drv?
```

---
## \#7 Posted by: TheCookieHunter Posted at: 2019-03-28T10:15:40.387Z Reads: 59

```
Yes i used a hot air soldering station but i don't have a microscope to see if there is a bad connection.But i think if one of the connections were bad it would not work at all.
```

---
## \#8 Posted by: Surfer Posted at: 2019-03-28T10:18:00.655Z Reads: 55

```
 If you are running the last firmware I recommend to try a older version, it seems more finiky the new detection and can communication
```

---
## \#9 Posted by: TheCookieHunter Posted at: 2019-03-28T10:21:59.687Z Reads: 58

```
I can't run it at all with the new firmware.I went back to the old firmware and i still have these problems.
```

---
## \#10 Posted by: Surfer Posted at: 2019-03-28T10:49:23.461Z Reads: 52

```
I mean a even older version, your picture looks quite up to date firmware, try something like 3.48 or so
```

---
## \#11 Posted by: TheCookieHunter Posted at: 2019-03-28T11:05:44.555Z Reads: 51

```
In the picture is the newest firmware but when i set it up one of the motors spins and the other sounds as if it is scraping something.I went back to the older firmware version and the glitching of the ESC with the changed drv.
```

---
## \#12 Posted by: linsus Posted at: 2019-03-28T12:12:18.203Z Reads: 43

```
apply plenty of flux, try resolder all the legs (2 pairs should bridged if i remember correctly)
Check for missing components, any that flew off? had gate resistors fly off and a cap once, so not impossible

Then try again
```

---
## \#13 Posted by: TheCookieHunter Posted at: 2019-03-28T17:16:28.697Z Reads: 37

```
![20190328_161805|374x500](upload://jDUqwOBKYtmM3HrPwOWHI6URNqW.jpeg) ![20190328_161827|375x500](upload://stMLgeGhM9r8NgWvgKqTFVeuXX8.jpeg) 
Is there a problem if one of the drvs is 78... and the other is 58...
```

---
## \#14 Posted by: MysticalDork Posted at: 2019-03-29T04:38:19.656Z Reads: 28

```
I'm pretty sure those numbers are date codes. Shouldn't affect anything.
```

---
## \#15 Posted by: TheCookieHunter Posted at: 2019-03-29T06:47:18.641Z Reads: 25

```
![Screenshot_20190329-084555_eBay|281x500](upload://v6wGMhaUYr8wpLl4kFmAv1Yl1SY.jpeg) 
I bought this drv for replacement one.Is it ok?
```

---
## \#16 Posted by: linsus Posted at: 2019-03-29T08:39:18.327Z Reads: 23

```
Ebay... not the place for components xD

Too high risk..
```

---
## \#17 Posted by: Mich21050 Posted at: 2019-03-29T08:54:15.588Z Reads: 20

```
https://www2.mouser.com/Search/Refine?Keyword=drv8302  \
https://lcsc.com/product-detail/MOS-Drivers_TI_DRV8302DCA_DRV8302DCA_C84672.html

Those would be better suppliers :slight_smile:
```

---
## \#18 Posted by: TheCookieHunter Posted at: 2019-04-02T20:51:26.671Z Reads: 13

```
What is the difference between  
595-DRV8302DCAR    and     595-DRV8302DCA
```

---
