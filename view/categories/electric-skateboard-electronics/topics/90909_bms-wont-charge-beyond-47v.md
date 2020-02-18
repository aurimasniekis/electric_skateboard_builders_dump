# BMS won&rsquo;t charge beyond 47V

### Replies: 5 Views: 159

## \#1 Posted by: Miquel Posted at: 2019-04-17T19:19:07.967Z Reads: 46

```
Hi folks,
I recently made my own battery pack (12S3P) but i'm facing an important problem i couln't solve. 
I'm using a 50.4v charger but the BMS seems to stop,  stucked at 47v. The light turns green.  

I'm using this 40A model that I bypass. B- to the antispark P- to charger port. 

![](https://ae01.alicdn.com/kf/HTB1bF7HMXXXXXbnXXXXq6xXFXXX6/12-S-40A-50-4-V-li-ion-BMS-PCM-batterie-panneau-de-protection-bms-pcm.jpg_q50.jpg)


First, i thought about soldering issue or bad connection somewhere but it doesn't seem to be the root of the problem. 

I also checked every cell voltage, everything looks ok (some group cells (p)have a 0.02 v difference). 

Now I've to admit i'm a bit confused, if any of you guys already had this problem and know how to solve it. 

Thx !
```

---
## \#2 Posted by: Andy87 Posted at: 2019-04-17T19:23:16.556Z Reads: 39

```
Do you have a wiring diagram how you wired everything up? Or maybe as min some pictures of the bms installed and maybe a link to the bms. That would help a lot.

Did you also check if your charger really output 50.4V?
```

---
## \#3 Posted by: Miquel Posted at: 2019-04-17T19:41:06.671Z Reads: 34

```
I found this one on the internet, i can't tell if it's correct. Someone on the forum already asked about bypassing this particular BMS, and they told him to connect battery minus to B- and P- to battery positive.  
 ![rBVaVVxPSoOAQFCVAAE0cC8GMcg022|690x422](upload://avJR87bfVvQQudKNSpqB7kN75Re.jpeg) 

Otherwise, my charger is brand new and fine (50.4v) output. I also checked each cell while bms plugged in
```

---
## \#4 Posted by: Andy87 Posted at: 2019-04-17T19:53:10.798Z Reads: 22

```
If you bypass a bms you don’t connect the main + from the battery at all to the bms. 
Charge - goes to B- and the P- goes from the bms to the battery -. The charger + goes directly to the battery +
```

---
## \#5 Posted by: Miquel Posted at: 2019-04-17T20:00:10.600Z Reads: 19

```
My bad ! I made a mistake. In fact P- is connected to charger port -.
And as you said main + isn't connected to anything except charger port +. 

Anyway charging works fine until I reach 47 V where BMS seems to cutoff.
```

---
