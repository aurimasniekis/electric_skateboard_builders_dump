# ESC Making a Beeping Noise

### Replies: 11 Views: 567

## \#1 Posted by: johnkibler Posted at: 2018-08-20T02:33:52.377Z Reads: 86

```
Hey everyone, this is my first esk8 build and I'm a little new to everything. Today I put things together before putting them on the deck to see if they'd work. Sure enough they did, but the ESC won't stop beeping. I saw another post kind of about this but it didn't really solve my problem. I have dual belt motors, a dual motor ESC, and two 5s LiPo batteries wired to the ESC through an XT-60 connector. Everything seemed to be working fine, I just shut it off quickly because the beeping noise was loud and was waking up the whole house. Has anyone else bumped into this problem? Anyone have a clue what went wrong? The motors are 270kv each.
```

---
## \#2 Posted by: mynamesmatt Posted at: 2018-08-20T02:36:00.814Z Reads: 83

```
usually helps to say the exact ESC and motors
```

---
## \#3 Posted by: DAddYE Posted at: 2018-08-20T05:05:32.860Z Reads: 74

```
You got probably a 6s ESC and you might need to either unsolder the jumper or order a 10s
```

---
## \#4 Posted by: johnkibler Posted at: 2018-08-20T12:45:17.579Z Reads: 56

```
Got both from someone on ebay.[https://www.ebay.com/itm/323106655294](https://www.ebay.com/itm/323106655294) [https://www.ebay.com/itm/323326552273?ViewItem=&item=323326552273](https://www.ebay.com/itm/323326552273?ViewItem=&item=323326552273)
```

---
## \#5 Posted by: telnoi Posted at: 2018-08-20T12:50:00.914Z Reads: 48

```
Follow the instructions provided by the seller. You need to setup the esc for the correct voltage range.
```

---
## \#6 Posted by: bartroosen12 Posted at: 2018-08-20T13:07:23.997Z Reads: 42

```
Yeah if the motors are 270Kv I think it's meant to use the 6S or 7S esc so I think the seller provided a 6 or 7S version of the esc.
-# Ow no I'm wrong 10S is also fine for these motors!
I think @dickyho knows more about these.
```

---
## \#7 Posted by: johnkibler Posted at: 2018-08-20T16:37:50.402Z Reads: 36

```
I guess part of the problem might be that I haven't set it up yet. Is there some more or less standard way to calibrate an ESC, or does it vary with every one of them? sorry this is probably another beginner question
```

---
## \#8 Posted by: bartroosen12 Posted at: 2018-08-20T17:36:37.184Z Reads: 34

```
No you don't need to set it up. It's just an alarm that you have a to high voltage connected to the esc.
If you got the 6S version it needs 22,2V and you put like 37V on the esc with your 10S battery, so that's why it's beeping.
![IMG_20180820_193857|281x500](upload://9RvI6AuIfM9rkGCFxWV3XAW4Px0.jpg)
You probably didn't read the discription, if you want the 10S or 7S version you need to leave a note when you order the esc.
If you don't leave a note the seller will sent you the 6S version by default.
![s-l400%20(1)|300x400](upload://ppwky1Yae9BosneufSjh9rHfpoo.jpg)
I guess he means the red circle in the picture are the 2 'bridges' so you need to carefully unsolder them like said in the discription to set the esc to 10S battery input voltage :wink:
```

---
## \#9 Posted by: Toughook Posted at: 2018-08-20T18:18:59.847Z Reads: 31

```
So are the 6, 7 & 10s ESC the same unit, just the solder on the bridges differs? Same capacitors and chips etc?
```

---
## \#10 Posted by: bartroosen12 Posted at: 2018-08-20T19:34:30.357Z Reads: 27

```
They are the same units yep
```

---
## \#11 Posted by: johnkibler Posted at: 2018-08-21T15:27:54.530Z Reads: 18

```
Thank you, I guess next time I should take a closer look at the description
```

---
