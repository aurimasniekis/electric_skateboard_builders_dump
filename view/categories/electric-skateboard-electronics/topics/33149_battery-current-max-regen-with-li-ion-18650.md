# Battery current max regen with li-ion 18650

### Replies: 7 Views: 1223

## \#1 Posted by: Silverline Posted at: 2017-09-14T17:54:50.991Z Reads: 247

```
Hallo

I have a dual motor setup on two focboxes.

My battery is a 10s5p made of Samsung q30 li-ions

What would people recommend for "Battery current max regen" on each focbox ?? At the moment i run them at -20A. I i think that its a bit to high right ??
```

---
## \#2 Posted by: MaxAssist Posted at: 2017-09-14T18:19:13.132Z Reads: 243

```
Does your battery pack have the BMS? If yes don't be mindful of the max regen b/c the bms will do the job for you. But I doesn't hurt to use Vesc as your second option, right? I have a torque board 12s4p pack, I set max regen 12A. Hope it helps
```

---
## \#3 Posted by: Jinra Posted at: 2017-09-14T19:11:39.289Z Reads: 233

```
Each one should be -10a. However since you don't regen very much for very long you would probably be safe setting it slightly higher for better braking at speed
```

---
## \#4 Posted by: Pedrodemio Posted at: 2017-09-14T19:16:47.788Z Reads: 228

```
You don't want the BMS cutting because of too high current, besides you losing brake if that happens, the current has nowhere to go and the voltage rises more quickly than the protection circuit on the VESC can react and you end up frying a DRV or everything
```

---
## \#5 Posted by: Silverline Posted at: 2017-09-14T19:29:08.680Z Reads: 217

```
Thanks guys...

I use the bestech 10s/80a BMS.

I will set it to -10 insted. But then i need to raise my 'motor current max brake' right, to have the same braking force as before ?
```

---
## \#6 Posted by: karma Posted at: 2017-09-18T20:37:50.074Z Reads: 188

```
So if I use 2 VESC I should give each VESC half of what the battery is capable off?
```

---
## \#7 Posted by: Jinra Posted at: 2017-09-18T21:30:46.964Z Reads: 180

```
correct

10 chars
```

---
