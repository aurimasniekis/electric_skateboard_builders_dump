# VESC - Current No Reverse With Brake - rapid acceleration

### Replies: 17 Views: 490

## \#1 Posted by: Ukesu Posted at: 2018-08-08T18:15:42.097Z Reads: 110

```
After many, I mean many attempts I lost all hope.

Current No Reverse With Brake mapped, center set, but when I accelerate there is no relationship between how much I move my acceleration and how fast motors are going. And motors starts to spin to 100% on 15% from controller. I tried so much settings with Pulselenghtand anything changes it even a bit :(

On Duty Cycle its working well but I got other problems on this control type so I want to stick to Current control.
Can you help me ? :)

![vesc|690x389](upload://u5isCpRGcXk7Sm48iCiqq3FSt5g.png)
```

---
## \#2 Posted by: Lionpuncher Posted at: 2018-08-08T18:16:50.196Z Reads: 101

```
Which remote are you using?
```

---
## \#3 Posted by: Ukesu Posted at: 2018-08-08T18:17:30.918Z Reads: 96

```
Nano X from Enertion
```

---
## \#4 Posted by: DeathCookies Posted at: 2018-08-08T18:21:20.182Z Reads: 93

```
I think the nanox works better with the Standard r2 Firmware.
When i used it with acks Firmware i fine tuned the throttle curve a lot to decrease the Power on Low speed.
Btw i like Index Finger Controll more because the throttle way is longer and thus preciser
```

---
## \#5 Posted by: mccloed Posted at: 2018-08-08T18:24:11.310Z Reads: 91

```
Are you just bench testing or are you riding the board when this happens? The speed will be variable with load on any vesc.
```

---
## \#6 Posted by: Sender Posted at: 2018-08-08T18:27:54.814Z Reads: 87

```
Also with the nano x:

Turn on remote, go full throttle then full brake

THEN turn on board
```

---
## \#7 Posted by: Ukesu Posted at: 2018-08-08T18:27:55.428Z Reads: 82

```
Bench test, but on duty cycle there was no rapid acceleration :/
Now I a little bit scared to test in with load because I do not want to my board fly off.
```

---
## \#8 Posted by: TowerCrisis Posted at: 2018-08-08T18:31:39.238Z Reads: 78

```
That is expected behavior on a bench test. There's very little resistance so it can't pull very many amps before it reaches top speed.
```

---
## \#9 Posted by: Ukesu Posted at: 2018-08-08T18:32:19.280Z Reads: 80

```
I tried, not working ;(
```

---
## \#10 Posted by: Ukesu Posted at: 2018-08-08T18:33:55.937Z Reads: 79

```
Hmm, i will try to check it on load :slight_smile:

Now it looks like this:
https://www.youtube.com/watch?v=zkrlPJHiRZU
```

---
## \#11 Posted by: TowerCrisis Posted at: 2018-08-08T18:40:58.047Z Reads: 73

```
If you've tried to tune it to work on a bench test it won't work well under load. Make sure the full stroke is mapped to the vesc.
EDIT:
My bad, just connect the belt and it will work fine. I couldn't see that it wasn't on viewing on my phone.
```

---
## \#12 Posted by: AutoItKing Posted at: 2018-08-08T18:43:24.200Z Reads: 72

```
It's working exactly as it should. Current mode is more like the throttle in your car. If you give your engine 15% throttle in neutral it'll rev high, but under load it won't.
There is absolutely nothing wrong here, just a lack of understanding.
```

---
## \#13 Posted by: skatardude10 Posted at: 2018-08-08T19:28:43.649Z Reads: 63

```
This is the answer. Nano X needs calibration every time you turn it on. 

Turn on remote, blinking light.

Full throttle, full brake, full throttle, full brake.

Turn on board, blinking light goes solid.

Now your remote will function normally, 15% throttle will equal 15% now instead of 100% and same for brake.

Had the same issue myself for weeks until I realized this. Remote on before board with full throttle full brake.
```

---
## \#14 Posted by: AutoItKing Posted at: 2018-08-08T19:32:29.447Z Reads: 55

```
You are correct, but that's not the problem here. 15% throttle will net 15% speed only if in duty cycle mode. Current mode behaves very differently. It is doing exactly what it should.

If you look at his screen shot you will see that he has 14% throttle but 95% duty cycle. This is because of current mode. NOTHING IS WRONG.
```

---
## \#15 Posted by: DeathCookies Posted at: 2018-08-08T19:34:58.593Z Reads: 57

```
I dont think that you need to calibrate the remote in every ride. You can turn the Board on and then the remote. This way you dont need a recalibrate and you will use the old settings
Correct me if i am wrong
```

---
## \#16 Posted by: skatardude10 Posted at: 2018-08-08T19:40:44.260Z Reads: 54

```
For other remotes maybe (haven't tried) but it's known for the nano X in particular you do have to do this "calibration" routine full throttle and full brake before connecting to the vesc to have proper functionality when the board is turned on. 

Otherwise your initial 15% throttle will = 100% throttle... Which is very jarring. Another option if you turn your board on first is to still just go full throttle full brake... Just spinning your wheels instead... Your remote will work properly after this... With a nano X just don't not calibrate your remote and hop on straight away or your throttle and brake will be hyper sensitive until you use full range of motion at least once.

Still, seems this may not be OPs issue, I'm leaning to agree with @AutoItKing's assessment of the situation... No load is very different than load. Just properly map your pulsewidths minimum, center and maximum values in vesc tool to = -100% / ~-0.5 - 0.5% /  100% output from ESC respectively, calibrate your nano-X full throttle and brake, turn on board and test with a load. Should be fine.
```

---
## \#17 Posted by: Ukesu Posted at: 2018-08-08T20:03:49.793Z Reads: 49

```
Tested on load and it is better but still very aggressive. ![38744346_302393763841499_3131369752530780160_n|259x500](upload://qRcYZiEcThQZSiTxWWRJaqXnWHO.jpg)
```

---
