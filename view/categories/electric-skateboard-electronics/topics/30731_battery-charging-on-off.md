# Battery charging on/off

### Replies: 5 Views: 369

## \#1 Posted by: Jedi Posted at: 2017-08-15T18:23:31.800Z Reads: 87

```
So I have a gen 1 Spacecell battery. To charge, I plug in the charger and the LCD turns on and the battery is charging. I don't need to switch the battery on to charge.

I also have a 10s3p pack from @JLabs. To charge, I plug in the charger, but must also switch on the battery. The battery won't charge unless turned on. 

Why is this? Is one method safer than the other?
```

---
## \#2 Posted by: Jinra Posted at: 2017-08-15T18:27:26.352Z Reads: 83

```
It's how the BMS works. The way that jlabs BMS works, it needs to be on to charge. The space cell BMS allows chargin whether or not the BMS is on, since it bypasses discharge.
```

---
## \#3 Posted by: Jedi Posted at: 2017-08-15T18:35:33.479Z Reads: 72

```
Ahh I see. Is one safer than the other? Will the jlabs battery auto shutoff at full charge?
```

---
## \#4 Posted by: JLabs Posted at: 2017-08-15T18:40:26.558Z Reads: 64

```
Yep as @Jinra said, its because of the BMS.. One isisnt really safer than the other, but the only disadvantage of having the switch on when charging is that the system is powered. You can solve this by disconnecting the XT90 or installing a loop key if you have an enclosure
```

---
## \#5 Posted by: fedestanco Posted at: 2017-08-16T00:13:27.506Z Reads: 44

```
@JLabs is safer. You can literally (dont do it) short the black and red cable without damaging the battery.
Plus if you are close to overdischarging jlabs' bms will cut the power, whereas the space cell would continue discharging till this point https://m.youtube.com/watch?v=bNNWbm681AI
```

---
