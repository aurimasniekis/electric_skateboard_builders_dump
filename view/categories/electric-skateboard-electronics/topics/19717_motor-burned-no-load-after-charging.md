# Motor burned (no-load) after charging

### Replies: 3 Views: 438

## \#1 Posted by: Radino Posted at: 2017-03-26T15:29:47.045Z Reads: 80

```
Hello,
 yesterday I tested my board until battery turned it off (esc cut off voltage?), then I was charging with Imax B6 (that was like 3th charging), After 2hours of charging 1 battery cell was about 3,64 V other 4.17~4.2 V (2hours safety shut down by Imax charger), today at morning I stared charging again, that cell went up to 3.82V then charging was completed (after 12mins). Then I went to try if everything is fine, I flip the board over (wheels up), start it on and then I pull the trigger, the sound of motor was different, I released trigger and after motor stopped I pulled trigger again and motor started smoking, cables were hot a little, after that I saw only sparks in my motor. 

Now I don't know what caused the damage, motor itself, battery, ESC or just bad luck.

Spec:
motor: KEDA A63S/28 - 250kv (63x56mm) (prop. I bought last motor from that e-shop)
ESC: SUNRISE Model 100A SBEC- 6A
Charger: Imax B6AC 50W
Battery: 5200mAH 6s 30C (60C)

Thank you very much for any help or suggestion.
```

---
## \#2 Posted by: saul Posted at: 2017-03-26T16:13:25.662Z Reads: 69

```
It was probably a bad idea to that. Or any ESC be your only battery protection. 

On a vesc you can set the cut off high enough that your packs should be safer but rc escape usually discharge way down to 3v or lower.
But if a cell was a bit lower than the others, it could drop below this and cause damage. Sounds like that's what happened here. Which means that cell is not safe to use anymore.

I'm repacking 4 sets of 6s into 4 of 5s because of a similar situation.  Lucky the numbers worked out. 
Get a low voltage buzzer. The 8s one from HK is good. Adjustable cutoff .1 3-3.8 or something.

The battery going crazy with a current spike could have made trouble. All bad luck in the end. Try for warranty if you can!

Also I was curious about that motor! Was it pushing good before that?
```

---
## \#3 Posted by: Radino Posted at: 2017-03-26T20:11:19.691Z Reads: 43

```
Hi, starts without pushing were hard, but sometimes it worked just needed to play with trigger. Then everything was smooth.
Thanks for your opinion. I bought e-shop battery but I made it to flat, 1 cell was different, like air inside... battery was most expensive I thought I payin for quality... at that price I would have turnigy 12 cells from hobbyking...
```

---
