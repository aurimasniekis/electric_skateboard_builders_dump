# Issues with Torque Boards Dual 6372 motor setup (brakes, sensors, etc.)

### Replies: 6 Views: 194

## \#1 Posted by: oahu_greg Posted at: 2018-09-24T01:38:51.016Z Reads: 61

```
Can anyone please help with my brake settings? I have tried adjusting everything that I can think of, and regardless of settings I always lock the wheels with the slightest touch of the remote.

I was thinking about going FOC to fix the issue, but cannot get the sensors to be recognized in FOC mode. I'm using New 4.12 VESCs & Dual 6372 motors from , 10s2p battery from Ownboard

![08%20PM|690x390](upload://98AtLot77IUnaze6771JWcM6jmN.png) ![26%20PM|690x392](upload://nFWbpoDPZeD59VbZeOojkQi6mxu.png) ![46%20PM|690x393](upload://fmOh9vhgpr97vz2w9K24owgHXaK.png) ![17%20PM|690x388](upload://rvQDy164r8KRYAYTgbdfXbM1G07.png) ![59%20PM|690x390](upload://vBsSJ8LtZKDlo3fKbxnJYHzX7mk.png) ![25%20PM|690x387](upload://bMdrNYpJ3ec5WQ8BcFRFoUNh5xl.png) ![38%20PM|690x393](upload://8hmct4hw5H9MfRedcGrFjOKEuao.png) ![13%20PM|690x393](upload://q21u93XKkXBiT3ilwvWrakdXeFu.png) ![56%20PM|690x388](upload://yVJmeQGBPWuaIPHlUfbuQHzO4NU.png) ![46%20PM|690x389](upload://tsCUswQT6Xdk87JEuGtQay42fAZ.png) ![37%20PM|690x389](upload://dYcgTc2aZZK6gqVbKufiyI92Hux.png) ![15%20PM|690x391](upload://uYwwbBaaopLO5eTW0StLVlKHC3K.png) ![26%20PM|690x393](upload://k8Ote0lbY2ezYHcmeDNFubGvw42.png)
```

---
## \#2 Posted by: Winfly Posted at: 2018-09-24T01:49:41.316Z Reads: 46

```
What remote are you using?  Try lowering the dead zone %?
```

---
## \#3 Posted by: oahu_greg Posted at: 2018-09-24T02:14:27.539Z Reads: 43

```
Thank you for the suggestion, I will be sure to try it!

I'm currently using the 2.4 Nano remote.
```

---
## \#4 Posted by: ksfacinelli Posted at: 2018-09-24T03:20:43.952Z Reads: 37

```
Try reducing your deadband down to 3-4%. I had similar problem the deadband at 15% created a large pause before kicking in and when it does you are already pretty far up on the curve. You should also feel your acceleration smooth out quite a bit. I am running the same remote and this adjustment made a huge difference.
```

---
## \#5 Posted by: oahu_greg Posted at: 2018-09-24T03:49:22.631Z Reads: 30

```
Just tried it and it helps IMMENSELY! 
Thank you, thank you, thank you!
```

---
## \#6 Posted by: ksfacinelli Posted at: 2018-09-24T03:54:32.448Z Reads: 29

```
Yea I am glad to hear it worked had the same problem and a member from the board pointed me in the right direction not sure why the tool defaults to 15% as this is way to much....
```

---
