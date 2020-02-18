# Anti Spark issue, need YOU!

### Replies: 2 Views: 62

## \#1 Posted by: JFK Posted at: 2020-01-06T18:40:22.680Z Reads: 23

```
Hi all,

First of all, I’m acoustician, not electronician (low skills), I did not plan to produce and sell AntiSpark !

I love DIY, so using my little cnc, I have made my first PCB for an AntiSpark, that I’ll use in my future projects.

I’m currently on a ESkate and a BoomBox for friends.

ESkate : 36V, 30A, 9.9Ah (10S3P), dual hub, 2xVESC 4.2.

BoomBox : 48V, 30A, 9.9Ah (13S3P), dual amp, DSP, BT5.0…

Using a Software, I have draw this schematic (Vedder's one) to get a PCB that I can mill :
![JFK_AntiSpark_Schematic|690x473](upload://pWDEO1LLofFUwdhsdHOMaUxDdbV.jpeg) 

The V1 is from the “automatic” PCB maker and the V2 is the same I have re-draw (R2 not on the photo):
![20200104_140002|690x388](upload://xkT57Qnm24zvC5rBoAZoTstjEQ4.jpeg) 

The V2 PCB, much more simple ! :
![20200104_131100|690x373](upload://qKKStdwspmXgUukbYF0LwJXCNcU.jpeg) 

Well ! First tests done @24v, 3A (lab power supply) with a 24v light bulb as a load.

Work perfectly, On, OFF, ON, OFF… Perfect.

But, I have an issue and need your help. (Same thing on V1 and V2…)

The second test I have done is with the BoomBox battery @49V charge.

Battery->BMS->AntiSpark->2x24v light bulbs.

Switch OFF, I connect the battery to the switch.

All is OFF, good.

Switch ON, all turn ON, good.

Switch OFF… It doesn’t switch OFF.

One of the 3 Mosfet stay closed, always the same one (close to the load).

It burn during the ON step, I have test from OFF to ON, then deplug the battery, the mosfet stay closed./is burned..

Thanks for your help :slight_smile:
```

---
## \#2 Posted by: PixelatedPolyeurthan Posted at: 2020-01-06T19:20:17.658Z Reads: 15

```
@Pedrodemio
```

---
