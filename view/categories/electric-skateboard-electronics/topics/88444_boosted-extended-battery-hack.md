# Boosted Extended battery hack

### Replies: 14 Views: 600

## \#1 Posted by: ryan380golf Posted at: 2019-03-27T04:55:19.557Z Reads: 120

```
I found ![image|375x500](upload://f3FoA1NM7kn7nVcCmkWTzQoMLuz.jpeg) an extended battery with what I think is a faulty bms.  Blinking red light of death.  13s2p pack with 18650s. 

Pulling out the bms and I’ll need to put in my own bms or go without.  Looks like a pretty straight forward hack and rewire. Will be using for my Foosted build.
```

---
## \#2 Posted by: Dirt_Bag Posted at: 2019-03-29T04:08:59.087Z Reads: 92

```
are those li-ion or lifepo4? i cant imagine boosted runs 13s li-ion
```

---
## \#3 Posted by: ryan380golf Posted at: 2019-03-29T04:21:01.235Z Reads: 89

```
They look like 18650's.  What I understand is that the standard range uses lifepo4 and the extended range use li-ion 18650.  I'll try confirm.
```

---
## \#4 Posted by: Dirt_Bag Posted at: 2019-03-29T04:30:12.108Z Reads: 87

```
they can still be 18650 sized lifepo4 batteries, 13s is nearly 55v, last i knew boosted has never run over 10s li-ion voltage equivalent. the average buyer wouldn't be able to control the speed
```

---
## \#5 Posted by: ryan380golf Posted at: 2019-03-29T04:52:48.961Z Reads: 81

```
It's definitely a 13s2p.  I checked each pair of 2 cells.  I'm really surprised I can't find more info on the BB extended battery...

I'm trying to confirm the cell type.  I really want to use them in this internal case but could open them and harvest out the cells.
```

---
## \#6 Posted by: ryan380golf Posted at: 2019-03-29T04:56:32.041Z Reads: 74

```
Quote that I found:

The new charger is 54.4v that’s basically 13x 4.18v logical for boosted to not charge there batteries to 4.2v. Boosted said 199wh so 13s2p of 1.8ah batteries sounds great. or they are using 15s lifepo4 safer and better life cycles and what they currently use. the reasons for increasing voltage, basically if they have a torque control ESC then they can draw on the voltage and also stop voltage sagging from reducing the top speeds that they provide. Every thing is regulated. You buy a v2 with a 99wh battery the pack is still the same as the V1 but the charge voltage is 54.4. They have 2 depths of the charging port one for 43.2v so you can use your V1 charger and the second for 54.4v that runs through a regulator to then drop the voltage to charge the cells.
```

---
## \#7 Posted by: Dirt_Bag Posted at: 2019-03-29T04:59:22.528Z Reads: 74

```
Wow... thats seriously impressive they upped it to 13s voltage. I had no idea they ever upgraded!
```

---
## \#8 Posted by: ryan380golf Posted at: 2019-03-29T05:26:59.911Z Reads: 69

```
They use a higher voltage then The esc limits the speed.  Only the stealth has access to the higher speed options.   Diy’ers have full access to speed. Boosted contains it.  Fast enough for their riders.
```

---
## \#9 Posted by: Pantologist Posted at: 2019-04-07T14:59:18.148Z Reads: 62

```
The specs on the label have always shown 13S specs.
```

---
## \#10 Posted by: Pantologist Posted at: 2019-04-07T15:01:46.125Z Reads: 62

```
Hey Ryan, have you been able to identify the cells?
```

---
## \#11 Posted by: ryan380golf Posted at: 2019-04-07T15:19:08.528Z Reads: 54

```
I’m gonna say 18650s.  Waiting for my bms to come in for it.  There was something wrong with the Boosted bms.  All out of balance but salvageable. Got it cheap.
```

---
## \#12 Posted by: Pantologist Posted at: 2019-04-07T15:33:31.536Z Reads: 49

```
Yeah definitely 18650 but it seems no one really knows the brand or model # of the cells.

My guess based on the label is Sony/Murata VTC5D cells.
```

---
## \#13 Posted by: gmurad Posted at: 2019-04-07T16:11:14.864Z Reads: 47

```
Cool! So they use a compression (e.g.: NESE) to keep the pack together?
```

---
## \#14 Posted by: ryan380golf Posted at: 2019-04-08T00:49:19.484Z Reads: 38

```
They are spot welded, but in a very tight case.
```

---
