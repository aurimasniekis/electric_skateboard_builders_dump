# Newbie: Few questions about electronics

### Replies: 22 Views: 1043

## \#1 Posted by: TunaTee Posted at: 2017-09-13T04:11:48.477Z Reads: 116

```
Hello guys,
Sorry that I gotta bother you.

I got 3 packs of 3s1p 5000 mAh zippy LiPo batteries.
I got a 190kv 6355 motor and a VESC from TORQUE.

1. Shall I do a serial or parallel connection? I know that serial gets you more voltages thus draws more power and parallel gives you the same voltage while higher capacity thus longer ride. 

2. Do I use an anti-plug while trying all these? I got a power button that I got from Luna Cycle it should work as an anti-plug I believe.

3. I got a battery capacity monitor where should I put the wires on? It has a black and a red wire. The instruction says to put it on to the battery but I am not really sure.
```

---
## \#2 Posted by: onepunchboard Posted at: 2017-09-13T04:19:12.947Z Reads: 111

```
1st question. go with series. if u dont go full power all the time u will get similar range.
```

---
## \#3 Posted by: TunaTee Posted at: 2017-09-13T04:26:00.242Z Reads: 108

```
So do I configure the vesc setting so that the motor does not exceed certain rpm to get the similar range?
```

---
## \#4 Posted by: onepunchboard Posted at: 2017-09-13T04:27:09.909Z Reads: 102

```
no u just pull less trigger. u may want to set erpm tho btw 60k to 65k. many recommend 60k
```

---
## \#5 Posted by: onepunchboard Posted at: 2017-09-13T04:28:35.318Z Reads: 97

```
batt life come down to whr not mah. v x mh = wh
```

---
## \#6 Posted by: capfirepants Posted at: 2017-09-13T04:35:47.158Z Reads: 92

```
1) series.
2) can you show us what this looks like? Never seen it before (btw. The correct term is Anti-Spark plug. Not trying to be a dick but fyi)
3) I put mine juat before the vesc, red wire to red vesc wire, black vice-versa.
```

---
## \#7 Posted by: TunaTee Posted at: 2017-09-13T04:39:00.345Z Reads: 82

```
I am just doing all these researches before putting up my electronics. They are lying on my table. I am afraid to put them incorrectly to cause a fire hazard.
```

---
## \#8 Posted by: capfirepants Posted at: 2017-09-13T04:40:29.252Z Reads: 78

```
Fire hazard is one thing, breaking them (mostly the vesc) another. Before you plug anything in, post a few good, detailed pictures here if you wanna be sure.
```

---
## \#9 Posted by: TunaTee Posted at: 2017-09-13T04:42:25.861Z Reads: 76

```
Thanks. Will do.
```

---
## \#10 Posted by: TunaTee Posted at: 2017-09-14T02:09:14.739Z Reads: 67

```
Hey capfirepants, can I ask you something.
So I should connect my batteries in series not in parallel, but what are the results of connecting them in series and in parallel. I have watched about 3 youtube videos but still could not get it.
```

---
## \#11 Posted by: Bloop Posted at: 2017-09-14T04:59:00.129Z Reads: 59

```
Hey if you have 3x 3s1p and connect them in series you will get a total of 9s1p. 

In paralel you would get 3s3p and this is not enough, The minimum requirement for vesc/motor is 6s.

So you know how to connect them? Also for battery and in general all electronics i suggest you to get a sheet of paper and draw the components and how you think they will get connected and post the pics here to be sure everything is alright.
```

---
## \#12 Posted by: pat.speed Posted at: 2017-09-14T13:02:59.113Z Reads: 51

```
If you connect the batteries in series you will increase the voltage and if you connect them in parallel you will increase the mag the battery has. So if you have one 3s lipo that has 3 cells in it. Each cell is 3.7v nominal and 4.2v when fully charged. So if you have 3 cell in each lipo each pack will be 11.1v nominal and 12.6 fully charged. Now if you connect three of those packs in series you will get 33.3v nominal and 37.8 fully charged, get it? 

But if you connect in parallel you will increase the mah. So each 11.1v lipo has lets say 5000mah if you connect three together you will have 15000mah and still only 11.1v. 

The last thing to know is that it doesn't matter which way you connect them, they will always give the same range just with different top speeds. This is because the Watt Hours of the pack are the same. If you have 3 of the lipos in series to give 37.8v the pack will only be 5000mah still so it will have a watt hour rating of 33.3v x 5a = 166.5 Watt hours. If you have the three batteries in parallel it will be 11.1 and 15000mah. So 11.1v x 15a = 166.5 Watt hours. 

I hope this makes thing clear
```

---
## \#13 Posted by: TunaTee Posted at: 2017-09-15T03:40:05.913Z Reads: 43

```
<img src="/uploads/db1493/original/3X/e/9/e9f249b6647bf1fff1decf4b99e9219f8a56a9d2.png" width="690" height="444">
I am planning to series them in this way.
```

---
## \#14 Posted by: TunaTee Posted at: 2017-09-15T03:40:31.977Z Reads: 42

```
Thanks for your explanation, now it makes much more sense.
```

---
## \#15 Posted by: Bloop Posted at: 2017-09-15T04:13:43.982Z Reads: 43

```
from second battery you can connect directly to the third.

You should have something like: 1st battery - connected to 2nd battery + . 2nd battery - connected to 3rd battery + then 1st battery + with 3rd battery - connected to an XT60/90 connector. and you should be fine. 

Also don't forget about balancing wires for each battery. How you planning to recharge your batteries??
```

---
## \#16 Posted by: TunaTee Posted at: 2017-09-15T17:01:39.021Z Reads: 42

```
Thanks for the instruction. Appreciate it.
I am planning to charge each of them separately. 
Can I ask some questions: 
1. Is there a better way to charge?
2. Also, you know there is a white connector sticking out, do you know what is that for?or do i just leave it hanging?
3. Also for the motor there is a white connector, does it have to go to the vesc?
4. I got a battery capacity monitor, do I solder them into the battery + and -?
Sorry, totally noob to electronics and I do not think many youtubers illustrated on that.
```

---
## \#17 Posted by: Bloop Posted at: 2017-09-15T17:51:18.175Z Reads: 40

```
is better to post pictures easier to understand what you mean.

1. The best way to charge your batteries is with a bms. It will make sure your cells are charged equally.
You can also use a lipo charger (hobbyking has many)  just need to find one to fit your battery pack. Usually the hobby king chargers are 6s  (the ones not that high on $$$) 

2. The white connector from the battery should be the balance wires so you will need to connect them to bms or the charger to keep your cells balanced

3. the motor has some wires except the 3 faze wires they must be the sensor wires that you will need to connect to the vesc if you want to run sensored / else you can leave them

4. yes you can connect it to the battery + and - i saw some people connecting it near the vesc terminals .
```

---
## \#18 Posted by: TunaTee Posted at: 2017-09-15T21:11:55.550Z Reads: 34

```
<img src="/uploads/db1493/original/3X/8/f/8f28ffab433a6c4c602b4b1da88d1edd3e3e2ed7.JPG" width="375" height="500">
This is my final build. 
<img src="/uploads/db1493/original/3X/6/f/6f40c28cc7ea62af0b2ebb399522fe0fafcd6900.JPG" width="375" height="500">
Im going to use the red wire from the first battery and the black wire of my 3rd battery to power the motor.

Is there any problem to put my battery on top of each other? Will they get overheated after a long ride?
```

---
## \#19 Posted by: Bloop Posted at: 2017-09-15T22:36:59.126Z Reads: 31

```
Batteries will be fine you will have to be carefull not to discharge them too much i mean vesc limits will help too.

Also have you figured a way to charge your batteries.? 

Nice build i like it :D my first build is full of ductape yet to add my enclosure.
```

---
## \#21 Posted by: TunaTee Posted at: 2017-09-18T23:31:43.769Z Reads: 25

```
Hey Bloop, I just got all my components needed to charge the battery lol.
I am using a Lipo balance charge and charging my 3s 5000mah battery at 5A.
I should stop the charging process when the voltage goes up to 12.6 correct?

Also, I am considering getting a BMS to charge my 3 3s Lipo battery because this plug and unplug process for each battery is just intimidating:)
```

---
## \#22 Posted by: Bloop Posted at: 2017-09-19T01:33:57.296Z Reads: 20

```
if you have a charger for lipos then you shouldnt need to worry about when yo stop. It will start beeping when is full. You only need to se it up right like the A you are chargin and the nr or series and connect the balance leads then you are good to go
```

---
## \#23 Posted by: TunaTee Posted at: 2017-09-19T02:22:40.738Z Reads: 21

```
I got everything set up nicely. Thanks for your help along the way :slight_smile: 
It is weird that I have to connect my remote control in CH1 to function. In the video, it says that I have to connect to CH2.
Well, the only problem at hand is that I cannot find a MINI USB CABLE!!!!!!! Haha, I thought I should have one somewhere in my house but couldn't find one when I really needed it.
```

---
