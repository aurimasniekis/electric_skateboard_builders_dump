# Balance wiring of the 10s3p xiaomi m365 scooter

### Replies: 3 Views: 1396

## \#1 Posted by: chickengun Posted at: 2018-10-03T17:55:25.587Z Reads: 61

```
Here is a picture of the 10s3p battery pack that you find in the xiaomi m365 scooter. My issue is I can't charge it anymore and I don't know why. I measured all the voltages across the cells and one of the welded spots was loose so I resoldered it and after that the voltage across the 10s3p battery pack was 36V which is normal. Still the voltage that's coming out of the BMS is just 18V so there is definitely something wrong with the connection to the BMS (or the BMS itself). The battery pack seems to be soldered properly, that's why I suspected the bms first. I ordered a new bms at aliexpress, soldered it but observed the same issue. Now I expect the balance cable. I would like to check the conductivity between the ribbon cable that goes to the bms and the cells using my multimeter (the ribbon cable has 19 pins, you can see it at the very top on my picture), the only problem is I don't understand the bms wiring. As you can see on the picture besides Battery B0 - B10 there is also LED+, LED-, NTC+, NTC- and KY. NTC seems to be the thermistor that is attached to the battery back. I started to measure the conductivity between ribbon pins and the cells but I don't understand what I just measured: For instance Cell "B3" is leading to 4 pins on the ribbon cable, one of them showing 1k Ohm resistance (there is a resistor near each cell, I don't know why), but for B5 on the other hand there is no 1k Ohm resistance and it leads to 5 pins on the ribbon cable! why? I could just buy the balance wires on aliexpress and change it without understanding it but it would be nice to check if everything makes sense here. I hope someone can shed some light on this matter and give me some advice what and how to check :) Thanks.
p.s. Usually there is a blue LED flashing on the BMS if the output voltage is correct but in my case it's flashing red. Sometimes when I plug/unplug the ribbon cable to the BMS I can make it flash blue for 2 seconds but then it goes quickly to red. If I can exclude that it's not the BMS how to find the error source?
![IMG_20181003_192757_HDR|365x499](upload://kOk8fzSJBGZkrymP7sBkMZe1M6F.jpeg)
```

---
## \#2 Posted by: Maxid Posted at: 2018-10-03T18:13:58.107Z Reads: 47

```
Tldr: the BMS on these scooters is known to fail. Try charging without it = directly to the main wires.
```

---
## \#3 Posted by: chickengun Posted at: 2018-10-03T19:09:16.157Z Reads: 37

```
Ok so I applied some force on the ribbon cable and now it's working. strange. It is not the bms, it's the connection to the bms. It's charging right now, will monitor...
```

---
