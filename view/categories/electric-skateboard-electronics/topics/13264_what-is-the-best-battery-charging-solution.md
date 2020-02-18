# What is the Best Battery Charging Solution?

### Replies: 26 Views: 2853

## \#1 Posted by: jonfmalm Posted at: 2016-11-18T06:50:50.707Z Reads: 305

```
Hey, all. Without doing the math, I originally went for a 6S 2A balance charger, because it was cheap, like 20$... but now I'm regretting it because with my 12S2P 5000mAh setup and parallel charging, it looks like it is going to take 15-30 hours to charge those mother---s.

Right now I all I could find on the sub is the Turnigy Reactor, but it's like 100$+, and basically I'm thinking that LiPo chargers like this should not be that expensive. 

How do you guys charge your batteries?
```

---
## \#2 Posted by: Jinra Posted at: 2016-11-18T06:54:53.234Z Reads: 303

```
It definitely shouldn't take 15 hours to charge. Assuming you're charging 10ah at 2amps, it should only take you 4-5 hours at most
```

---
## \#3 Posted by: jonfmalm Posted at: 2016-11-18T07:02:20.130Z Reads: 300

```
I'm charging 12 2S 5aH batteries in parallel, so it would be like 60aH? Regardless, 5 hours is far too long, ideally 1 hour approx.
```

---
## \#4 Posted by: Jinra Posted at: 2016-11-18T07:09:09.892Z Reads: 296

```
Ah I see, yea it's charging slow due to lower voltage. You should just connect 3 of them in series and charge at 6s with 2 packs. Slower charging is better. You could charge each 6s pack in an hour with a 5A charger, but you'll most likely only find 4A chargers out there, which will still be fairly fast. Like I said though, slower charger is much better for the battery. I don't know about your situation, but i rarely ever go from 100 to 0 to do a full charge. In fact my battery's never been below 20%. Only takes me 2~ hours to charge my pack. I'm running 10s @ 10ah
```

---
## \#5 Posted by: jonfmalm Posted at: 2016-11-18T07:38:38.819Z Reads: 282

```
I'm using a 5A charger, but the maximum W is 50, so for each 6s pack I would only be putting out 2A, so it would take 2.5hrs per pack. or 10 hours altogether.
```

---
## \#6 Posted by: jonfmalm Posted at: 2016-11-18T07:40:25.242Z Reads: 273

```
I've heard of people using constant power supplies with a BMS, but the BMS is huge once you get up to 12S, and definitely not worth putting on the e-board.
```

---
## \#7 Posted by: Okami Posted at: 2016-11-18T09:32:32.165Z Reads: 271

```
I think the turnigy reaktor is the best bet there is.. u can apply to search for used ones on ebay.. and once a new listing is there, you will receive an email..

I think there were some in pretty decent shape for about ~50usd +/- shipping.. Though, you also need a power supply but I think you can modify a PC one, if you dont intend to carry it around with you and charge outside of home..

Btw - there's also this program called ''Calc RC''
It is quite useful as it allow to calculate the wattage and time it would take to charge the batteries!
```

---
## \#8 Posted by: yaca Posted at: 2016-11-18T10:26:42.306Z Reads: 251

```
Just for to see an other possibility: I charge my 10s 5100 mAh battery with a dual charger 2 x 100 W in 1 hour.

I have to seperate the 2 x 5s lipos with this connector at first:

<img src="/uploads/db1493/original/3X/9/4/948e7924557f5749bf72f8fd3f188b09e6f05d6c.JPG" width="690" height="460">

and that's how I charge:

<img src="/uploads/db1493/original/3X/0/0/00d3c83ef8973f564c96393736e3cc1d7e6e4bfa.JPG" width="333" height="500">

The only problem is the price of the charger. But I use it for many rc batteries so I need it.
```

---
## \#9 Posted by: B4Me Posted at: 2016-11-18T12:33:15.662Z Reads: 222

```
Dosnt have to be huge ? :slight_smile:

http://raphaelchang.com/projects/bms/
```

---
## \#10 Posted by: TarzanHBK Posted at: 2016-11-18T14:21:01.851Z Reads: 216

```
hope this awesome thing is available soon!
```

---
## \#11 Posted by: B4Me Posted at: 2016-11-18T14:27:52.904Z Reads: 215

```
I think the design is open sourced on this forum have a search on "raphael" bms
```

---
## \#12 Posted by: TarzanHBK Posted at: 2016-11-18T14:40:36.252Z Reads: 211

```
yah i know, i ment pre assembled and ready to go version to buy. I mean I´m good with soldering cables and small things, but this pcb is next lvl shit :D
```

---
## \#13 Posted by: Hummie Posted at: 2016-11-18T14:40:56.243Z Reads: 209

```
Meanwell power supply and do 12s all in series at 400 watts with one main battery plug. Use 12$ battery medic like device for balancing on the side.  30min.  Still at 1c charge rate.
```

---
## \#14 Posted by: Okami Posted at: 2016-11-18T22:20:55.480Z Reads: 198

```
What's the typical price for such unit?

Does it beat this:

http://www.ebay.com/itm/TURNIGY-DC-Charger-20-AMP-LiPo-400W-Reaktor-VENOM-SKYRC-iMAX-HiTec-/222060730151?hash=item33b3d9d727:g:a3QAAOSwe7BWxInY

As it is 6s charger, you will have to split the pack.. and max charge per pack will be 10A + a PSU is still needed..

I think it has enough amps (10A for each 5-6s'' pack would equal to 2c for 5ah pack, 1c for 10ah pack)

--

Of course I take maximum ratings but I think the charge time would not be that bad, when charging at 1c..
```

---
## \#15 Posted by: Okami Posted at: 2016-11-18T22:27:38.732Z Reads: 185

```
At what amps do you charge? Im running 6s, so cannot tell by sight how much that would be.. :D
```

---
## \#16 Posted by: yaca Posted at: 2016-11-18T22:50:41.483Z Reads: 186

```
I charge at 1C, that's 5100mA. For one hour charging I would need in theory 2 x 107 watts (5s X 4,2V X 5.1 A) Just have 2 x 100 watts, so maybe it needs a bit longer, but usually I don't run them completely empty.
```

---
## \#17 Posted by: Okami Posted at: 2016-11-18T23:52:06.546Z Reads: 173

```
Thanks for response. So yeah, each ''module'' of 100w, delivers about 5A.. which seems correct.

About 10A in total then..

What PSU do you use? Do you have a commercial one? I assume.. it runs 200w+ (to supply the 100 x 2)
```

---
## \#18 Posted by: Hummie Posted at: 2016-11-19T03:43:45.152Z Reads: 157

```
@Okami are u asking me?  The meanwell is maybe 60$
This thing you put up seems nice maybe but I'd much rather have a single plug that does 50.4 volts.  
And these cheap things on the side to see what's happening and balance. 400 watts at 50.4.  I'm sure there's other bulk chargers that could do way more watts too. I forget what model I have..nothing catchy
https://hobbyking.com/en_us/turnigy-dlux-lipo-battery-cell-display-and-balancer-2s-6s.html
```

---
## \#19 Posted by: Okami Posted at: 2016-11-19T09:42:38.902Z Reads: 150

```
yeah, it was directed at you, sorry for not ''marking the reply''.

I agree it can be more convinient to have just one setting and that's all. Though, if someone has more than one battery to charge, it is probably nicer if there are some options to regulate the voltage / current.
```

---
## \#20 Posted by: yaca Posted at: 2016-11-19T10:00:46.696Z Reads: 143

```
My dual output charger runs AC/DC, so it has a build in power supply. At DC it has 200/100 watts, at AC 100/100 but also I can change to 200/0 watts or 150/50 watts and everything between.
```

---
## \#21 Posted by: Okami Posted at: 2016-11-19T13:53:52.448Z Reads: 135

```
Have you tried to charge just through DC ? Have you speculated how it would be to charge your main pack from a weaker pack while outside?
```

---
## \#22 Posted by: yaca Posted at: 2016-11-19T15:45:19.352Z Reads: 136

```
Not sure if I understand, but charge through DC means you need an extra power supply or a  car battery. Charging with an other battery on the outside like a powerbank? Never thought about that.
```

---
## \#23 Posted by: rasmukri Posted at: 2016-11-19T16:03:19.386Z Reads: 133

```
I have a 10s balance battery charger. So I just plug in my balance leads and the main power I charge at 3.5 amps it goes full charge in about a little over an hour. But u also only go about 50% on the battery before I charge. About a 7mile ride takes 3700mAh and I have a 9s4p homemade 18650 battery that has a max power of 8200mAh.
9s you may ask? Well it was 10 but I had a bad cell so I just hacked it off and called it a day.
```

---
## \#24 Posted by: Okami Posted at: 2016-11-19T17:29:29.723Z Reads: 126

```
Yes, you got it right. A powerbank to carry along
```

---
## \#25 Posted by: yaca Posted at: 2016-11-19T20:24:53.753Z Reads: 122

```
I think this is not really a good idea, because when you connect an extra battery to fill the onboard battery it will just flow from one to the other till both batteries have the same voltage, so you can not charge it completely.
```

---
## \#26 Posted by: Okami Posted at: 2016-11-19T21:07:15.323Z Reads: 128

```
This is why you would need a step down module and design a pack that has higher voltage than your board's pack.. 

If you got 6s board battery voltage, then choose 8s for powerbank, to include the 1.5v drop from the lowest voltage point it will have (about 26.4v in my case (3.3v x 8)).. if you subtract 26.4 - 1.5 = 25.3, which would translate to about 4.21v for 6s battery.. which would be just great. 

Though, in my opinion, this only works great if you got plenty of laptop batteries (cells) or you got some other odd battery which can not deliver a lot of amps (to be used as the main battery)..

---

So yes, you would not connect it directly.. that is probably not a good idea.. someone has to find a source how much amps does flow from one battery to another in such a scenario...

----

Another option I discussed is to use a current limited step - up module. This would enable to use all sorts of laptop chargers or just a smaller voltage powerbank, to step up the voltage to the desired charge voltage.

----

I know not many is gonna go this route.. I just like the idea about using both laptop batteries and also be able to charge my board elsewhere.. without actually always taking the powersupply with me.. if the module weights around 200g, that is not a that big burden to carry with you..

---

Basically, all smart balance chargers are voltage step - up modules... they take less voltage and 'boost it'' to higher voltages levels. That's also why there are usually some cooling as things get hot there.
```

---
