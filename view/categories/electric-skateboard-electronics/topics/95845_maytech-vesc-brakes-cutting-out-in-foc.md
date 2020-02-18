# Maytech VESC, brakes cutting out in FOC

### Replies: 7 Views: 232

## \#1 Posted by: YungDaff Posted at: 2019-06-04T16:48:37.838Z Reads: 52

```
So when I opened up my enclosure to install my metr pro module, I meanwhile hooked up my vesc to my pc and converted from BLDC to FOC. After a test run I was blown away how quiet FOC is compared to the screaming BLDC. The acceleration was great and braking was pretty strong as well, however I noticed a problem. When braking and almost coming to a full stop by pushing my remote at full brake the brakes would just cut out and I would start rolling again. But if I let go of the lever on the remote and attempted to brake, they were working just fine until I was pulling at full brake and almost coming to a complete stop. Here, the problem would show itself again. 

Anyone had any similar problems? 

My vesc settings are: 

Battery max: 20A

Battery max regen: -8A

Motor max: 40A

Motor max braking: -40A

I am running a single maytech vesc bought from @e.board_solutions

https://electricboardsolutions.com/products/speed-controller-based-on-the-vesc%C2%AE-project
```

---
## \#2 Posted by: YungDaff Posted at: 2019-06-04T17:02:35.591Z Reads: 42

```
![unnamed%20(1)|230x500](upload://tnJsJjZWWlvMu9214qs9aTEDtLJ.jpeg) 

This is the error I get in the metr pro. Seems to be a "DRV" error. Is my vesc ruined? 

Searched a bit on the forum and it seems that this has happened to other people aswell. I will switch back to BLDC and see what happens.
```

---
## \#3 Posted by: Jinra Posted at: 2019-06-04T17:14:32.320Z Reads: 35

```
Cheaper VESCs like maytechs are known for blowing under FOC. That DRV almost certainly means your vesc is toast, well at least your DRV chip is.
```

---
## \#4 Posted by: YungDaff Posted at: 2019-06-04T17:23:06.645Z Reads: 36

```
I changed back to BLDC, all while not having to plugging into the pc, just by using the metr pro. The braking is normal again, not cutting out at all. I am not getting the DRV error in the logs either. So my vesc is probably intact and working. 

Lesson learned: DO NOT use FOC with the maytech vescs, they cannot handle it. 

Next upgrade: other vesc :smiley:

Which vescs work with FOC? Flipsky? @Jinra
```

---
## \#5 Posted by: Jinra Posted at: 2019-06-04T17:24:40.983Z Reads: 36

```
Flipsky should work with it, I haven't used it myself though. The focbox unity or official VESC work as well. Be careful, your DRV is still likely damaged and may cutout even in BLDC. Just go slow for a while until you make sure it's stable.
```

---
## \#6 Posted by: YungDaff Posted at: 2019-06-04T17:30:43.145Z Reads: 35

```
If the DRV is damaged, what does this result in? Is it just the brakes that get affected or could this lead to the motor just shutting off when I am out riding?
```

---
## \#7 Posted by: Jinra Posted at: 2019-06-04T17:54:25.011Z Reads: 30

```
The VESC relies heavily on the DRV so it's entirely possible your board shuts off or reboots while riding.
```

---
