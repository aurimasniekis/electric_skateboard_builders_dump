# Confirm Vesc settings an voltage cutoff at 40% bat. Level for 12s5p/130 kv dual setup

### Replies: 11 Views: 130

## \#1 Posted by: lockeboss Posted at: 2020-02-09T14:52:11.270Z Reads: 35

```
So after some long time I finally got the board on the street last season but I was only able to make 4 test rides before winter.

Im using a dual setup with:

Motor: 2 x mad hubs 130 kV 

(https://www.electric-skateboard.builders/t/review-and-eu-usa-group-buy-90mm-mad-hub-motors-75kv-or-130kv-dual-170-euro-1st-round-closed-working-on-the-dd-conversion-kit-mad-fury/62002)

Vesc: 2x FLIPSKY FSESC 6.6 

(https://flipsky.net/collections/new-accessories/products/flipsky-fsesc-6-6-based-upon-vesc%C2%AE-6-heat-sink)

Battery: 12s5p

 (https://eskating.eu/product/flat-12s5p-eskating-electric-skateboard-battery-samsung-30q/)

Right now I'm using this settings:

![vescmonitor|241x500](upload://f8bwi1C4uIGKBVUllfF4zmUqnZA.jpeg) 

![vescmonitor|241x500](upload://eGYw0rqiSrYVqNvApREDNd3Y5xW.jpeg) 

![vescmonitor|241x500](upload://jLwfSK8bGxjobe4CWotVsgyC7PU.jpeg) 

![vescmonitor|241x500](upload://opikoDLRxzUAAgp0MSKyfkBFJV5.jpeg) 






So far everything seems working OK but it's my first board so I don't have any experience. It feels a little weak even riding up flat hills and I'm not sure if its because of some false settings.

Also there seems to be a problem with the battery. I got voltage cutoff at 40% battery level at every ride.
Battery cutoff is set as suggested by vesc tool.

Does this mean the battery is broken? Or the bms? Or some settings?

Hoping for some Tipps :D
```

---
## \#2 Posted by: rey8801 Posted at: 2020-02-09T21:20:25.780Z Reads: 25

```
No the problem are the hubs. They have really high Kv. I am using the 75Kv version and they have so much more torque.
```

---
## \#3 Posted by: Santino Posted at: 2020-02-10T08:19:01.519Z Reads: 22

```
Also if you are planning to store your board for the winter, leave the battery at storage charge, and check it every couple of weeks at least....many people let their batteries unatended resulting in catastrofic failure, money wasted...
```

---
## \#4 Posted by: lockeboss Posted at: 2020-02-10T10:03:13.002Z Reads: 23

```
OK so I guess I expected to much 😁
```

---
## \#5 Posted by: lockeboss Posted at: 2020-02-10T10:06:41.624Z Reads: 22

```
I know about the storage charge an it was in regular use for bench testing.
But from the first ride on it always died at 40%.
I'm not sure if the battery is broken or the bms.  if it can be repaired or if I need to buy a new one.
```

---
## \#6 Posted by: Santino Posted at: 2020-02-10T14:32:59.781Z Reads: 22

```
You can check your P groups (the internal battery resistance ir), it could be a something simple or it could be thet 30Q are not original...Also you could set up your cut off numbers using the following Esk8 calculator https://shop.3dservisas.eu
At 40% maybe they are saging enough to activate the cut off end of the ESC or the BMS if its set to charge and discharge balance...
```

---
## \#7 Posted by: lockeboss Posted at: 2020-02-10T16:37:33.167Z Reads: 15

```
I used the cutoff numbers wich the vesc tool calculated (start 36v,end 33,6v).the calculator you suggested calculates the same numbers.

Should I measure the p groups when fully charged or after it shuts down at 40%?
```

---
## \#8 Posted by: Santino Posted at: 2020-02-10T23:02:08.601Z Reads: 13

```
I would mesure the P groups ASAP....Check everything its ok...internal resistance it is a must, to at least know how are the batteries holding up....Just to let you know, if your battery sags to much, you will activate the BMS discharge protection if you have it running, or/and the ESC...Lest says you push your throttle hard at 37v, and your sag is 6v for any reason, 37v-6v= 31v ....and then cut of happen suddenly....
```

---
## \#9 Posted by: rey8801 Posted at: 2020-02-11T08:19:54.254Z Reads: 11

```
for the 130Kv pass 15kmh they starts to pull and bring you up to ultrasonic speed. 0-15kmh is their weak spot, don't push them too hard there. They ask a lot of current to produce strong torque, due to the low efficiency at lower speed. If you are capable you can switch to wye configuration of the motor terminal and they became the 75kv version. Much much better.
```

---
## \#10 Posted by: lockeboss Posted at: 2020-02-11T18:16:35.200Z Reads: 9

```
I'm not really sure how to check the ir. I only have a multimeter.I also have the ackmaniac app and some recorded data. But there is no voltage staging visible ecpect the moment the board turns off at 40%

I measured the voltage of the packs:


Pack 47,7 v (80%)

1. 43,6/4,1
2. 39,75/3,85
3. 35,72/4,03
4. 31,68/4,04
5. 27,65/3,48
6. 24,17/4,03
7. 20,14/4,03
8. 16,11/4,03
9. 12,07/4,04
10. 8,04/4,03
11. 4,02/4,02
12. 0

So there seems something wrong with nr 2 and 5.maybe not balanced correctly?
```

---
## \#11 Posted by: Santino Posted at: 2020-02-12T22:28:05.972Z Reads: 6

```
Thats it is not balanced..Also 12 is 0? that is dead....Your should check at esk8.news forum...If 12 is dead you need to change the P group depending on how much use did you put on the battery....You have to balance every P group, the lowest voltage in a P group is goind to cut off the bat....As I mention before, go to the other forum and ask at the newbies questions, you will get tons of help...
```

---
