# Recommendations for replacement battery pack

### Replies: 3 Views: 503

## \#1 Posted by: bobkat Posted at: 2017-04-24T01:05:14.102Z Reads: 71

```
Hello friends!

So just to give a little background I have an esk8 setup I got about a year ago that is DIY but was pre-built to ride. It has a carvon v2 hub motor, vesc, and a 12s1p a123 26650 cell pack with BMS. After this winter I started riding again recently and ran into an issue where about 1-2 miles into the ride the board just cuts off and will not turn back on at all for a while even though its not reaching its cut off point or the voltage meter doesn't seem to go down all the way. After about and hour or 2 when I charge it, it starts working again. Now it has a built in BMS and I'm not sure if thats whats faulty or the cell's themselves. The pack is very similar in specs and setup to this although probably a slightly different model: https://victpower.en.alibaba.com/product/60437915682-800503104/Victpower_36v_lifepo4_battery_pack_36v_skate_board_2500mah_battery_pack.html

So after opening the pack and looking for loose connections I'm kinda lost as to what else I can do to fix the issue. Given that it is a cheaper pack I think just putting some money towards a quaility built pack might just be the better opition at this point. I was thinking of going with something from http://www.chiboards.com/ thats made from a member of the forums here. It looks like the cells are 18650 and have different voltages etc.

Basically my current setup could get up to 25mph and roughly 7 miles and I was hoping to keep that the same or more range is fine. Would a 12s2p 44.4v 5 AH or 10s3p 37v 7.5 AH setup be a better replacment and could anyone let me know additionally what I might have to change in the VESC if I get one of those two? I haven't connected to it yet and am still going through a lot of videos to try and learn its values properly so I don't mess anything up. I know the VESC currently operates in FOC mode.

Lastly thanks to anyone in advance for advice!
```

---
## \#2 Posted by: willpark16 Posted at: 2017-04-24T03:12:29.468Z Reads: 53

```
12s2p a123 will have more current
```

---
## \#3 Posted by: Namasaki Posted at: 2017-04-24T04:00:41.575Z Reads: 48

```
I would highly recommend finding out for sure what the problem is before replacing anything.
You need to get it connected to bldc tool and check settings and try to see if there is a Vesc error code.
If the whole system is powering down, that could be the bms protection circuit. It might be overheating or you could have 1 or more battery cells with low voltage.
If you have a multi meter, you could open it up and check the individual battery cell voltages.
```

---
