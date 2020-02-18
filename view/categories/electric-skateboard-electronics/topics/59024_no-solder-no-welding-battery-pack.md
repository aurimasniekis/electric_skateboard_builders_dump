# No solder no welding battery pack?

### Replies: 8 Views: 2527

## \#1 Posted by: Travo Posted at: 2018-06-15T17:17:45.514Z Reads: 231

```
Hello everyone, I was looking at building a 18650 10s battery like the one Mike Beard did in his [video](https://www.youtube.com/watch?v=-h0qhQqU2Sg) on Youtube.  I don't own a spot welder and have been told that soldering directly to the 18650 cells are not a good idea.  I'm going to use Samsung 30q batteries.  I was wondering if instead of soldering the batteries together I could use this [18650 Battery Case](https://www.aliexpress.com/item/-/32831937650.html) and then go about connecting them all together with nickel strips and finally put the batteries in after.  I'm no electrition by any means so I'm just curious to wether the battery holder would be able to hold up or if it would melt or if this is even possible. Thanks
![jpg_640x640|500x500](upload://qvtKxELhlWuAhDM6BD24nJ1udjF.jpg)![High-Quality-1-X-18650-Battery-Holder-SMD-SMT-Battery-Box-With-Bronze-Pins-Radiating-Battery|500x500](upload://juC8jKd986xgenRzKCrhu9o1cws.jpg)
```

---
## \#2 Posted by: wafflejock Posted at: 2018-06-15T17:23:47.590Z Reads: 220

```
http://www.electric-skateboard.builders/t/n-e-s-e-no-solder-module-battery-packs/36847 <-- can see the thread here on building packs without soldering/spot welding anything.  Never used one of these myself but just pointing you to people who have.  Being new to electronics I wouldn't say building your own battery is a great place to start (lots of room for tragic failure).  Personally use two 5S lipo I hook in series to make a 10S.  You could also do a set of 2S, 3S, or 4S to get a 9,10 or 12S pack made without worrying much about heat getting into the cells and damaging things.

---

Working with lipos the dangers are basically just the spark from high amp discharge if the exposed leads ever touch so be very conscious of not cutting through both wires at the same time and wrap one up with electric tape if it is exposed and not actively being worked on.  Other danger is in puncturing the packs since there isn't typically the same hard shell with LiPos (they are typically expected to expand to some degree when used and apparently gas builds up inside the cells).  I 3d printed some shells for my lipos there are also hard cover ones you can buy but depends on how you plan to attach them to your board what the best option would be.
```

---
## \#3 Posted by: Travo Posted at: 2018-06-15T17:40:12.676Z Reads: 200

```
Those battery packs look great I might actually give them a try.  I would use LiPo but I just find it very inconvenient to have to plug and unplug the batteries all the time as well as pop them out of the case to get them to charge.
```

---
## \#4 Posted by: wafflejock Posted at: 2018-06-15T17:43:54.859Z Reads: 193

```
I made them pretty easy to connect/disconnect that is a bit of a pain but I sort of prefer having the battery detached from the board while charging (just in case something goes wrong at least it doesn't take the whole board and both lipos with it immediately)

[3d printed swappable battery](https://photos.app.goo.gl/KzDYcYYeHPuD4u5e2)

[Editable Design](https://cad.onshape.com/documents/15cd342c90ae1b0b6fd666bf/w/40780c7d8d67fd69a32fbf6e/e/fe1a99d1423c52e012228250)
```

---
## \#5 Posted by: Travo Posted at: 2018-06-15T17:53:11.819Z Reads: 173

```
Wow that actually looks very clean and practical very well done!  How long does it take to charge the batteries in between runs?
```

---
## \#6 Posted by: wafflejock Posted at: 2018-06-15T17:57:53.211Z Reads: 178

```
If I drain them down all the way it's a bit over an hour and a half typically to juice each one up.  I have two chargers now since I also use them for charging my quadcopter lipos and didn't like having to wait so long to have everything ready to go.  My original charger was 80W so could charge at about 3.4-3.6A (21V) before it would start to overheat itself new one is rated for 500W so I can charge at a full 1C or 5A so can fill the whole thing in 1hr in theory but usually only drain them a bit over half way before recharging so usually about 45min per battery.

New one is this https://www.banggood.com/EV-PEAK-AR1-500W-25A-DC-1-6S-RC-Battery-Balance-Charger-p-1095822.html?gmcCountry=US&currency=USD&createTmp=1&cur_warehouse=CN&utm_source=googleshopping&utm_medium=cpc_ods&utm_content=heath&utm_campaign=pla-heli-us-pc&gclid=Cj0KCQjwx43ZBRCeARIsANzpzb8q6pkv9P4xQnHslSvmOtdWMpwnfdc8OZMI4Oqu6JnhsMm5lV7QX80aAm2bEALw_wcB been nice only down side is didn't come with AC->DC power supply so using my bench power supply to give it DC in at 36V

---

Actually just got 2 new batteries too but need to print them new shells and try them out, hope is I can keep a pair in a backpack and take longer trips without worrying about running out of power.
```

---
## \#7 Posted by: Travo Posted at: 2018-06-16T18:13:29.354Z Reads: 121

```
Sounds good I'll definitely be looking into it. Thanks for all the info really appreciate the help.
```

---
## \#8 Posted by: uigiroux Posted at: 2018-06-17T13:53:36.215Z Reads: 88

```
The N.E.S.E. modules have become even more user friendly now that they've made dual sided modules.  I requested a custom order where there would be the screw ports on both sides of the unit, so that instead of needing to use 12, or 10 modules to make a 10s__p battery pack, you can now order half the amount using his 2s4p modules.

![image|666x500](upload://tlzR0JefIGIMxvOSCtHCPJIAODf.jpg)

So this is the highest you can go, 8 cells, so you could do 10s4p, 12s4p (that's what I'm making), and all you need is 5 for 10s, or 6 for 12s.  Then you just use their small bus bars to connect the modules, and that's pretty much it.

Another huge benefit of this is that it makes it so you have no limitations when you fly with your esk8.  I think the law now doesn't allow for batteries larger than 99Wh, which almost all good batteries are larger than.  You just unscrew the bus bars that connects everthing together, and you are left with essentially individual cells.  Technically each pair would count as one battery, so it'd be 4p batteries of whatever cell you used.  Still, there's no cells in the world that are powerful enough that that would be a problem :slight_smile:  If you want something smaller than 4p, you could order a dual sided 6p module for Xs3p, 4p dual modules for Xs2p.

I originally intended to just build my battery myself to save a large amount of money, but once I saw they could make these with dual sided power connectors, I sold my spot welder and placed an order.  Message @agniusm he is the owner of the company and will work with you and answer any questions you have.  He's been very helpful and quick to answer my questions.  Good luck!
```

---
