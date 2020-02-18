# Need help for best setting dual e-mtb

### Replies: 34 Views: 1178

## \#1 Posted by: celica39 Posted at: 2018-02-09T21:08:33.683Z Reads: 177

```
hi there i just finish  my mountain board today (new motor mountings ) 
i need some help to  set my vesc 4.12  to the best value to reduce heat  so here my set up 
14 teeth to motor and 48 for  my 8inch wheel  (yes l know i can use 10 teeth but i want to keep some top speed )
6s 2x 16ah 15c
2x sk3 192kv
4.12 vesc with 2.18 firmware
ppm remote  and bluetooth  with  app

To keep things simple i just need the minimum information to have a safe ride experience with good brake and smooth acceleration and reduce chance of overheat my esc , some talk about erpm max  , but at 6s i dont think its a problem to set it at lower value , also i have tried the traction control but it doesnt seem to work with 6s because of less power at the wheel  but here i have snow and if this feature can help me to limit the spinning it will be great to use it thanks everyone

motor max 60a 
motor min 60a
batt max 60a
batt min 10a
absolute max 130

sorry my weak english , i can also try to upload screenshot thanks
```

---
## \#2 Posted by: Namasaki Posted at: 2018-02-10T04:48:55.553Z Reads: 152

```
These are the settings I run on my dual drive street boards running 10s 5ah 60C Lipos.

Motor max 80a
Motor min -40a
Batt max  50a
Batt min  -10a
Absolute max 140a
```

---
## \#3 Posted by: Eboosted Posted at: 2018-02-10T05:19:23.856Z Reads: 140

```
That would be too slow for my taste, at 6s you will have a top speed of 38km/hr my bet is the performance will wear out pretty fast on you and will leave you wanting for more with a subpar esk8 experience.

I'd get at least an 8S to 51km/hr and much wider powerband. 

You are going to be runing only 22.2V nominal and 25.2V at full charge, I'm not sure if your battery could handle 60A of discharge for each vesc
```

---
## \#4 Posted by: Jebe Posted at: 2018-02-10T06:10:39.727Z Reads: 130

```
More voltage, less amps required = longer running times and battery life
```

---
## \#5 Posted by: celica39 Posted at: 2018-02-10T17:16:04.989Z Reads: 123

```
i already run  32ah 6s this set up for a while  but i can also series to 12s but i don't need such speed thanks
```

---
## \#6 Posted by: celica39 Posted at: 2018-02-10T17:17:27.699Z Reads: 123

```
yes l know but at 12s is too fast for me thanks , since 'bigboytoys' past away l realized it can happen to me to so i prefer run slower but with range
```

---
## \#7 Posted by: FredrikHems Posted at: 2018-02-10T17:41:48.563Z Reads: 122

```
You will have the same range at 12s 16Ah as 6s 32Ah, if not more..
```

---
## \#8 Posted by: celica39 Posted at: 2018-02-10T18:06:39.659Z Reads: 123

```
but theses are the 4.12 version and l have  read they burn  with too much voltage
```

---
## \#9 Posted by: FredrikHems Posted at: 2018-02-10T21:09:25.718Z Reads: 111

```
Most people can run them at 12s without problems.. Remember that you can «burn» them up at 6s too, as you will be pulling a shit ton of current/amps ..
```

---
## \#10 Posted by: celica39 Posted at: 2018-02-10T21:16:42.907Z Reads: 102

```
yes you right!!! but if it can help reduce the amps draw it will solve heat problem too 
but if  i need to find in the bldc app a feature reduce my top speed to 25mph 
please anyone?
```

---
## \#11 Posted by: FredrikHems Posted at: 2018-02-10T21:31:23.018Z Reads: 100

```
You can do some math and set a max erpm to limit you max speed. If you post all your specs I can do the calculations for you :wink:
```

---
## \#12 Posted by: celica39 Posted at: 2018-02-10T22:36:58.916Z Reads: 100

```
ok here its what i have on my hand  for 12s

14 tooth motor and 48 for wheel with 8inch tires

Or  with 10 tooth pinion motor with 48 tooth wheel  with 8inch tires

dual  sk3 192kv

4.12 vesc with 2.18 firmware

ppm remote and bluetooth with app
```

---
## \#13 Posted by: FredrikHems Posted at: 2018-02-10T23:09:16.181Z Reads: 96

```
You shold be using the 10t for a better reduction ratio.. 192kv * 44.4v = 8524 rpm’s at the motor. 
8524/4.8 = 1775 rpm’s at the wheel.
200mm * 3.14= 628mm per revolution of the wheel. 
628mm* 1775= 1 114 700 Mm per minute 
1 114 700Mm\1000= 1114 m per minute.
1114m\60= 18.56 m per sec
18.56*3.6= 66 km per hour. 
Now, this will roughtly be your top speed with a erpm of 59 668.. 

Now, since 66km/h will be your top speed, we say that is 100%.. 
25kmh/66kmh= 37% 
59668/100*37= 22000..

And there you go! Limit your erpm to 22000, but make sure to uncheck «limit with negative torque», and you should not reach more than 25 km/h. 

However, it would be more efficient to have lower kv motors, but oh well.
```

---
## \#14 Posted by: celica39 Posted at: 2018-02-11T05:02:04.070Z Reads: 85

```
thanks for the math ! is 
but 25km/h is too  slow my top speed was 39km/h at 6s and 45km/h  will be just fine at 50volt for me
```

---
## \#15 Posted by: FredrikHems Posted at: 2018-02-11T08:03:09.995Z Reads: 83

```
Oh Sorry, I read 25 kmh instead of 25 mph. Set a Max erpm of 35000 for 40kmh/25mph, or 40000 for 45kmh. :smiley:
```

---
## \#16 Posted by: celica39 Posted at: 2018-02-11T17:23:57.904Z Reads: 77

```
lol not problem  the calculation are for 10 tooth or can be use with the 14 tooth as well ? I found  also on my android app a speed limiter but did'nt try for now , my present project is build traction edge with some cutting tire and stud for the winter condition here , l think i will post a some picture about this soon so thanks   for the help 
 Frederik
```

---
## \#17 Posted by: FredrikHems Posted at: 2018-02-11T17:41:02.463Z Reads: 73

```
You will Get a little more speed with the 14T, but you should use the 10T for better performance, AS your motors are pretty high kv
```

---
## \#18 Posted by: celica39 Posted at: 2018-02-11T21:23:49.606Z Reads: 70

```
less energy spend at the start with the 10 tooth  i guess
```

---
## \#19 Posted by: FredrikHems Posted at: 2018-02-11T21:27:05.108Z Reads: 68

```
Not only at the start, but really whenever you are using power ;)
```

---
## \#20 Posted by: celica39 Posted at: 2018-02-11T22:34:11.145Z Reads: 66

```
drift!!:smile:
```

---
## \#21 Posted by: Lambjr088 Posted at: 2018-02-12T05:15:33.247Z Reads: 57

```
@FredrikHems where can I find these formulas to calculate my speed needs? Can you post them on here?
```

---
## \#22 Posted by: Der6FingerJo Posted at: 2018-02-12T07:00:46.397Z Reads: 59

```
You can use websites like [calc.esk8.today](http://calc.esk8.today) that does all of the calculating for you.
```

---
## \#23 Posted by: celica39 Posted at: 2018-02-12T16:57:20.884Z Reads: 59

```
thanks ! but yes i already use the calc in the past   but i was there to search the best setting for the vesc with 8inch wheel is very different from the 90mm skateboard from most people on this forum
```

---
## \#24 Posted by: celica39 Posted at: 2018-02-18T22:04:38.540Z Reads: 44

```
Hi fred , can you tell me about erpm setting . l have this in my ppm configuration and one in motor configuration thanks
```

---
## \#25 Posted by: FredrikHems Posted at: 2018-02-18T22:09:16.730Z Reads: 47

```
I am not 100% sure on what you mean.. Do you mean that there is 2 places to enter the max erpm?
```

---
## \#26 Posted by: celica39 Posted at: 2018-02-18T22:25:08.083Z Reads: 50

```
Yes there 2 place
```

---
## \#27 Posted by: FredrikHems Posted at: 2018-02-18T23:56:33.573Z Reads: 49

```
Mhm.. I am not an expert at the vesc, so I guess you will have to ask some others.. 
@JohnnyMeduse might know?
```

---
## \#28 Posted by: E1Allen Posted at: 2018-02-19T08:09:35.357Z Reads: 52

```
![IMG_4186|281x500](upload://cFAX0ZwpbIbXoAgvQCKy7mszPm9.jpg)

This one. But where that check mark is make sure it's unchecked. If you leave it checked like the picture it will apply brakes when it hits the RPM limit which is bad when you're moving fast.
```

---
## \#29 Posted by: celica39 Posted at: 2018-03-28T22:50:48.423Z Reads: 40

```
Thanks you sorry for my late reply! And what beautiful place you live! Its my dream to go there and maybe never come back to canada 😂  so if i set a lower value the top speed will also reduce ? Thanks
```

---
## \#30 Posted by: E1Allen Posted at: 2018-03-28T23:21:27.034Z Reads: 39

```
Yes. The lower the erpm it will limit your top speed
```

---
## \#31 Posted by: celica39 Posted at: 2018-03-29T00:08:07.828Z Reads: 41

```
![Capturegjj|690x403](upload://70uFixPsNPGVPemeH1idrCoIgu5.PNG)
```

---
## \#32 Posted by: E1Allen Posted at: 2018-03-29T04:13:34.718Z Reads: 37

```
Yeah. Make sure you set it for both vesc.  Test to see how top speed is then change if necessary
```

---
## \#33 Posted by: MannyM0E Posted at: 2018-03-29T04:39:38.491Z Reads: 37

```
[quote="Namasaki, post:2, topic:45984"]
se are the settings I run on my dual drive street boards running 10s 5ah 60C
[/quote]

Are these split in half for each motor ? Or do you put this setting per motor ?
```

---
## \#34 Posted by: Namasaki Posted at: 2018-03-29T11:48:30.884Z Reads: 31

```
I run those settings on each motor.
```

---
