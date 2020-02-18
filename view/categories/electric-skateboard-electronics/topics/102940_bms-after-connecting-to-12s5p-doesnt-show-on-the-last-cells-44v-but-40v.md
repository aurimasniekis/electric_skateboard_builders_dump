# BMS after connecting to 12s5p doesnt show on the last cells 44V but 40V

### Replies: 17 Views: 126

## \#1 Posted by: Marin1981 Posted at: 2019-10-14T17:52:28.910Z Reads: 27

```
![gallery|690x331](upload://4r10DKyLJdyl8dCa9PSePMzzc8S.jpeg)
Hi to all!
I connected BMS (Bestech) balance wires according to the picture above and according to scheme from Bestech I tested voltages on pin connector and for some reason on the far end I don't get ~44V but 40V.

Is this ok or not, I measure it several times and for each pin Volts are rising by 3.6V but at the last one it shows 40V.

Can someone please take a look at the above picture and let me know if anything is wrong with it?
Thanx
```

---
## \#2 Posted by: Jumpman Posted at: 2019-10-14T17:59:44.985Z Reads: 25

```
You have to start your balance leads 1-12 starting from your negative end.  So from B-,1,2,3,4 etc.
```

---
## \#3 Posted by: Tinp123 Posted at: 2019-10-14T18:01:37.527Z Reads: 25

```
Which bms do you have? 12 or 13 balance wires?
```

---
## \#4 Posted by: Marin1981 Posted at: 2019-10-14T18:59:45.447Z Reads: 24

```
I have 12 wires
```

---
## \#5 Posted by: Marin1981 Posted at: 2019-10-14T19:03:39.654Z Reads: 24

```
I connected main minus B-, and started from 1bto the last one. As I said on first I measure 3.6,and after they all rised for 3.6 and on the last wire it says 40V.
I don't understand what is wrong, I checked diagram and connections dozen of times.
```

---
## \#6 Posted by: Tinp123 Posted at: 2019-10-14T19:07:12.408Z Reads: 24

```
Take a good look on your bms pcb, where connector for balance wire is. You should see that first pin on pcb (which should go on first group negative) is not soldered on balance wires connector. You can take photo and post it here just to confirm. In this case, your first balance wire will go between 1st and 2nd group, second wire between 2nd and 3rd group and so on. If you did everything right, your last balance wire should be connected after last group, on battery main positive
```

---
## \#7 Posted by: Marin1981 Posted at: 2019-10-14T19:09:08.740Z Reads: 23

```
I have 12 balanced wires. On the main minus and +I measure 44V.on balance wires I measure
1. 3.6
2. 7.2
3. 10.8
4. 14.4
5. 18
6. 21.6
7. 25.2
8. 28.8
9. 31.4
10. 35 
11. 38.6
12. 40.1V
Where did I go wrong?
```

---
## \#8 Posted by: Tinp123 Posted at: 2019-10-14T19:17:14.348Z Reads: 22

```
See my last post. Upload photo of bms pcb here please :) part where balance wire connector lays
```

---
## \#9 Posted by: Marin1981 Posted at: 2019-10-14T19:21:24.137Z Reads: 21

```
![15710807982017128584344477497306|374x500](upload://6EdRSeL1Ri6HOErPQKKDgn3Hb9p.jpeg) ![15710808510905590554449049866776|374x500](upload://1zys8Vgu9BeXYaD1jqu8BhoOQ2j.jpeg)
```

---
## \#10 Posted by: Tinp123 Posted at: 2019-10-14T19:24:42.393Z Reads: 18

```
Now when looking at voltages, try to meassure voltage on your last group. From your last measurement seems its 1.5v?
```

---
## \#11 Posted by: Marin1981 Posted at: 2019-10-14T19:31:42.765Z Reads: 18

```
No it is 3.6V.on first four groups is 3.5V,everywhere else is 3.6
```

---
## \#12 Posted by: Tinp123 Posted at: 2019-10-14T19:39:20.239Z Reads: 16

```
But you wrote up there that you got 38.6v after 11th and 40.1v after 12th group?
```

---
## \#13 Posted by: Marin1981 Posted at: 2019-10-14T19:42:45.868Z Reads: 15

```
Sorry I went by memory, but few moments ago I measured as in previous reply.
Can you help me out I can't find where did I made mistake
```

---
## \#14 Posted by: Marin1981 Posted at: 2019-10-14T19:44:41.788Z Reads: 15

```
Just measured again on 11th I have exactly 36V and on 12 39.6V
```

---
## \#15 Posted by: Tinp123 Posted at: 2019-10-14T20:02:42.752Z Reads: 16

```
You are measuring on balance wires, right? I see you dont have balance wire on your main battery negative (like I told you should do) and you have only 12 balance wires, it is normal that between first and last balance wire you get only 39.6v. Put one probe on battery main negative and one probe on last balance wire, you should get 43.2v now. Btw you did not use insulation rings and you didnt put fishpaper between groups. Also, take care of your balance wires so they won't be pierced by the nickel in the middle of your battery
```

---
## \#16 Posted by: Marin1981 Posted at: 2019-10-14T20:21:43.125Z Reads: 16

```
![15710836041168896383950217228116|374x500](upload://7MgEtpG91gEz4GujEBToERPDJ3O.jpeg)
Is this thick black the main negative? I connected it as per bestech instructions.On their paper says to connect first B- on main negative and then balance wires on pluses on each group and in between. 
So if it is normal that between 1st and 12th wire I get 39.6V if I get it right I haven't made mistake?
Just measured from main negative and last wire again you were right I get 43.3V.

You see well havent used fishpaper and no rings,I should but this is my first battery pack and first electric longboard so still learning. 
I will certainly put insulation between because already I burnt one cell.... and I will take care of balance wires. 

Thank you very much for your help I started to become crazy😁😁👍👍👍
```

---
## \#17 Posted by: Tinp123 Posted at: 2019-10-14T20:35:36.667Z Reads: 15

```
No problem for help!

But look, I would really really rebuild that pack. Take that very seriously. Pack is very long and there will be some flex in your board. Its just matter of time when thin pink insulation will wear of and you will get big fire and everything will be destroyed. Also you didn't use those insulation rings + your nickel has sharp corners which could (arguably) pierce positive end and create short. One more thing: if you want to solder wire on end of goup, use few layers of nickel. Use few layers of nickel for series connections (I can not see that from your photos), but silicone wire is much better for series connections, especially for such a long, one layer pack. Batteries could be really dangerous,tak care! :)
```

---
