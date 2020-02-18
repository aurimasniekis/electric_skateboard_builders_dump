# How can I change the battery indicator on my diyeboard ESC/Battery?

### Replies: 28 Views: 1995

## \#1 Posted by: queue_together Posted at: 2018-02-01T04:06:23.323Z Reads: 216

```
The battery indicator doesn't work so I'd like to swap it out, prefferably with something like this:
https://www.amazon.com/Universal-Voltage-Type-Indicator-3-15cells-Lithium-Ion/dp/B078GPQRQP
That displays a percentage rather than voltage.. Unless I should be displaying voltage?

Do I just remove the pre-installed adapter on the cables and solder the new indicator directly? Is there an alternative to soldering that wouldn't be permanent?
```

---
## \#2 Posted by: queue_together Posted at: 2018-02-01T04:07:06.883Z Reads: 208

```
Here is a picture of my battery
![image|500x500](upload://bBe2pDdCITxD5RIrmEoDMkDqSI0.jpg)
```

---
## \#3 Posted by: Namasaki Posted at: 2018-02-01T04:54:17.713Z Reads: 190

```
I changed mine from percentage to voltage because in my opinion, its more important to monitor your battery's voltage.
```

---
## \#4 Posted by: pennyboard Posted at: 2018-02-01T05:05:14.876Z Reads: 190

```
You have to solder that monitor across the battery cable, so that it is in parallel with the XT60. You won't be able to plug that battery monitor directly into the esc
```

---
## \#5 Posted by: pat.speed Posted at: 2018-02-01T05:07:42.637Z Reads: 189

```
He will also need a switch then so he can turn the monitor off. Dw he might have an antispark.

I think there must be two pins on the esc to read voltage though because how would the stock meter read it
```

---
## \#6 Posted by: pennyboard Posted at: 2018-02-01T05:10:09.828Z Reads: 181

```
Yeah he'll deffinetly read the switch. I have the same monitor and esc, and tried to hook it up to the esc's battery monitor hook up, but after inspecting all the pins using a DMM, i couldn't figure out which one, if any, directly outputted voltage. I didn't that hard though so maybe someone else will have better luck with it than me
```

---
## \#7 Posted by: queue_together Posted at: 2018-02-01T05:14:35.787Z Reads: 175

```
I found one that has a sleep mode built in, maybe I could try that

https://www.ebay.com/itm/12V-48V-Waterproof-LCD-Indicator-Battery-Capacity-Tester-Lead-acid-Monitor-BI753/311945713954
```

---
## \#8 Posted by: queue_together Posted at: 2018-02-01T05:15:48.849Z Reads: 166

```
So you can't read battery from the remote only from the monitor?
```

---
## \#9 Posted by: pennyboard Posted at: 2018-02-01T05:25:53.277Z Reads: 164

```
Installing a new monitor shouldn't change the battery read-out on the remote, assuming the remote already has a battery read-out built in. 
You're not trying to instal this battery monitor on your remote are you?
```

---
## \#10 Posted by: Bjork3n Posted at: 2018-02-01T05:38:36.624Z Reads: 166

```
Hey! I did exactly this to my diyeboard kit. 
Just do a small cut in the wires behind the xt60 connector and solder the wires to the cable. 

Very easy and works perfectly . 
See pictures.![received_10155039281092078|281x500](upload://jsARrSByfkP0DCrN8KCsNAtNsPq.jpeg)![received_10155039316962078|281x500](upload://yvC5Y311aTYvTDAQWa5n8TqwqBV.jpeg)![received_10155039323707078|281x500](upload://87YcD9XZpjGnh3X8pX7feqlNTjz.jpeg)![received_10155039342557078|690x388](upload://95U9c3uHiZkH4ZPJHAW2Cs8Dai4.jpeg)
```

---
## \#11 Posted by: queue_together Posted at: 2018-02-01T05:54:27.760Z Reads: 155

```
Thanks for the reply, 

Something like this?
![image|690x289](upload://qjuHNPKh7TxMrg7IYLUycKypMlk.png)
```

---
## \#12 Posted by: Bjork3n Posted at: 2018-02-01T06:27:43.218Z Reads: 148

```
Yeah you could do like that also. 
I however attached it to the cable that is between the esc and male xt60 connector.
This way you can swap batteries and have the indicator work no matter what battery you use :slight_smile:
```

---
## \#13 Posted by: queue_together Posted at: 2018-02-01T06:43:36.625Z Reads: 149

```
How does this look

![image|690x261](upload://4f51TDl5pWRJyN8KVtiNO2i5YvO.png)
```

---
## \#14 Posted by: Bjork3n Posted at: 2018-02-01T07:10:13.388Z Reads: 149

```
![Battery indciator|657x500](upload://wi90Vwve4H8NWv718RS6m9dUvqK.png)

Like this
```

---
## \#15 Posted by: queue_together Posted at: 2018-02-01T16:24:21.158Z Reads: 128

```
Ok sweet that's essentially what I was thinking of with my second picture, I think we just had things flipped horizontally.

Never really done too much soldering in the past so this will be a challenge for me. Just solder and wrap up in electrical wire?

Is your indicator on all the time? Have you noticed any significant battery draw from it? Probably not right
```

---
## \#16 Posted by: dspx Posted at: 2018-02-01T17:56:28.773Z Reads: 126

```
Chiming in. 
I tested the same battery capacity/voltage gauge and this similar meter: https://www.amazon.com/gp/product/B071HW4QHL/ref=oh_aui_detailpage_o03_s02?ie=UTF8&psc=1

At least for me, the DROK meter was much more accurate when I compared its readings with the readings from my multimeter. The other tester was outputting 0.4 volts higher, even after I configured it to match my battery pack. Could be an isolated incident *shrug*.
```

---
## \#17 Posted by: queue_together Posted at: 2018-02-01T18:26:11.626Z Reads: 125

```
Is there any noticeable battery drain due to the battery indicator since it is always on?

Are you still using the DROK? Get's the job done?
```

---
## \#18 Posted by: dspx Posted at: 2018-02-01T22:04:10.389Z Reads: 120

```
Well, admittedly, I've only tested its initial accuracy.. haven't installed it yet to test its effect on the battery. Not 100% certain, but it might be possible to restrict power to the monitor by soldering the positive lead to the output of your power switch instead of the battery. I have no practical knowledge of this, just something I read in the Q&As on the amazon page.. maybe someone else can confirm?
```

---
## \#19 Posted by: pennyboard Posted at: 2018-02-01T22:45:43.893Z Reads: 112

```
Just a heads up, if you instal the indicator that way, you Need an on/off switch for it. I've seen battery's completely ruined because an indicator was left on for 3 days. It doesn't use a lot of power, but over the course of days, it Will drain your battery
```

---
## \#20 Posted by: queue_together Posted at: 2018-02-02T00:45:59.121Z Reads: 111

```
I wonder if anyone sells indicators with switches built in
```

---
## \#21 Posted by: pennyboard Posted at: 2018-02-02T02:09:20.794Z Reads: 98

```
You can pick up a switch at Lowe's or Home Depot for like $3
```

---
## \#22 Posted by: telnoi Posted at: 2018-02-02T06:01:42.952Z Reads: 100

```
Be careful which one you buy, not all of them are waterproof..and from what I remember the voltage reader can be connected directly to the diye Esc, allowing it to turn on via the switch. Just use the original connection of the old one.
```

---
## \#23 Posted by: queue_together Posted at: 2018-02-02T23:41:06.980Z Reads: 100

```
Can I wire it to the power switch that came with my esc?
```

---
## \#24 Posted by: queue_together Posted at: 2018-02-03T04:30:23.844Z Reads: 98

```
@telnoi elnoi The connection on my esc for the battery indicator is a 5 pinned connection

![received_10157107667464922|690x387](upload://oHKlcIpjG6BJvXooTOZPegoARUu.jpeg)
```

---
## \#25 Posted by: telnoi Posted at: 2018-02-03T07:26:11.373Z Reads: 93

```
No. How was the original voltage reader connected? Just replicate the original connection.
```

---
## \#26 Posted by: ARetardedPillow Posted at: 2018-02-03T08:16:31.490Z Reads: 93

```
I would just get a bluetooth module, its cheap, easy, and it gives accurate info unlike some indicators that shows percentages

Just realized that a bluetooth module is cheaper than an indicator
```

---
## \#27 Posted by: Bjork3n Posted at: 2018-02-03T09:32:28.089Z Reads: 87

```
Just use this indicator @queue_together.
It has a auto turn off feature so it wont drain the battery continuously.
I have this indicator installed on 2 of my boards, works great!

https://www.ebay.com/itm/12V-ACID-LED-Lead-Battery-Capacity-Indicator-Charge-Power-Level-Tester-Voltmeter/232568974492?hash=item362630ec9c:g:rNEAAOSwUnFZtejy.
```

---
## \#28 Posted by: dspx Posted at: 2018-03-27T04:14:10.339Z Reads: 78

```
Just following up for anyone still curious. The battery drain is unnoticeable - my board has been idle for a few weeks and the percentage has remained the same. The DROK has a stand-by setting that uses a negligible amount of power until activated. I have it connected directly to the battery.
```

---
