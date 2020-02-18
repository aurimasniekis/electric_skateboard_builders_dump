# Motor cogs during speed

### Replies: 21 Views: 1014

## \#1 Posted by: abctheing Posted at: 2017-08-17T11:59:05.525Z Reads: 111

```
Hello, i sorta finished my first build, but i have a huge problem.

Throttling from standstill works fine, but of course the motor will cog a little bit when i do that, because of the weight on the motor.

But if the board is rolling downhill and i don't touch the throttle, meaning 0%, as soon as i accelerate the motor will cog and throw me off. The board will instantly stop and make screeching sounds. The same thing happens if i brake, but not always. The brakes usually work just fine, but sometimes the brake won't respond until i brake a lot, then the board stops and cog. When i'm going downhill the brakes sometimes stop working aswell, basically the brakes completely die. If i jump off the board and throttle a bit forward, the brakes will work again. The cogging only happens when i'm not touching the throttle, meaning if it's at 0% throttle and i move the thumbstick in either direction. Sometimes i can throttle from standstill and if i keep the board at speed then brake, the brakes will work just fine, but If i then start to accelerate again, the board will stop and cog.<img src="/uploads/db1493/original/3X/7/a/7aa493c3db0af1a1118d0dc3b874c3d1d7805d60.png" width="690" height="364"><img src="/uploads/db1493/original/3X/6/f/6f348d9f21de69ef0ab668b4c50af54b303fb9f1.png" width="690" height="362"><img src="/uploads/db1493/original/3X/a/6/a660f018e403ed6a849dd40078dd65ad224d221a.png" width="690" height="365"><img src="/uploads/db1493/original/3X/4/f/4f756278528f681b02c4e33374fa719c53b810ac.png" width="690" height="364">
```

---
## \#2 Posted by: Ishayc Posted at: 2017-08-17T12:30:43.632Z Reads: 91

```
Share some info about your gear.. Battery, Motor etc
```

---
## \#3 Posted by: darkkevind Posted at: 2017-08-17T12:36:33.663Z Reads: 88

```
It sounds like you haven't done, or didn't apply a motor detection.
```

---
## \#4 Posted by: abctheing Posted at: 2017-08-17T12:41:55.505Z Reads: 85

```
Yes, i'm using a torqueboards 6374 motor. 36/13 gearing i THINK. I use a 50 volt 18650 battery, 9450 mah. Built it myself. I use the enertion vesc-x. I'm also using the winning remote. Orangatang kegel wheels.
```

---
## \#5 Posted by: abctheing Posted at: 2017-08-17T12:42:15.651Z Reads: 79

```
Hmm i have done the detection and hit apply, is there more to it?
```

---
## \#6 Posted by: darkkevind Posted at: 2017-08-17T12:45:08.501Z Reads: 76

```
Were the VESC-x's capable of 12s?
```

---
## \#7 Posted by: darkkevind Posted at: 2017-08-17T12:45:30.105Z Reads: 75

```
Did you write config after that then reboot VESC?
```

---
## \#8 Posted by: abctheing Posted at: 2017-08-17T12:46:17.949Z Reads: 75

```
Yes it's capable of 12s and i did write and reboot.
```

---
## \#9 Posted by: Ishayc Posted at: 2017-08-17T12:47:49.528Z Reads: 73

```
What is your motor KV? It needs to be 170kv max in order to stay within the erpm 60000 limit
```

---
## \#10 Posted by: abctheing Posted at: 2017-08-17T12:55:06.549Z Reads: 68

```
It's 190 KV. What erpm are you talking about? I could also say that when i try to spin the motor with BLDC, it just makes a clicking sound, it won't spin.
```

---
## \#11 Posted by: Blasto Posted at: 2017-08-17T12:55:15.296Z Reads: 69

```
Try this

Motor max 80
Motor min -40
Batt max 40
Batt min -15

But it does sound like your hitting your set erpm limit
```

---
## \#12 Posted by: Ishayc Posted at: 2017-08-17T12:58:29.424Z Reads: 67

```
You set the erpm values to 60000. 
If you have 190kv and 12s it means - 
12*4.2[v]*7[poles]*190[KV] =~ 67,000.

Try checking the "hit erpm with negative torque" check box and try again, it might help.
```

---
## \#13 Posted by: abctheing Posted at: 2017-08-17T13:03:53.029Z Reads: 64

```
Ok i put BR ERPM to 60000,00.

But this happens when i do calibration: https://www.dropbox.com/s/7fe5pjhn7m1chd9/IMG_3884.MOV.mov?dl=0
```

---
## \#14 Posted by: Ishayc Posted at: 2017-08-17T13:07:04.906Z Reads: 61

```
Hmm, Its seems like the motor loses it's poles position for some reason.
```

---
## \#15 Posted by: Blasto Posted at: 2017-08-17T13:10:37.706Z Reads: 60

```
Slightly increase your low duty at detection to about 0,1... but shouldnt make a difference in the parameters received
```

---
## \#16 Posted by: abctheing Posted at: 2017-08-17T13:14:26.009Z Reads: 62

```
Wow thanks, it works! But what does the Min ERPM really do? It's at 850 now.
```

---
## \#17 Posted by: toma Posted at: 2017-08-17T13:15:12.098Z Reads: 61

```
My guess is you've got a loose connection. Perhaps you haven't done motor detection. Do you have hall sensors or not?
```

---
## \#18 Posted by: abctheing Posted at: 2017-08-17T13:15:32.461Z Reads: 61

```
No it's sensorless
```

---
## \#19 Posted by: Jinra Posted at: 2017-08-17T13:52:50.113Z Reads: 57

```
[quote="Ishayc, post:12, topic:30874"]
Try checking the "hit erpm with negative torque" check box and try again, it might help
[/quote]

that's how you street your face
```

---
## \#20 Posted by: Ishayc Posted at: 2017-08-17T15:16:05.098Z Reads: 46

```
Hmm Then I probably got it wrong
```

---
## \#21 Posted by: abctheing Posted at: 2017-08-18T11:58:49.559Z Reads: 36

```
Ok, so the board rode fine today, but the belt broke :( I couldn't get the drive wheel pulley centered, i tried for many hours to get it right. But when the board goes downhill and i brake, the board will brake fine but the motor will make a screeching sound. I am a bit worried and the screeching sound makes people look.
Is there any settings that can stop the sound?
```

---
