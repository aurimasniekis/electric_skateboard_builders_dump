# What settings should I be running on my board?

### Replies: 14 Views: 340

## \#1 Posted by: ajplant96 Posted at: 2019-05-06T03:10:38.393Z Reads: 125

```
So I'm still in the process of putting together my Evolve Carbon GT restoration using a Focbox Unity, generic 60a BMS from Ebay, 140KV 5065 Racerstar motors (replacing with 170KV 6355 Maytech motors eventually), and a 10s4p battery rated at 10.5AH (soon to be replaced with a 10s5p using 18650 Samsung 30q cells)

I'm just wondering what settings I should be running my board with when setting up the Focbox Unity.
```

---
## \#2 Posted by: mynamesmatt Posted at: 2019-05-06T03:26:44.614Z Reads: 123

```
![SEARCHGIFlookacrazycoolnotcap|640x360](upload://91D857RdjdvdTGB6mvtQIO8LBiU.gif)
@Sn4pz i use this way too much
```

---
## \#3 Posted by: AlanZhou Posted at: 2019-05-06T03:30:11.698Z Reads: 118

```
Dammit just before I was bout to post
```

---
## \#4 Posted by: Hummie Posted at: 2019-05-06T04:04:53.151Z Reads: 109

```
see what u like
```

---
## \#5 Posted by: ajplant96 Posted at: 2019-05-21T08:19:40.792Z Reads: 74

```
I only post asking for advice if the search function ends up being as pointless as your response...
```

---
## \#6 Posted by: Linny Posted at: 2019-05-21T08:34:37.361Z Reads: 74

```
80A motor max and - 80A brake seems good, bump it down to 60 if its too torquey for you. 

For a 10s5p 30Q, 60A is good. 

Regen braking can be -15
```

---
## \#7 Posted by: ajplant96 Posted at: 2019-05-21T12:51:31.861Z Reads: 62

```
Thank you! Will test 80A out but tbh I did try 60A about a week ago and that was plenty torquey to the point of sticking to slow mode, hopefully 80A is a perfect compromise to just stick to that, otherwise like 50A for R-Spec I guess.
```

---
## \#8 Posted by: Linny Posted at: 2019-05-21T13:15:24.987Z Reads: 58

```
Ah, 80A is definitely more powerful than 60. Since 60 is too much, try 50 then. I always do low numbers and bump it up if i feel like i need more boost. 


But 60A battery is good enough. I am on 60A on a 10s4p. A 10s5p might be able to output more but i like to be safe
```

---
## \#9 Posted by: briman05 Posted at: 2019-05-21T13:22:35.945Z Reads: 58

```
@ajplant96 the 5065 racerstar motors are only rated to a 36A max so you can push more current over the lines but it isnt going to do anything.

![image|621x499](upload://qnLI2IDA6SJz4g0Yj5icamIGOkR.jpeg)
```

---
## \#10 Posted by: ajplant96 Posted at: 2019-05-22T10:51:13.356Z Reads: 38

```
With either battery would you say I should take into account the 60a rating on my bms?
```

---
## \#11 Posted by: Linny Posted at: 2019-05-22T11:33:34.612Z Reads: 35

```
Yea, since your BMS is rated for 60A. If you do more than 60A for example, your BMS will cut power to protect the battery from going kaboom
```

---
## \#12 Posted by: ajplant96 Posted at: 2019-05-22T11:39:11.935Z Reads: 36

```
Okay, but that’d be only if it were possible to draw more than 60a I’m guessing? Given the current motors on the board only do 36a as previously stated it shouldn’t be an issue? (60a was more than enough torque for me though)
```

---
## \#13 Posted by: Linny Posted at: 2019-05-22T11:49:15.354Z Reads: 36

```
Yep, should be fine.
```

---
## \#14 Posted by: ajplant96 Posted at: 2019-05-23T10:31:49.738Z Reads: 26

```
Sweet, thanks for your help. Won't be long 'til I switch out for the 10s5p and 6355 motors anyway so the fun is only just beginning with getting this thing running again.
```

---
