# How to Modify a BMS

### Replies: 2 Views: 413

## \#1 Posted by: BooYA Posted at: 2018-07-18T10:51:48.464Z Reads: 72

```
Hi everybody,
I'm sharing with you an interesting mod I did to my BMS, as it might be useful to someone else. 

I'm building a 12S pack and so bought a 12S 60A BMS from Supower/Batterysupport.
Even though this BMS is renowned for its quality, I was disappointed by its size and the lack of switch. 
So I searched the web for a lighter solution, and surprisingly found out that there was very few 12S Li-ion BMS available.
However, I found big choice of 13S BMS. And even more interesting, I noticed that my 12S BMS from batterysupports was originally designed as a 13S PCB but lacked components on the 13rd stage... 

I found a tiny, 8 euros 13S BMS with great reviews and perfect parameters, bought it and modified it to remove all the components on the 13rd cell stage : 
![20180705_180855|281x500](upload://9oxonSL1Hi6oHnEdZNRdeumh90V.jpg)

I then plugged my battery to it, everything okay, plugged charger, charging went okay, and the charging Mosfet stopped the charge as soon as one cell reached 4.2V ( I used a very tiny 3x4S 1300mah unbalanced lipo battery pack to check the balancing feature) the BMS started burning the higher cells and even has leds to show which cells are being balanced! I was checking everything with lipo checkers. 
When the high cells got down to 4.15V the charging Mosfet started to charge again etc.
I then tried the output, hooked up leds and let the pack fully discharge the whole day through the discharge Mosfets, which eventually stopped the discharge immediately when the weakest cell was 2.9V! And I charged again no issue :slight_smile:

So it seems possible to modify a bms to suit one less cell pack
```

---
## \#2 Posted by: Holyman92 Posted at: 2018-07-18T12:06:48.933Z Reads: 50

```
Next time, don't bother taking off the 13th stage man... it's fine and will work the same if you hookup everything the same way you normally wpuld... just leave off the 13th balance lead
```

---
