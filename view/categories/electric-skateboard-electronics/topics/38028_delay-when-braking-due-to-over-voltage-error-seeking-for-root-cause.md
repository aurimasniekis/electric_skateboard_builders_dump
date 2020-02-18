# Delay when braking due to Over Voltage Error - Seeking for root cause

### Replies: 7 Views: 392

## \#1 Posted by: carletto Posted at: 2017-11-11T16:54:01.810Z Reads: 71

```
Hi everyone,
I put a new VESC (4.12 with FW 2.18) on my board. I noticed a problem though.

ON BENCH: when I trigger the remote (PPM with current no reverse with brake) in order to brake, the drive apply the mechanical resistance only when the wheel is not spinning anymore. I noticed it because after the wheel stopped, I made it spin again with my hand and I felt a resistance only after some revolutions (I kept the remote on "braking" all he time while trying this)

ON STREET: with my weight on the board I can definitely feel that it start braking after a relevant delay and, most important, when I give throttle again I experience the same delay.

At first I thought that I had to change the batteries of the remote, but when reading the data of the VESC I could see that the PPM percentage was perfectly synced with my actions on the remote.

I tried looking for a solution but I couldn't really find anything suitable to my case.
Did anyone of you experienced something similar?
```

---
## \#2 Posted by: Grolletje Posted at: 2017-11-11T20:25:42.149Z Reads: 54

```
I lately saw a video from a guy with sort of the same problem, he adjusted a setting in the ppm menu with a significantly shorter delay time than the set time. 

maybe this is your problem too
```

---
## \#3 Posted by: carletto Posted at: 2017-11-12T14:57:30.090Z Reads: 33

```
UPDATE
Checking at the online plot I noticed that the VESC report the OVER VOLTAGE error. 

Does anyone have an idea about what could be the cause?
(Battery voltage = 41 V, Vesc maximum input voltage = 41,5 V)
```

---
## \#4 Posted by: Deckoz Posted at: 2017-11-12T15:26:42.200Z Reads: 28

```
Series connection loose
```

---
## \#6 Posted by: carletto Posted at: 2017-11-12T17:13:51.804Z Reads: 20

```
connections among battery's cells or you mean between the battery pack and the vesc?
```

---
## \#7 Posted by: Deckoz Posted at: 2017-11-12T17:35:41.868Z Reads: 17

```
Yes. If your getting over voltage during braking and have checked everything possible. More then likely a series connection of the batteries is broken and it works fine on the bench but when you put load on it(riding with weight) the connection not strong enough for the amperes
```

---
## \#9 Posted by: carletto Posted at: 2017-11-12T17:46:58.889Z Reads: 14

```
Even on the bench is not working properly. That's how I found out of the that the VESC was in error.
Actually I think that when the board is loaded the higher inertia masks this problem a little bit.
```

---
