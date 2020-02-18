# Optimal Gearing for 125mm gummies?

### Replies: 13 Views: 364

## \#1 Posted by: Resonant Posted at: 2019-03-17T11:03:30.500Z Reads: 162

```
Havent bee able to find much info regarding 125mm gummies and what kind of gearing is necessary to get the speed and torque I want. I am not sure if I can decrease the size of the wheels for increased torque. But what gearing would I need with 125mm wheels running 12 dual 6374s to get a 31-33 mph top speed minimum and very fast acceleration. I had planned this out before but for 97mm wheels not sure what things I need to modify to get the desired specs for 125mm wheels since I have cuanged my plans. Im guessing I would need a wheel pulley between 40t-70t using just not sure which # of teeth exactly, and this would be using a motor pulley of 16t.
```

---
## \#2 Posted by: trampa Posted at: 2019-03-17T11:28:40.296Z Reads: 158

```
Use the calculator on www.VESC-Project.com
We gear tge gummies 14/44, which is pretty long and fast. Dual 6374 will give plenty of power. With dual VESC Six Plus on 12S the performance is insane.
```

---
## \#3 Posted by: meesie Posted at: 2019-03-17T12:17:36.349Z Reads: 154

```
get a pulley that fits your wheel, then  adjust your motor pulley accordingly to get the maximum top speed you would like to achieve.

i've got a 12s, 190KV, 97mm wheels setup, i run this with 1:3 gearing (12:36). this gives me a topspeed of 40Kmh which is exactly how fast  i'd like my topspeed to be. 

using this method of limiting your topspeed to your desired max speed gets you the most torque out of your setup. if anything in my message is unlear let me know, english is not my first language :smile:
```

---
## \#4 Posted by: ninTHIENdo Posted at: 2019-03-17T12:44:36.722Z Reads: 139

```
Is the calculator broke? Or am I only allowed to use a 1s build for the battery selection side?

![image|281x499](upload://c0CLKCO4Rpestqd2dZdOkG7SNue.jpeg)
```

---
## \#5 Posted by: ninTHIENdo Posted at: 2019-03-17T12:48:58.615Z Reads: 121

```
Never mind, you can’t switch the cell count on custom motor, so it defaults to a 1s. The best option is to choose a motor closest to the specs you have it seems
```

---
## \#6 Posted by: meesie Posted at: 2019-03-17T14:20:47.090Z Reads: 100

```
http://calc.esk8.it/#{%22batt-type-lipo%22:0,%22batt-cells%22:12,%22motor-kv%22:190,%22system-efficiency%22:90,%22motor-pulley-teeth%22:16,%22wheel-pulley-teeth%22:55,%22wheel-size%22:125}|

this calculator works really well. 50km/h is ~33mp/h by the way.
```

---
## \#7 Posted by: myreala Posted at: 2019-03-17T17:32:03.352Z Reads: 87

```
I am on 10s and my gearing is 15/44. On my low kv motors that equates to 23mph top speed, plenty for me.
```

---
## \#8 Posted by: Resonant Posted at: 2019-03-18T03:34:24.298Z Reads: 61

```
which belts would I use for 14/44 then?
```

---
## \#9 Posted by: mynamesmatt Posted at: 2019-03-18T04:20:26.312Z Reads: 57

```
https://www.bbman.com/belt-length-calculator/

use this
```

---
## \#10 Posted by: myreala Posted at: 2019-03-18T04:26:46.852Z Reads: 51

```
I ended up using 280mm but depends on your mount
```

---
## \#11 Posted by: Resonant Posted at: 2019-03-18T04:27:00.933Z Reads: 54

```
What would I use for desired center distance for 15mm belts? 7.5mm? Have no idea what to use for this
```

---
## \#12 Posted by: ninTHIENdo Posted at: 2019-03-18T04:43:54.840Z Reads: 52

```
It’s the distance from center of the wheel pulley to the center of the motor pulley, whatever the distance of those two points is what you’ll use as the center to center distance.
```

---
## \#13 Posted by: trampa Posted at: 2019-03-18T11:18:56.651Z Reads: 41

```
Changed that for you. Should work now.
```

---
