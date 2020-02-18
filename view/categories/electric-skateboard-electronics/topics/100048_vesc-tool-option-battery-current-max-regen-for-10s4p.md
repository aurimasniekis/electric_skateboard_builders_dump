# VESC Tool option &ldquo;Battery Current Max Regen&rdquo; for 10s4p

### Replies: 5 Views: 201

## \#1 Posted by: Waiboard Posted at: 2019-08-10T16:50:09.798Z Reads: 46

```
I am configuring my VESC Flipsky 4.20 dual for two Flipsky 6354 190KV motors and a 10s4p battery Samsung 25r cells with BMS 100A for loading and unloading.

According to what I read and investigated the option "Battery Current Max Regen" is the ability of the battery to regenerate when braking. Since I am using Samsung 25r cells that support 4A maximum continuous load, I should put Battery Current Max Regen: -4

This is correct?
```

---
## \#2 Posted by: L3chef Posted at: 2019-08-10T17:51:39.314Z Reads: 45

```
It´s 4A per cell. and you have 4 in a parallel group. so 4*4 = 16
and you have dual drive so divide that by 2.. 8 per vesc
```

---
## \#3 Posted by: Waiboard Posted at: 2019-08-10T17:57:49.373Z Reads: 42

```
Perfect, thanks for the explanation!

I ask you why Flipsky gives a recommended setting of -20A?

I also saw that many put in their configuration -20 or similar high values for 10s4p batteries and I don't understand why. Since putting those values would damage your battery.
```

---
## \#4 Posted by: L3chef Posted at: 2019-08-10T18:02:12.776Z Reads: 42

```
Could it be that they have that value for a single drive? Usually when you brake hard it´s only for a couple of seconds max. and that should not damage the battery.. They set a higher value to get stronger brakes..
```

---
## \#5 Posted by: kntzn Posted at: 2019-08-10T18:11:19.524Z Reads: 41

```
Your battery has multiple charging currents.

I mean there are maximum constant current and absolute max. charging current. (Peak).

If u exceed the peak current that is usually several times higher than the max. constant current, you can destroy the battery’s chemistry. 

L3chef is right here, if you are live and ride in flat area, you are not going to break hard too long.
```

---
