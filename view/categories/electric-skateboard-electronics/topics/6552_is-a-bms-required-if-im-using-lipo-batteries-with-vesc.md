# Is a BMS required if I&rsquo;m using Lipo batteries with VESC

### Replies: 25 Views: 4343

## \#1 Posted by: Raf Posted at: 2016-07-24T10:31:17.432Z Reads: 327

```
Just as the tittle says. Is it required to use a BMS on my LiPo batteries if i am using a VESC on my setup?? i am planning on making a 12s setup with 4 3s 20c LiPo packs.
```

---
## \#2 Posted by: jrpwit Posted at: 2016-07-24T11:21:41.085Z Reads: 324

```
Cleaned up the title. Anyways a bms is not required for lipos or really any battery type. A bms just makes charging a little easier. Just get a balance charger which will charge and balance batteries like a bms does. Also what kv are you using with that 12s setup?
```

---
## \#3 Posted by: Raf Posted at: 2016-07-24T11:22:46.133Z Reads: 323

```
dual 190kv motors
```

---
## \#4 Posted by: jrpwit Posted at: 2016-07-24T11:29:29.437Z Reads: 316

```
Sweet! But you may want to consider doing 10s instead of 12s. You dont want to push 60,000 erpm when you cells are fully charged on 12s but is the cells are at 3.7 volts you will not go past 60k. So just dont go full throttle when the board is fully charged especially if their is no weight on the board. The newer vesc should not have this problem though whenever people start making it.
http://www.electric-skateboard.builders/t/choosing-the-right-motor-kv-for-the-vesc/3125
```

---
## \#5 Posted by: Raf Posted at: 2016-07-24T14:44:19.921Z Reads: 276

```
so a better motor would be the 170kv? which will allow me to go full throttle on a full charge?
```

---
## \#6 Posted by: Raf Posted at: 2016-07-24T14:50:18.937Z Reads: 267

```
and would that matter if i am going for a dual motor setup? or does the 12s still affect it
```

---
## \#7 Posted by: jrpwit Posted at: 2016-07-24T19:52:03.475Z Reads: 242

```
Only the amps from the battery are split in half in duel setups. The volts stay the same tho so 50 volts on both motors. I mean dual 190kv on 12s has been done. Longhairboy uses it in his boards but to be on the safer side 10s would be best. Enertion uses 10s 190kv setups so and his boards are monsters! Anyways if you do decided to go 12s (which is totally fine) just make sure to limit the erpm in BLDC Tool to a max of 60,000 erpm. Everything should work fine if you do that. Anyways like I said vesc v6 is coming soon and it will fix the erpm problems. Happy building :smiley:
```

---
## \#8 Posted by: Raf Posted at: 2016-07-24T21:12:29.092Z Reads: 231

```
do you know when this VESC comes out. And also i have read that around 8000 RPM on the motor would make for an efficient built. On my speed calculator i have 80mm wheels with a 12s battery pack and a 12t/32t gear ratio. The RPM according to my calculator with this setup it is at 8000+ RPM but when i set the battery size to 10s it goes down to 7000+. Anyways to fix this or am i just talking complete shit??

Also i thought a 12s battery setup would be 44V (as recorded on my speed cal)

10s speed cal

<img src="/uploads/db1493/original/2X/f/f27a396a6ffb0a92fc62dde899d045e67bbff415.png" width="690" height="367">

12s speed cal

<img src="/uploads/db1493/original/2X/f/f09bee53a2aad12a8da8cbcc9eea1eb258bc825a.png" width="690" height="365">


I know that a 12s setup would work but as this is my first build i would like to take the safer side and not blow anything up as i am still learning a lot
```

---
## \#9 Posted by: Namasaki Posted at: 2016-07-24T21:42:03.338Z Reads: 197

```
Lipo cells are 4.2v at full charge so 
12s is 50.4v  at full charge.
```

---
## \#10 Posted by: jrpwit Posted at: 2016-07-24T22:45:49.999Z Reads: 195

```
Im not too familiar with rpm but I would imagine lower rpm is better for the motor and vesc because the motor is spinning slower. In my opinion, your rpm whether is higher or lower shouldn't really make a difference. Like I said 10s and 190kv would be safest but their is noting wrong with 12s as long as you are careful and set an erpm limit.
```

---
## \#11 Posted by: Hummie Posted at: 2016-07-25T00:01:38.444Z Reads: 189

```
the vesc and motors like to go fast.  they are more efficient at higher speeds.  not over the erpm limit though.  I forget the optimum number the vesc likes to go but it's really beside the point because you'll doing all kinds of speeds and not staying at one.   if you did go over the erpm limit with even the lower kv motors such as going down a steep downhill that's bad.  I think its really bad.  shut off the board or brakes go on or something.   
i dont use a bms.  i use the vesc's low voltage cut offs.  I charge with a 48 volt adjustable bulk charger (meanwell but not the best) and small balancers off the side.  easy and quicker at 400 watts.  not the safest and you have to be aware of what's going on as apposed to a bms or balance charger of course but I always am around when charging.
```

---
## \#12 Posted by: DeathCookies Posted at: 2016-07-25T11:43:33.726Z Reads: 176

```
[quote="jrpwit, post:2, topic:6552"]
A bms just makes charging a little easier
[/quote]

Thats not true at all. It will controll each individuell cell voltage and can shut down **while** riding if one cell goes below a certain voltage. A balance charger cannot check the cell status while riding!

--> Additional securtiy feature
```

---
## \#13 Posted by: Bender Posted at: 2016-07-25T12:04:34.262Z Reads: 165

```
I'm not trying to be contrarian, I'm genuinely curious, has anyone ever had this happen in a real world situation.
And would It cause you to SYF? (Due to loss of breaks or acceleration)
I'd rather ruin my battery than my face :grin:
```

---
## \#14 Posted by: Raf Posted at: 2016-07-25T14:44:38.957Z Reads: 159

```
isn't it dangerous letting them fully charge to 4.2v or is it only dangerous if you charge over that
```

---
## \#15 Posted by: DeathCookies Posted at: 2016-07-25T15:13:33.636Z Reads: 151

```
My first comment was not that good....
I think you have three options to set with a BMS:

1. Do nothing (you can drive normally and ruin you cells)
2. Low Voltage Cutoff (slowly decreases speed)
3. Instant off

Well you are right. I would not recommend instant shutdown... I would always prefer LVC because you can test the battery with a little topspeed test. If you are slower than normal one or all cells are depleted. 

Currently i have the problem with a Zippy battery from HobbyKing that they are drifting.

One time i had one cell at 3.3 and the other 6 at 3.7. You dont feel the difference because it is just one cell but if i had driven along that cell were destroyed...
Thus a BMS is practical! IMO
```

---
## \#16 Posted by: Raf Posted at: 2016-07-25T15:15:58.926Z Reads: 152

```
with that battery did you have to throw it away or did you use a balance charger to get them back to the same?
```

---
## \#17 Posted by: Namasaki Posted at: 2016-07-25T15:32:47.369Z Reads: 150

```
4.2 is normal voltage at full charge for 3.7 cells. 
It is safe to charge them to 4.2
```

---
## \#18 Posted by: jrpwit Posted at: 2016-07-25T20:09:32.744Z Reads: 146

```
What I meant by "easier" is that you dont have to deal with the balance leads. All you do is plug in the charger and boom the cells get charged and balance. I know the draw backs of a bms such as shutting off if a cell becomes too unbalanced but this is unlikely. Many people use a bms and dont have a problem. Is a bms necessary? No, but is will it make you cells safer and make the cells last longer? Yes, although it may not make the cells last that much longer. I really dont feel like arguing but the facts is the the bms protects the cells which means it will shutting down the board if necessary. That bad cell cold damage the other cells completely destroying the battery.

Btw I dont use a bms. Lipos unlike li-ion is much cheaper so if a cell gets destroyed I wouldn't care. I just uses the low voltage cut off on the vesc and a voltmeter to monitor the cells while riding. I have noticed that the cells hardly come unbalanced at all even after they are fully discharged which further proves my point that a cell to become too unbalanced that it would cause the bms to shut off the board. This is also the reason I feel I dont need a bms. Why do you think Enertion and ebike batteries use a bms? Again, cause it protects the cells.
```

---
## \#19 Posted by: Bender Posted at: 2016-07-25T20:42:55.060Z Reads: 133

```
Thanks for the explanation
How do you set LVC?
```

---
## \#20 Posted by: Hummie Posted at: 2016-07-26T00:04:02.114Z Reads: 126

```
theres two lvc.  one that drops the power a bit and the second that really cuts it down.  go to motor config tab and then motor tab again and they're there on the right
```

---
## \#21 Posted by: DeathCookies Posted at: 2016-07-26T14:22:05.957Z Reads: 120

```
I am currently using this pack but more as a spare pack because i have to be careful with it... 

i can charge it with a balance charger and it will balance it but when i ride hard it will drift very fast...
```

---
## \#22 Posted by: DeathCookies Posted at: 2016-07-26T14:26:29.860Z Reads: 117

```
You got me wrong!
I have no BMS yet but i am a huge fan of a BMS because it is protecting the cells!
<br><br
[quote="jrpwit, post:18, topic:6552"]
I know the draw backs of a bms such as shutting off if a cell becomes too unbalanced but this is unlikely.
[/quote]

That is not a draw back! It is a huge advantage over a balance charger.
<br>
[quote="jrpwit, post:18, topic:6552"]
Is a bms necessary? No, but is will it make you cells safer and make the cells last longer? Yes,
[/quote]

I do agree!
<br> 
[quote="jrpwit, post:18, topic:6552"]
That bad cell cold damage the other cells completely destroying the battery.
[/quote]
Why? Could you explain it a bit further?

<br>
[quote="jrpwit, post:18, topic:6552"]
I have noticed that the cells hardly come unbalanced at all even after they are fully discharged
[/quote]
Mhm... One of my 6S Zippy Flightmax 8Ah is drifting... Since one cell dropped down to 3.3V while the rest is at 3.8V - 3.9V this cell (3.3V) is always drifitng very fast. I can ride with this pack but not 60% of its charge....otherwise this cell would be completly damaged!
```

---
## \#23 Posted by: Gandinator Posted at: 2018-08-04T17:26:21.141Z Reads: 29

```
Hi, I need some help.
Do you know anywhere I can get a good BMS. My setup is a 10S (2x 5000mah 5S lipos). I want it for charging. I dont know how discharging helps because I assume that the cells are discharged when you ride the board right? Of course I dont want to spend a lot...

Thanks
```

---
## \#24 Posted by: Hummie Posted at: 2018-08-04T18:02:38.373Z Reads: 30

```
maybe you could unsolder it and ride with a cell less or add a replacement cell.  i have a couple laying around.
```

---
## \#25 Posted by: DeathCookies Posted at: 2018-08-04T19:02:14.850Z Reads: 30

```
One less is a draw back but a possibility. Replacing is only valid if the IR is the same or it will get unbalanced soon again.
```

---
