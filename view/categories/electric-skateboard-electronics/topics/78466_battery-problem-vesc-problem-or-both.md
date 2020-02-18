# Battery problem, VESC, problem or both?

### Replies: 16 Views: 441

## \#1 Posted by: Fearless562 Posted at: 2018-12-19T20:25:15.378Z Reads: 94

```
Having some issues with my setup. (At the moment I’m running TB Single 6374, 12s4p, and 4.12 VESC. The set up worked fine for months until I installed Bluetooth module from BKB. Then about a week ago I was riding and the board Powered down and gave me a FAULT ABS OVER CURRENT followed by a FAULT ABS UNDER CURRENT reading. This happens several times in a row on my way home from a ride. When I got back home I wanted to plug into my computer and see what was going on. When I tried to power the board back on the bench it would not turn on.... I hooked it up to the charger and it came on reading 85% when I disconnect it however it wouldn’t turn on again until connected to the charger. I unplugged everything And tried to check all the connections which all seemed good. Then when I plugged the VSC back into the battery it’s sparked and blew fried my XT90 connector.  I could barely get them apart but when I did I noticed it was burnt up. I then Soldered on a new male and female XT90 antispark connector to the VESC and battery and tried to plug them in and again my battery won’t turn on.... I disconnected them and Plug the battery into the charger it came on...unplug the charger  and the battery will flip on and off. However when it’s plugged in to the VESC nothing… I’m lost here. Not sure what I should do to Test whether it’s My VESC or my battery causing the issue.  Any advice Is greatly appreciated.
```

---
## \#2 Posted by: Andy87 Posted at: 2018-12-19T20:35:50.051Z Reads: 81

```
Do you use a bms for discharge?
Do you use a loopkey?
The abs over and under current faults you had the one day sound like there was a loopkey not fully plugged in, or a bad connection between your battery and vesc.
Could be that this already damaged something on your vesc and that than resulted in the spark and melting down of your xt connectors.
If you get your vesc powered on, does there blink any red light?
```

---
## \#3 Posted by: Fearless562 Posted at: 2018-12-19T23:33:33.183Z Reads: 70

```
The TB battery has a built in BMS and on off switch and I just plugged it directly into the VESC via the XT90 antispark that it came with. Do I need a loopkey as well?  Im trying to figure out another power source to check it.  I have some 3S LiPo Packs but they use XT60 can I just make an adapter from the XT90 to XT60 and plug it into that?
```

---
## \#4 Posted by: Santino Posted at: 2018-12-20T04:02:52.879Z Reads: 59

```
I would try to use the Lipo, just to check if the Vesc is OK... You could use and adapter...if it powers and shows no problems (red light blink or so), then you know what to do...
```

---
## \#5 Posted by: Andy87 Posted at: 2018-12-20T04:45:39.514Z Reads: 53

```
If I remember right there is a discharge bms in the tb battery. 
A loopkey is never bad, but if you have a discharge bms with e-switch you don’t need a loopkey.
Could be that there is an issue with your bms, or the switch on the bms or all together.
To check the vesc with your lipos is a good idea.
Sure you can make a xt60 to xt90 adapter, that shouldn’t be an issue
```

---
## \#6 Posted by: Fearless562 Posted at: 2018-12-21T00:06:51.607Z Reads: 47

```
 So tried plugging the VESC Into the LIPO  battery and it shorted out the anti-spark XT 60 Loopkey.   TheVESC never turned on obviously. Does this mean the VESC is shot? Looking at it visually it seems normal but I’m not sure exactly what to look for....
```

---
## \#7 Posted by: J0ker3366 Posted at: 2018-12-21T00:12:21.270Z Reads: 43

```
That could possibly be crossed wires somewhere
```

---
## \#8 Posted by: Fearless562 Posted at: 2018-12-24T04:17:39.625Z Reads: 42

```
Where would it be a crossed wire in the VSC or the BMS somewhere?
```

---
## \#9 Posted by: J0ker3366 Posted at: 2018-12-24T04:27:31.859Z Reads: 43

```
Take one of your 3s lipos and plug it straight to the vesc. Nothing else. Probably pop a small bit but nothing to worry about as youre only doing it once or twice. What your looking for is if the vesc will power on by its self. If the lights come on then you know your vesc is ok. 

Next you add in the bms. Pull the jst as you're only wanting to see if the bms is operational. Wire in the bms to the lipo and vesc. If the vesc lights up, you know the bms is good. 

Process of elimination. If after everything works with the lipo, I'm willing to bet its in the battery.
```

---
## \#10 Posted by: Fearless562 Posted at: 2018-12-24T22:24:17.087Z Reads: 37

```
Ok. The 3s lipo has an XT60 and and the VESC has an XT90. I made an adapter. Should I use that or just attach a Xt90 to the lipo or Vice versa. Whenever I plug it in it’s not a little spark it’s enough to weld the two plugs together I have some pictures of the connectors after plugging them in and also the adapter I made... thanks for the help I appreciate it. [image|666x500](upload://4d7umqQwDhlr8ZxzPSPTcK11uhG.jpeg) ![image|375x500](upload://rqgYvtDkshq4bbT2niKSbHJJ1sM.jpeg) ![image|375x500](upload://7xo1PGFa2l9FzEgHGdCs9s5PAXy.jpeg)
```

---
## \#11 Posted by: TowerCrisis Posted at: 2018-12-24T22:30:12.635Z Reads: 33

```
Well that's bad. I've done that once, it happened after one of my vesc's went to a dead short and I melted my loop key.

Show us your vesc, the battery, and the adapter all in one picture (disconnected obviously)
```

---
## \#12 Posted by: Fearless562 Posted at: 2018-12-25T02:14:04.421Z Reads: 33

```
![image|666x500](upload://cgf5ACfSaiyCXTa9LgOOyw1eFju.jpeg) ![image|666x500](upload://b9RktyEEeYKBJt9fP3jxaYiDrJr.jpeg) ![image|375x500](upload://mgEqUCy5rXuR3DZyvRTJXlT3HGN.jpeg) ![image|375x500](upload://cO2yUYW3RjTwm9VWejdnWdMGCLu.jpeg) ![image|375x500](upload://p9LH0SP5ovFUJJbkmISFuHu05Ud.jpeg) ![image|375x500](upload://uIYbtmqSPEBpZoQMR5hrIN9MwzX.jpeg) ![image|375x500](upload://QjZtEnpFBnVkNYk0XJg6FfIwYJ.jpeg) ![image|375x500](upload://aHodD1RRDLmm9fturI26vemyovR.jpeg) ![image|375x500](upload://hyua1Y53armzastNEaQZC7EfV0j.jpeg) ![image|375x500](upload://iPghf1KwmvXk1WNTwYzlyjO5jer.jpeg)
```

---
## \#13 Posted by: Fearless562 Posted at: 2018-12-25T02:16:13.538Z Reads: 30

```
So I also added some photos of the Vesc.  I took off all of the shrink wrap to get a better look and everything seems ok but I’m pretty new to all of this. Thanks
```

---
## \#14 Posted by: Fearless562 Posted at: 2018-12-28T18:26:27.764Z Reads: 24

```
Anyone see anything wrong with the VESC?
```

---
## \#15 Posted by: CP123 Posted at: 2019-05-11T19:36:14.363Z Reads: 17

```
Hey ive got a question. Ive got this board with a dual esc off of ebay, and 2 3s batteries with a belt driven motors all bought off ebay. It worked awesome for quite some time. I plugged it in to charge it and then i went to ride it again, it wouldnt do anything. The brakes would work, but it wouldnt accelerate. I found that if i push started it, it would go but it was glitching a lot. Like the esc was bad. I replaced the esc with the same model, and it didnt do anything. I replaced the motors thinking it would solve my problem. Still nothing. The only origiinal part is the battery. Do you have any idea whats happening?![Screenshot_2018-11-06-06-19-16|250x500](upload://nhbPAOQ0ZEiQsbEYZ51EQOHg6Ne.jpeg) ![Screenshot_2018-11-06-06-19-21|250x500](upload://rbFXIG22EDApaZURy5JHv1NQ1x5.jpeg)
```

---
## \#16 Posted by: J0ker3366 Posted at: 2019-05-11T19:56:14.887Z Reads: 16

```
Check all your connections. Pay close attention to phase wire connections @ esc, motor and where the two connect between each other. Report back after.
```

---
