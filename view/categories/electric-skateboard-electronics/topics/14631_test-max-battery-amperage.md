# Test Max Battery Amperage

### Replies: 9 Views: 2945

## \#1 Posted by: deke997 Posted at: 2016-12-14T02:26:43.414Z Reads: 189

```
I have a bunch of unmarked 18650's that I pulled out of some laptop batteries I had lying around. I plan to use these batteries to test several different designs/configurations, but I need to know the max current that I can draw from them. I have been searching all over, but I can't seem to figure out how to test this. 

Just to be clear, I am not trying to test the _capacity_, I am trying to test the _max current_ that I can draw from them. For example, Samsung 25R's have a capacity of 2500mAh, but the max current is 20A.

Does anyone know how I can test these batteries? Technical responses are welcome.

UPDATE:
I found  a bunch of old batteries at a thrift store in my town. They couldn't sell them, so they let me have them for free! I have taken about half of them apart, and I have about 50 cells so far. I have a LUC V6 charger from [Li-Ion Wholesale](https://liionwholesale.com/collections/chargers/products/efest-luc-v6-6-bay-lcd-and-usb-li-ion-battery-charger?variant=16915974852), and I used it to charge up all the cells individually. It has an "activation" feature that is supposed to bring cells back from the dead, and it's working great! Most of the cells were around 2.9-3.0 volts, but a few were at 2.0 volts and under. The charger was able to bring back almost all of the cells. I have only found 3 completely bad cells so far.

Everything is reasonably holding a charge so far. I just started testing my cells with a 1157 style light bulb. This light bulb has two filaments, the smaller of which draws about 0.5 Amps at around 12 volts. I wired up my sleds so that I have 3 cells in series to get close to the voltage, and I have 2 of these sleds in parallel. This results in the load on each cell being about 0.25 Amps. I have two multi-meters set up; one to monitor voltage and one to monitor amperage. The amperage drops as the voltage drops. It starts at 0.52 Amps, and it ends at 0.45 Amps, but the difference negligible for my tests. I will attach pictures of my setup to this post.

So far, I have just been testing the capacity of these batteries. I wasn't expecting much, but they are performing much better than I thought they would. I will be posting the results of my tests for each one.

Panasonic CGR18650A
2000mAh
Max Current: Not yet tested
Tested Capacity: 1083mAh
I tested these cells at 0.5 Amps, and they lasted a little over 2 hours. I did not have two sleds in parallel when I tested these, so the amperage is twice as much as the rest of the tests. I will test again at 0.25 Amps when I get a chance. These cells are the oldest of the bunch, and they appeared to be the worst in terms of holding a charge. A day after I charged them, they dropped to about 3.95-4.00 volts and then stayed there.

Samsung 26D
2600mAh
Max Current: 5.2A
Tested capacity: test in progress
I am testing these cells at 0.25 Amps. The are performing well so far. After charging, they stayed at around 4.13 volts. At full capacity, these cells should last this test for 10.4 hours. It has been 4.6 hours so far, and they are not even halfway depleted. They are currently at 3.735 volts.

<img src="/uploads/db1493/original/3X/5/2/524eee9661dd649672ccea8a26b082ebb123ba04.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/6/7/6718ca8bb223cb7f5f089a1b863f9a24f5b0c1f7.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/d/5/d5ef8d0da80fbcd9950ec81128c80a7382530547.jpg" width="690" height="388">
```

---
## \#2 Posted by: Okami Posted at: 2016-12-14T09:02:04.749Z Reads: 156

```
You can try to hook up some 12v headlights and then see do they bear the load.. though, you will probably need an amp meter (like a multimeter) or a wattmeter.. 

_Though, for this you will need 3 cells in serial, to get the desired 12 or so volts, so maybe even 4 work. You should get about ~4.5a draw from single 55w headlight, if the cells can give off such current. ~3.9 draw if the headlight works with 4cells in serial._ 

Multi meters usually dont allow current to be bigger than 10A.. otherwise they burn out or something (has not happened to me yet).. so if you want to test more than 10A in single setting, you probably need bigger amp ampmeter and then get a load which is also so big.

I can direct you to this (ES forum): 
https://goo.gl/r1fjE9

He used sleds, so that he can pop out a cell, if it goes bad. I believe that at least a few cells of his monstrous pack went bad over time.

Here's a quote from him:

> I have yet to find any laptop cell that can't withstand 2C. Also, since they are used and free, burn 'em up. LOL! Who cares if they can't take the load. THEY ARE FREE!!! I run 12P at 50 amps or slightly over 2C 100% of the time. It works quite well. On a hot summer day where I live it gets to 100F. The batteries rarely get above ambient. IE: You can run them harder than you think. Don't bother with thinking in terms of 1C just because that's all the more a laptop might draw.


It was kind of revealing to me.. did not know that laptop cells can be ''punished'' so much, that they might even offer 4A-5A easly or even more. They do get warm of course but not burning hot.. at least that's what the guy on that thread says..
```

---
## \#3 Posted by: Okami Posted at: 2016-12-14T09:12:43.401Z Reads: 114

```
So yeah, I assume you would need to strive for 4P - 5P config at least to be able to test it on a board.. Though, you are welcome to test out 2P or 3P config as well and report how much power / speed you actually had with such batteries..
```

---
## \#4 Posted by: Ackmaniac Posted at: 2016-12-14T09:46:59.152Z Reads: 107

```
Out of my 8P pack i can draw 80 - 85 amps. Then they sag from fully charged to 2,66V under load. So that is the maximum you can do to them. So roughly you can say that you can draw 10 Amps from them. They get warm but not hot. But of course we don't draw max amps constantly from them. If you would draw that much amps constantly then they would get very hot. But on a longboard it is fine with 12S8P. 
For example from a Samsung 25R cell you can draw much more than 20 amps as long as you don't do it continuously.
Samsung says 95A for less than 0,5 seconds. And some make discharge tests at 35A continuously (not recommended).

Maybe you can get away with a 12S4P if it is a cruiser for the flats. But i would not recommend it. But those cells were already declared as dead. So who cares.
```

---
## \#5 Posted by: deke997 Posted at: 2016-12-14T15:40:13.659Z Reads: 94

```
I have a multi-meter that can do 10A, but I don't want to risk burning something out (I know it's a very small risk, but still, the multi-meter I have isn't mine, and it's expensive..). I'm considering calling up a batteries+bulbs store to see if they have equipment to test these with. From what I'm reading from you guys, though, I should expect to get 4-10 Amps, right?

The headlight idea got me thinking. Could I just get a few different bulbs of increasing wattages, and then see where the brightness stops increasing? I think this would give me the max current, but not the max continuous current. If I were to monitor the temperature while doing this, I could then find which bulb it could power continuously without getting too hot, which would also give me the max current, correct? BTW, what is a good temp range for 18650's?

 I am also using sleds right now, at least for testing. I'll have to see if they can handle what I going to do to them in the future. My final build will probably require a lot of amperage at times. I'm doubtful that they'll be used in the final build because they take up a lot of space, and I'm not sure that the spring connections will be able to handle a large amperage without getting hot. I'll have to test to find out. I have access to a battery spot welder, so I'll probably end up going that route in the final build.
```

---
## \#6 Posted by: Okami Posted at: 2016-12-14T15:52:55.234Z Reads: 81

```
For continous I think you should expect 2-4A for them to work somewhat okay also in the longterm..

10Amps is the maximum they can deliver for a short time.. I assume that if you tried to pull 10A for longer period of time.. the cells would just get ''weak'' - sag, like @Ackmaniac mentioned..

Im not sure about that wattage thing you plan to do..

I only assume you will take 20w - 30w - 50 w, perhaps 100w bulbs and then see how much current the cells deliver and how high they get..

Check what happens if you add 2 bulbs in parallel, I think that you could somehow decrease the amps this way, as the resistance is smaller. But you should check as Im not sure does it work 100% like a resistor (the lightbulb filament)..

---

Spot welding sounds okay but in your case I would run the cells in sleds for about a month.. if none of them shows signs of extra heat or decreased life.. then you could spot weld them together.. The guy who pushed his e-scooter very hard, had to replace a few cells, they just did not charge high enough, he said, I think.
```

---
## \#7 Posted by: deke997 Posted at: 2016-12-14T18:12:58.899Z Reads: 68

```
I will get some stuff together today and start testing. I'll update when I have some more info.

I should clarify, however. I do not plan on using these cells for my final build. I am trying to test a variety of different wheel and motor configuration to see which one best fits my needs. Once I know my wheel and motor configurations, then I will know what specs my battery needs, and then I can pick the cell that will meet those specs most efficiently. I am building my battery for my board, not my board for my battery. I am using these cells to simply test my configurations because I do not want to waste $100 on 25R's if another cell ends up working better in the end.
```

---
## \#8 Posted by: Okami Posted at: 2016-12-14T18:40:42.939Z Reads: 59

```
Good thinking. I think is has not been massively de-bunked whenever you need 40A or 60A or what amps cells for riding the board..

Wish you Good work then and I hope you manage to pull together some data / tests, to see which config/ how many amps/ cells are actually needed for you!
```

---
## \#9 Posted by: jmasta Posted at: 2016-12-14T21:12:04.288Z Reads: 53

```
I use this inline power analyzer / wattmeter:  https://www.amazon.com/Tenergy-Precision-Meter-Analyzer-Backlight/dp/B017YCTRKK

It will record peak amps, in addition to many other variables.  I added XT-90 connectors to each side so I can easily add it to the system for monitoring.  Usually it will live on my charger however
```

---
