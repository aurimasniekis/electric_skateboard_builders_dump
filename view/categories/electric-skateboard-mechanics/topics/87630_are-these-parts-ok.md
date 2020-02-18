# Are these parts OK?

### Replies: 12 Views: 411

## \#1 Posted by: Michal Posted at: 2019-03-19T13:53:10.378Z Reads: 161

```
I want to make my first all terrain dual drive electric board on a budget. I am thinking of using the following parts:

(ESC)
https://flipsky.net/collections/electronic-products/products/dual-fsesc4-12-100a

(Motors)
https://www.ebay.com/itm/6354-6364-6374-6384-150-170-200-230-270KV-High-Efficiency-Brushless-motors/303074535503?var=602007163506
(the 6474 200kv variant)

(battery)
https://hobbyking.com/en_us/turnigy-battery-5000mah-5s-20c-lipo-pack-xt-90.html

(Trucks/wheels/pulleys/motor mounts)
http://www.diyeboard.com/11-offroad-allterrian-power-truck-kit-with-8-pneumatic-tires-p-709.html

Are any of the parts not OK? If so can you link better parts with a good price.
```

---
## \#2 Posted by: Linny Posted at: 2019-03-19T13:55:05.753Z Reads: 135

```
If you're gonna get Flipsky i'd say get the motors from them as well. Dual 6355 will do fine but if you want more power you can go dual 6374.

And stay the hell away from the diyeboard site
```

---
## \#3 Posted by: Andy87 Posted at: 2019-03-19T13:55:43.314Z Reads: 131

```
Take the 4.20 plus version. Seems to be more reliable. Motors I can’t say anything. Lipos i personally wouldn’t go below 40C.
```

---
## \#4 Posted by: Grozniy Posted at: 2019-03-19T15:12:16.440Z Reads: 116

```
If you haven't already, read this first
https://www.electric-skateboard.builders/t/is-diy-esk8-right-for-you/84563?u=grozniy
Second, buy cheap, buy twice.
Like @Linny said, stay away from that site.
Like @Andy87 said, for off-road go with 40c lipos at least.
Quality motors are Maytech or @JLabs motors. It all depends where you are in the world.  
User feedback says to not purchase 4.2 dual. But 4.2 plus maybe.
And the most important is safety gear. Medical bills are far more expensive and not so pleasant to have as just a broken board.
Also consider reading this series
https://forum./t/building-a-lightning-powered-murder-board-part-1/119?u=grozniy
```

---
## \#5 Posted by: brenternet Posted at: 2019-03-19T20:09:17.301Z Reads: 85

```
As the others have mentioned, the parts list is a bit weak overall. I would highly suggest a good further read and not to rush in to it. Trust me, you'll think you're ready to assemble and something will be missing anyway. Rushing will just waste money.

We can probably all attest to that :confused:
```

---
## \#6 Posted by: MysticalDork Posted at: 2019-03-19T22:04:23.071Z Reads: 75

```
5Ah of batteries is also a little small, especially for a dual setup. I'd recommend either bigger lipos or 18650s. Spend the money on a really solid battery, it's the heart of your build.
```

---
## \#7 Posted by: Gamer43 Posted at: 2019-03-19T22:10:03.656Z Reads: 73

```
Flipsky is currently working on a fix for the cutout issue for their 4.20 hardware versions.

Another member of this forum and I have verified that the proposed change (well, we figured it out in the first place) makes the 4.20 (original and plus) versions even more bulletproof than some of the best 4.12 hardware versions.
(By that I mean we ran +- 60A motor current on FOC with sensors, and full throttled the test board up a steep hill, ran this test several times)

I would wait until Flipsky implements the change, unless you are able to make the change yourself. It's not a difficult rework, but is very tedious, especially for those who may be less experience with SMD soldering.
```

---
## \#8 Posted by: Michal Posted at: 2019-03-20T07:12:23.576Z Reads: 62

```
Do you know when they will do this?
```

---
## \#9 Posted by: mishrasubhransu Posted at: 2019-03-20T08:03:23.594Z Reads: 52

```
What's the change?
```

---
## \#10 Posted by: meesie Posted at: 2019-03-20T09:49:56.666Z Reads: 47

```
if you're building an all terrain board i'd go with four of those lipo's. 2 in series 2 in paralel for 10s2p. MTB's need a lot of power so you'll need a big battery if you want some decent range. the ESC is not bad and as for motors go 190 or 170KV. buy your motors as big in size as your budget will allow
```

---
## \#11 Posted by: Gamer43 Posted at: 2019-03-21T04:55:28.318Z Reads: 35

```
We've been in contact with Flipsky, they haven't given us a timeline yet.

The change is swap out the 4.7ohm gate resistors with, if you have the plus version, 22ohm, if you have the original version, 47 ohm.

If you need I can show a picture of the resistors in question.
```

---
## \#12 Posted by: Michal Posted at: 2019-03-21T09:25:12.496Z Reads: 30

```
Thanks a lot for the answers, this will definetly help my build.
```

---
