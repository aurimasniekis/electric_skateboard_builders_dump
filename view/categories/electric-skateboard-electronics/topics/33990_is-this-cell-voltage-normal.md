# Is this cell voltage normal?

### Replies: 19 Views: 779

## \#1 Posted by: Mikkiller Posted at: 2017-09-26T11:15:20.354Z Reads: 94

```
Hi guys,
I have just finished assembling my esk8 a few days ago and for the past two nights I've been going out for a ride. I ride until the vesc cuts out the power and I have to push back home. When I get home, I start charging the batteries for the next day. 
I use 2x 5s 5000mah lipo in series, a 190kv 6364 SK3 motor and a FOCBOX. The charger is an IMAX B6 from hobbyking.
Battery cutoff start: 34v
Battery cutoff end: 33v

This is what I see when I start charging the batteries:
Battery 1: 1st cell 3.21v, all other cells around 3.40v. As they charge the cells get balanced and they all reach 4.20v.
Battery 2: All cells around 3.50v

Is this behaviour normal? Shouldn't the cells evenly discharge when I ride? 

Thanks a lot in advance :)
```

---
## \#2 Posted by: Silverline Posted at: 2017-09-26T11:18:55.269Z Reads: 91

```
Try only run them down to arround 3,7volt pr. cell when you are out skating.
I don`t know why, so many think that they can run lipo`s down to 3,2 volts pr. cell. This is not very healthy for lipo cells.


https://www.rcgroups.com/forums/showpost.php?p=26358338&postcount=5
```

---
## \#3 Posted by: Mikkiller Posted at: 2017-09-26T11:31:25.867Z Reads: 78

```
Thanks, I didn't know that. I actually thought I was being very conservative. However, isn't this going to limit my range significantly?
Also, I forgot to mention that I'm charging them very slowly (1-1.5 A) because I have a weak power supply. Is that ok?
```

---
## \#4 Posted by: Silverline Posted at: 2017-09-26T12:23:38.322Z Reads: 70

```
Yes it does. More Range = more mAh / wH

But your lipo's do not like that low voltage, so you are going to loose capacitance anyway , if you'r continue to run them that low anyways.
```

---
## \#5 Posted by: Namasaki Posted at: 2017-09-26T12:25:37.619Z Reads: 68

```
[quote="Mikkiller, post:3, topic:33990"]
However, isn't this going to limit my range significantly?
[/quote]

This is why you should over build if at all possible
```

---
## \#6 Posted by: pat.speed Posted at: 2017-09-26T12:27:47.655Z Reads: 62

```
I thought you could discharge lipos down to 3.2v volts before they get damaged. Discharging lower than 3.7 most likely won't damage the cells but may lower the charge cycles right?
```

---
## \#7 Posted by: Namasaki Posted at: 2017-09-26T12:30:19.811Z Reads: 59

```
The problem is that most people monitor total pack voltage, not individual cells. 
If you run your 10s pack down to 32v, some cells could be much lower
```

---
## \#8 Posted by: Silverline Posted at: 2017-09-26T12:30:29.220Z Reads: 52

```
All i can say is. If we run lipo's down to 3,2v pr. Cell on racing quads , they wear out pretty quickly. They simply loose punch and capitance. If i only run Them down to 3,8 v pr cell, they live a Hell Lot longer.
```

---
## \#9 Posted by: pat.speed Posted at: 2017-09-26T12:33:33.960Z Reads: 48

```
Yeah that happened to me. I have the lvc set to 3.4v per cell and 4 cells were at 3.6v but one had dropped to 2.9v. Luckily I was able to revive it and I've been monitoring it closely for the last few rides I did and it was fine stayed in balance with the others so it's all good. Then I fractured my ankle so I can't ride for a while😭
```

---
## \#10 Posted by: pat.speed Posted at: 2017-09-26T12:34:27.700Z Reads: 48

```
Yeah I see what you mean because doesn't that drone flying stuff draw a hell of a lot of current?
```

---
## \#11 Posted by: Silverline Posted at: 2017-09-26T12:47:25.441Z Reads: 44

```
Yes it does... So even when i land at around 3,8volt pr. Cell, sometimes under hard load the cells comes down to 3v. So think how low your cells is under load, when they are 3,2 without load
```

---
## \#12 Posted by: Mikkiller Posted at: 2017-09-26T12:47:41.807Z Reads: 46

```
Thanks for all the replies. 
Anyway, I was reading a few topics on RC forums and they all say that the resting voltage should be around 3.7v. However, the voltage on load (so, when we are riding I guess) can get lower as long as cells get back to a higher resting voltage after we use them. 
I guess that the VESC can only measure the voltage when it's being used (with load), so couldn't the cutoff be a bit lower than 3.7 and still be safe?
```

---
## \#13 Posted by: pat.speed Posted at: 2017-09-26T12:49:50.807Z Reads: 44

```
Yes pretty much but it's kinda hard to estemate the voltage sag depending on your lipos. You will just have to test I guess
```

---
## \#14 Posted by: Vieo Posted at: 2017-09-26T12:50:55.124Z Reads: 44

```
I think it depends on how much risk you wana take
```

---
## \#15 Posted by: Mikkiller Posted at: 2017-09-26T13:21:15.647Z Reads: 41

```
I will try to run some tests and let you know. 
By the way, do you think that a BMS wired for discharge may maintain the voltage equal in all cells?
```

---
## \#16 Posted by: bartroosen12 Posted at: 2017-09-26T14:29:00.182Z Reads: 35

```
I have a 10S lipo pack and I always run them with a cutt off around 3,2V so after a ride all 10 cells are around 3,4V. The cells aren't warm/hot after a ride and it seems te be no problem.
If you run the batteries lower to like 2,8V, my previous battery became pretty hot and yeah I know this isn't healty at all, just don't try because I fucked up all my 12cells and it was a waste of money.
```

---
## \#17 Posted by: raven Posted at: 2017-09-26T15:13:29.689Z Reads: 33

```
Did you try single charge each cell. I have dead batteries and will try to bring them back to live when the electronics arrive
```

---
## \#18 Posted by: bartroosen12 Posted at: 2017-09-26T15:17:14.684Z Reads: 34

```
Yeah I charged every cell back to 4,2V and everything seemed to be fine but after every ride cells were totaly not balanced anymore and also very hot and swollen if I did hard accelerations so they couldn't handle high currents.
```

---
## \#19 Posted by: Mikkiller Posted at: 2017-09-30T02:17:37.549Z Reads: 22

```
After trying different values for cutoff start and cutoff end, I think that 3.7v/cell is actually the best value you can put as cutoff end. Now I have:
-Cutoff start 3.8v/cell
-Cutoff end 3.7v/cell

When I put the batteries in charge tonight I was surprised to find out that almost all cells were around 3.7v in both batteries. The one cell that always had a lower voltage this time was at 3.67v, which I think is acceptable. 
I was also very surprised at the range, which was basically the same as before, although I probably didn't climb as many hills as usual. 

All in all, I'm very satisfied. Thank you guys for your help. I hope I didn't ruin my batteries too much by discharging them this much for a few cycles.
```

---
