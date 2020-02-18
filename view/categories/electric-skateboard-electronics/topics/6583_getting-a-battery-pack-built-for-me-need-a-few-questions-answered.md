# Getting a battery pack built for me. Need a few questions answered

### Replies: 8 Views: 952

## \#1 Posted by: Airmacx Posted at: 2016-07-25T06:17:28.540Z Reads: 78

```
So I bought 40 18650 Samsung cells. I was told 10s4p would be the best configuration for my single motor build. I have the Enertion R-SPEC 6372 motor. 

Because I don't have any knowledge or a workplace or even the tools to put a pack together, I'm getting someone I know to do it for me. He said he would help but he asked me a few things... 

"I see you have no pack protection circuit, I’d strongly suggest we include this rather than run the risk of your pack going the way of low priced hover boards.
 
Do you know the maximum current you expect to draw from your motor? This will help us decide on the nickel strip we use for welding as well as an appropriate battery protection circuit.
 
We can also help with a charger."

Before I reply to him I'd like to know what a pack protection circuit is? And about the maximum current, what does that imply? Thank you in advance.
```

---
## \#2 Posted by: Jinra Posted at: 2016-07-25T06:36:27.603Z Reads: 78

```
He's talking about a BMS pretty much. It helps prevent damage to your cells by managing discharge/charge currents and prevents voltages from getting too high or low. You should be good with a 60-80A max current BMS depending on your weight, terrain, and gearing reduction. For reference the VESC, if you're using it, handles 50A continuous (240A burst).
```

---
## \#3 Posted by: Airmacx Posted at: 2016-07-25T06:49:16.560Z Reads: 79

```
Oh thought he was talking about  a Bms, just didn't call it that haha. So I should say I want a 60-80 Max current or?
```

---
## \#4 Posted by: Namasaki Posted at: 2016-07-25T06:53:43.139Z Reads: 73

```
Sounds like your friend knows what he's doing.
You want a BMS (battery management system) 60-80 amp continuous current capability.
you will have to order it from China or get it on eBay.
If you get one on eBay, get it from seller called Supower.
They have quality.
At 10s you probably won't pull over 30amps from the battery.
But its a good idea to over build.
http://www.ebay.com/itm/36V-37V-42V-10S-60A-Lithium-ion-Li-ion-Li-Po-LiPo-Polymer-Battery-BMS-PCB-System/221769582503?_trksid=p2045573.c100033.m2042&_trkparms=aid%3D111001%26algo%3DREC.SEED%26ao%3D1%26asc%3D20131017132637%26meid%3D21e7469c7458459c8f12a9f7fd49a120%26pid%3D100033%26rk%3D7%26rkt%3D8%26sd%3D231538664490
```

---
## \#5 Posted by: Airmacx Posted at: 2016-07-25T06:58:46.913Z Reads: 65

```
Sweet. So I've replied to him, see what he says next. When he asked what Max current I want, 30 should be right yes?
```

---
## \#6 Posted by: Jinra Posted at: 2016-07-25T07:03:31.178Z Reads: 66

```
60-80 like we said :P You could probably get away with lower, but there's a chance your system will shut off if you ride the motor hard.
```

---
## \#7 Posted by: Namasaki Posted at: 2016-07-25T07:03:49.471Z Reads: 66

```
Max current could mean peak current.
You should think in terms of continuous current.
The cells your using should be 20amp continuous X 4p so the battery pack will handle 80 amp continuous
You can use a 60 amp continuous BMS
How heavy nickel strip you use depends on the capability of his welder
```

---
## \#8 Posted by: Airmacx Posted at: 2016-07-25T07:08:39.558Z Reads: 63

```
Thanks! And thanks to @Jinra too! I'll let you guys know how it all turns out . I have everything, my motor is en route to my place, the VESC is at the post office and I just ordered an enclosure from @MasterCho so things are finally arriving!
```

---
