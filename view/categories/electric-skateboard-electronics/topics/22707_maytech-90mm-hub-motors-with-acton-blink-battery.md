# Maytech 90mm Hub motors with ACTON Blink battery?

### Replies: 2 Views: 664

## \#1 Posted by: Tomer Posted at: 2017-05-09T08:07:34.010Z Reads: 104

```
Hey folks,

Long story short - I have an ACTON Blink belt version skateboard with a broken ESC.

I am going to use its parts to build a DIY skateboard. Right now I am expecting a Matytech VESC which I bought to arrive, and I am going to use the ACTON Blink motor and battery (with ACTON's charging port 
and ON/OFF switch).

I am thinking about changing the motor in the future to [90mm Hub motors also by Maytech](https://www.aliexpress.com/item/Maytech-longboard-electric-skateboard-90mm-hub-motor-and-back-truck-for-hub-motor-3pcs-10-OFF/32773154580.html?ws_ab_test=searchweb0_0,searchweb201602_5_10152_10065_10151_10068_5160014_436_10136_10137_10157_10060_10138_10155_10062_10156_10154_10056_10055_10054_10059_10099_10103_10102_10096_10147_10052_10053_10142_10107_10050_10051_10172_5150014_10084_10083_10080_10082_10081_10110_10111_10112_10113_10114_10181_10183_10182_10185_10032_10078_10079_10077_10073_10070_10123-10077,searchweb201603_2,ppcSwitch_5&btsid=0cb38b00-e042-4d90-a9bd-01017d62aba1&algo_expid=c43c71da-6649-479b-8545-e4b8c7200aa5-1&algo_pvid=c43c71da-6649-479b-8545-e4b8c7200aa5). In order to get top speed from it, I would like to know if ACTON's battery pack is good enough to deliver enough power to it? I am kinda new to all this and the only thing I know about the battery (from searching in this forum) is that the battery pack reads 41.4 volts at a full charge, and the pack is 72 Wh ([source](https://www.electric-skateboard.builders/t/acton-blink-board-modification/8623)).

Should I be okay? Or will I need to upgrade the battery pack to reach top speed? If so, to which one? 
And what do you guys think about these motors?

Thanks.
```

---
## \#2 Posted by: aigenic Posted at: 2017-05-09T11:23:23.313Z Reads: 79

```
Short answer: you would have to change your bttery...

YOur battery pack has capacity of 2Ah which is not much...If you could somehow find out its max discharge rate (in C or amps) it would help :)  But I think it wont be more than 30A (800W / 37V = 21,62 A) which is quite little :O  So if you upgrade to Maytech hubs you will get just half of its max power without damaging your battery (by my calculations, if the discharge rate is higher, it might be possible)
If you upgrade to maytech's you wont get better range, your max speed would be higher (34kmph: http://calc.esk8.it/#{"batt-type-lipo":1,"batt-cells":10,"motor-kv":60,"system-efficiency":90,"motor-pulley-teeth":1,"wheel-pulley-teeth":1,"wheel-size":90}| ) but the torque would suck due to low discharge rate of the battery. So it would be unnecessary for so big hub motor (80mm or even 70mm would be enough)

But if the battery has a higher discharge rate then it something completely different ;) 

Try asking ACTOn support, they might find out the discharge rate :) maybe it will be higher, but i dont think so :) 

EDIT: ACTON uses 10S1P configuration, to use Mtch you would have to lower amp rating in your VESC to just 30 A so the Maytech hub would give you just 1100W (and you cant be sure if it is really 30A and not 25A for example :D ) which is not worth the money...
```

---
