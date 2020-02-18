# BMS heating after pluging the balancing cable

### Replies: 17 Views: 321

## \#1 Posted by: dilaboards Posted at: 2018-07-29T10:22:10.934Z Reads: 87

```
Hey there. I am new to the topic and I couldn’t find an answer on other topics related to BMS. 

So, I bought brand new Samsung batteries and created a 8s2p pack. All batteries have same voltage individually and also when connected in parallel. Currently the pack has 28.1 volts since it hasnt been charged yet. 

I wired a BMS on it starting with B- and P-. I connected also the balance wires to all the positive ends of the battery cells. When I check the voltage from negative wire to all the individual balance leads it is in line with the battery, total 28.1 volts. 

However when I plug the balance flat cable into the BMS, it starts to heat up. When I measure the voltage on the P- lead it is showing 26.0 volts so it seams this is heating up the BMS. 

Anybody struggled with a similar problem before?

Thanks Anze
```

---
## \#2 Posted by: i2oadsweepei2 Posted at: 2018-07-29T11:42:38.565Z Reads: 80

```
Can you show us some photos of the batteries, leads and bms? Do you have a link or any documentation for the bms you can share with us and where you bought it?
```

---
## \#3 Posted by: dilaboards Posted at: 2018-07-29T12:26:45.483Z Reads: 76

```
Hi. Thanks for replying. Attached a BMS spec!![image|281x499](upload://309G5VyMeGaRI6NYuDuI83rQIAy.jpg)[image|281x499](upload://uT58bpxXjGEfIXoQQAEDjK4rZMH.jpg)

Batteries are Samsung bought from this page
https://eu.nkon.nl/samsung-18650-inr18650-25r.html
```

---
## \#4 Posted by: dilaboards Posted at: 2018-07-29T12:27:40.323Z Reads: 73

```
![image|281x499](upload://uT58bpxXjGEfIXoQQAEDjK4rZMH.jpg)
```

---
## \#5 Posted by: i2oadsweepei2 Posted at: 2018-07-29T12:40:08.142Z Reads: 65

```
Sorry I meant pics of your built battery. Maybe one of the members here can spot something. I hope this works out.

My only thought it the balance leads aren’t in the proper order or the bms is defective. I know you said you checked... Does it get really hot or just warm? I’m wondering if it’s bleeding of power to balance.
```

---
## \#6 Posted by: Sender Posted at: 2018-07-29T12:40:45.584Z Reads: 61

```
Put pictures of your wiring up.  Also I am not seeing the manufacturer wiring diagram.

I have a similar BMS I am using for charge only.
```

---
## \#7 Posted by: dilaboards Posted at: 2018-07-29T13:10:45.538Z Reads: 54

```
Here the picture of the wiring with voltage measured between battery negative and battery positive (28.1 volts). ![image|375x500](upload://eNdEMZkxvYN1iIzwjv4NzdVNwjG.jpeg)
```

---
## \#8 Posted by: dilaboards Posted at: 2018-07-29T13:11:49.739Z Reads: 53

```
And here the picture with voltagr measured between battery positive and P- string which is supposed to go into the ESC.
```

---
## \#9 Posted by: dilaboards Posted at: 2018-07-29T13:13:01.316Z Reads: 52

```
![image|375x500](upload://ejhkwH6UO5QIROYIZMJv9dNqps6.jpeg)
```

---
## \#10 Posted by: accrobrandon Posted at: 2018-07-29T13:31:44.234Z Reads: 51

```
cant tell about the wiring with that picture, but the first couple times I wired a bms I got the balance wires all back wards from 10 - 1 instead of 1 -10 and when i plugged in the pigtail the bms got hot quick which i quickly unplugged and it was still fine...just had to re wire in the proper sequence... id double check all balance lead are in perfect order.. 

standard reply i know...
```

---
## \#11 Posted by: dilaboards Posted at: 2018-07-29T15:17:29.277Z Reads: 47

```
I feel kind od stupid but at the end despite double checking the cables were not wired correctly. I reversed the order and no heating occurs. What is interesting though is that now also to voltage on P- plug is equal to the battery voltage. Thank you guys for quck response. ![image|375x500](upload://4ZjodhCAXDjw1TSah4hmKTuubVs.jpeg)
```

---
## \#12 Posted by: Sender Posted at: 2018-07-29T15:42:48.269Z Reads: 38

```
Hell yeah! Glad it's sorted
```

---
## \#13 Posted by: accrobrandon Posted at: 2018-07-29T16:58:40.904Z Reads: 35

```
like i said...i did the same dumb ass mistake twice...on 2 diff batteries.... now i wont F it up again =P
```

---
## \#14 Posted by: Sender Posted at: 2018-07-29T17:20:08.290Z Reads: 32

```
I always get my wife to double check. Another set of eyes. She doesn't know batteries, but she's not dumb like me, lol.
```

---
## \#15 Posted by: Chase Posted at: 2018-07-29T19:02:44.075Z Reads: 25

```
I’ve done the same thing as well even after thinking I had double checked. It’s because sometimes the wires will overlap each other when they come out of the connector and are easy to mix up. Luckily the bms was fine.
```

---
## \#16 Posted by: Wilsonliang777 Posted at: 2018-07-30T08:56:11.477Z Reads: 18

```
I did the same thing when I installed my first bms.
```

---
## \#17 Posted by: Wilsonliang777 Posted at: 2018-07-30T08:57:58.540Z Reads: 18

```
Don't feel stupid.  We all done it.
```

---
