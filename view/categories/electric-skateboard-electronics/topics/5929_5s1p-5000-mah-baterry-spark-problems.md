# 5s1p 5000 mAh baterry spark problems

### Replies: 7 Views: 1275

## \#1 Posted by: crucialhunter Posted at: 2016-07-11T20:33:23.574Z Reads: 80

```
Hi!

I have two exact batteries that i use in series . Both are the same model, 5s1p 5000 mAh batteries.

This is the first time i have to charge them after a full discharge, wich never reached less than 3.2v.

One of them seems to charge correctly.

<img src="/uploads/db1493/original/2X/3/34882fd6d50b9b38843d6ebf0779c3528e76e37e.jpg" width="666" height="500">

But the other one doesn't charge more than this 

<img src="/uploads/db1493/original/2X/e/ed0637da8029f9f2759c08992ecb9b73dd18d5f5.jpg" width="666" height="500">>

A : Does this mean that the battery is damaged?

B : Another important question, before charging them after long usage, the charger tells me they are 4 s , but after some charge it detects again 5 s, is this something i should worry about?

C : When i conect the VESC to the batteries there is a small spark (im using xt60 conectors) should i worry about this ?


thanks!
```

---
## \#2 Posted by: relaxnfly Posted at: 2016-07-12T00:12:54.566Z Reads: 57

```
A. Based on your info I wouldn't guess there is a problem with your battery.  I don't  think your battery is damaged.

B. There is definitely something wonky here.  I would think your charger auto detects based on the balance lead that is connected.
 
C. Im not a VESC user but I would expect a spark until you install some type of anti spark device.

I would suggest going back through your charger settings and make sure they are where they should be.   Give use some more  info on the settings you are using so we can help.
```

---
## \#3 Posted by: sl33py Posted at: 2016-07-12T00:25:05.162Z Reads: 54

```
Nothing looks wrong to me, other than the voltage.  Physically - does the one (or either) get hot when charging or discharging?  Is the pack puffed or swelled at all?  If you ride just the suspect one for a bit - try to run the voltage down a bit - does one cell dip significantly or earlier than the rest?  That would make me think a single cell is going bad.

For detecting 4 vs 5s - check your connectors are tight and not damaged.

3.2v is too low IMO.  I don't go below 3.7/3.6v per cell.  Others can chime in here on what they set their low voltage cutoff for.  Under load they can dip quickly, so i'd rather have a bit less range and better battery life, than to over-discharge and ruin a pack.

Do you have a cell alarm?:
https://www.amazon.com/Battery-Tester-Voltage-Buzzer-Alarm/dp/B005GJCJOA
Nice since it will alarm as soon as the lowest cell hits your set voltage limit.
```

---
## \#4 Posted by: sl33py Posted at: 2016-07-12T00:28:18.045Z Reads: 44

```
in series @10s - you will get spark.  You can eliminate this with a simple anti-spark loop key, or one of the anti-spark switches.

If you want to make a cheap DIY anti-spark loop key, here's a quick how-to i did a while back:
http://www.electric-skateboard.builders/t/how-to-anti-spark-xt-90-loop-key/204
```

---
## \#5 Posted by: claudiofiore88 Posted at: 2016-07-12T00:33:56.664Z Reads: 38

```
Does your charger have a resistance function?  I was talking to my cousin about that function the other day.  He said that it has to do with the health of the battery. Can anyone here confirm this?
```

---
## \#6 Posted by: Namasaki Posted at: 2016-07-12T01:10:23.403Z Reads: 36

```
Are you charging in balance charge mode?
Did you set the mah charge limit and charge time limit?
```

---
## \#7 Posted by: sl33py Posted at: 2016-07-12T01:13:06.380Z Reads: 33

```
Good call.  I know that my iCharger has this, but also think the B6AC has it (check midway to see example screen):
http://www.skyrc.com/index.php?route=product/product&product_id=217

look for Internal resistance in the menu of your charger and see if it has one cell w/ super high IR.  Or compare the "good" battery and suspect one's IR if only the sum of the cells.

Looking at the pics it's hard to tell exactly which charger this is...  If it has IR measurement/meter or not.

GL!
```

---
