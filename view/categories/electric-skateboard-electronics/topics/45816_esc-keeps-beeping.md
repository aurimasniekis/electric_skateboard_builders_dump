# ESC keeps beeping

### Replies: 17 Views: 2681

## \#1 Posted by: jimmaskell Posted at: 2018-02-07T16:16:46.269Z Reads: 139

```
One day when I started my electric skateboard I kept beeping after I turned it on. It is the ESC that is beeping, but I do not know why it keeps beeping. It is a repetitive beep, which sounds the same as when you turn on the ESC.

Here is a photo and a link to the ESC.
![image|499x500](upload://kvoOgzW1h6plw40ACdDb2lqpr27.jpg)![ESC|499x500]

https://www.ebay.com/itm/Single-Motor-Electric-Longboard-Skateboard-Controller-ESC-Replace-Control-Modul/322629605298?ssPageName=STRK%3AMEBIDX%3AIT&_trksid=p2057872.m2749.l2648
```

---
## \#2 Posted by: LunarKim Posted at: 2018-02-08T04:51:00.482Z Reads: 112

```
My memory is probably a low voltage alarm. When purchasing 6 cells, you have to set 8 cells, 10 cells, 12 cells.
```

---
## \#3 Posted by: Sk8Board Posted at: 2018-02-08T06:36:49.350Z Reads: 104

```
@LunarKim is right, there are 2 or 3 solder pads that have to be connected or disconnected to determine the correct voltage. It should show on the ebay listing. If that doesn't work, I found if there was a bad connection between the battery and the esc, a high resistance between the two, or batteries can't provide enough amps, then the esc beeps.
```

---
## \#4 Posted by: jimmaskell Posted at: 2018-02-08T08:41:16.609Z Reads: 94

```
Okay thank you! When I tried to connect the bms I got a short, but everything still seemed working, but apparantly I damaged the cells. I guess I have to buy two new 3s LiPo's.
```

---
## \#5 Posted by: b264 Posted at: 2018-02-08T09:01:21.314Z Reads: 89

```
You're lucky the building didn't burn down...
```

---
## \#6 Posted by: jimmaskell Posted at: 2018-02-08T15:40:46.946Z Reads: 80

```
What exactly do you mean by this?
```

---
## \#7 Posted by: SHHHECTER Posted at: 2018-04-13T01:15:19.751Z Reads: 65

```
Sorry men how could you fix this problem? @jimmaskell 
I am having the same problem, with the same anoying sound!
```

---
## \#8 Posted by: aponty Posted at: 2018-04-16T16:01:14.592Z Reads: 56

```
Second this. It's not my battery or the voltage, even with the board upsidedown on my countertop it beeps repetitively every time I hit the brakes.
```

---
## \#9 Posted by: Nordle Posted at: 2018-04-16T16:27:38.957Z Reads: 55

```
How is it? I mean the sound, is it like R2D2 speaking with you? Or just an annoying beep?

Seriously, if everything else is working fine i would just try to desolder the buzzer;)
```

---
## \#10 Posted by: aponty Posted at: 2018-04-17T03:15:11.050Z Reads: 49

```
It's just an annoying repetitive beep. And unfortunately everything isn't working. It doesn't brake, it only beeps (even with both motors disconnected, so it's not a braking-voltage-spike warning), and one motor won't spin at all; it just beeps. So, I've got a quarter functionality I guess- I can go forward with one motor, but not stop haha
```

---
## \#11 Posted by: jimmaskell Posted at: 2018-05-27T18:48:01.519Z Reads: 39

```
Hey man, sorry for the late respond, but I found out that it was a low voltage alarm. that's because I'm using LiPo batteries, which tend to drop in voltage quite fast. So right now I'm looking into a voltage regulator to keep the voltage at a consistent level
```

---
## \#12 Posted by: Superchris Posted at: 2018-05-29T10:03:00.219Z Reads: 38

```

I'm having the exact same problem. Did a voltage regulator do the job for you?
```

---
## \#13 Posted by: jimmaskell Posted at: 2018-05-29T10:09:09.824Z Reads: 36

```
@Superchris No, because all the voltage regulator would do is produce a lot of heat and they are quite expensive for such high amps. Right now I'm gonna try to connect another two 3s in series and those in parallel if that makes sense, so the voltage curve is way nicer and the capacity is twice as big.
```

---
## \#14 Posted by: Superchris Posted at: 2018-05-29T10:16:51.793Z Reads: 33

```
Ok, i'm running 2 4s 5000 mAh in parallel and i can't stop the beeping. Guessing i have incorrect voltage.
```

---
## \#15 Posted by: jimmaskell Posted at: 2018-05-29T14:57:25.446Z Reads: 28

```
@Superchris What voltage is the ESC rated for?
```

---
## \#16 Posted by: Superchris Posted at: 2018-05-30T12:14:18.389Z Reads: 26

```
@jimmaskell
It's rated for 24V, 36V and 48V. That's the problem. 2 4s in parallel is 14.8 V. I thought I could use it anyway, but i might have to buy another ESC.
```

---
## \#17 Posted by: jimmaskell Posted at: 2018-05-30T14:33:06.828Z Reads: 21

```
@Superchris Yeah that's the problem. Maybe you could try to put them in series, but I don't know how the ESC will react to that.
```

---
