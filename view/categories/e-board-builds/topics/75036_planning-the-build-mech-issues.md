# Planning the build - mech issues

### Replies: 22 Views: 586

## \#1 Posted by: Euformelo Posted at: 2018-11-17T22:09:53.425Z Reads: 159

```
Hi people from forum!

I'm trying to build a first all terrain skateboard with following equipment that I have for now:

Motors:
2 x 280KV 5055 SK3 motor (I know it is high KV but will try to get more torque with gearing)

Battery:
I've got 2 x 5000mah 6S, will use them in parallel, if it's gonna be to low can go with series then step down voltage a little bit. Later will trey to build my won battery 10S.

ESC:
Maytech SuperESC (VESC)

Wheels:
200*50 pneumatic ones

Gears:
Gearing will be 'direct drive' - helix gears (not really good with this one).

Deck:
Will try to get drop down one or one like [this](https://www.electric-skateboard.builders/uploads/db1493/original/3X/c/2/c287694097ada2394d7ba84c017c1f66d11393be.JPG) if found one in EU.

Tracks:
Unknown
.............................................................................................................................................................................

Ok, now the questions:

1. Drive train, I want to model all gears first helix ones and then send them to CNC.
I decided to go with 60T on wheel and 10T on motor gear. 105mm is the full diameter of the gear not reference  one. What do you think about this? Ratio ok?

2. Tracks - wheels have 10mm shaft where i can find them in EU?

All in all thank you for your responses and help up front and my apologies if this topic should be on other place.
```

---
## \#2 Posted by: Grozniy Posted at: 2018-11-17T22:30:54.677Z Reads: 135

```
Use this for all your calculations. Keep in mind to have ERPM less than 60000.
https://www.electric-skateboard.builders/t/new-esk8-calculator-in-wild/74497?u=grozniy
```

---
## \#3 Posted by: Grozniy Posted at: 2018-11-17T22:31:53.724Z Reads: 120

```
You need trucks  with 10mm axles?
Search trampa, mbs, or surfrodz.
```

---
## \#4 Posted by: Euformelo Posted at: 2018-11-18T18:43:45.493Z Reads: 105

```
Hi @Grozniy, thank you for your answer. I've un destood the first part about gears.
 
Trampa is too expensive :sweat_smile:, MBS and surfrodz are in US. Do you know any shop for Deck and tracks that is in Eu and a little bit lower prices?

All in all what do you think about this configuration?

Thank you upfront
```

---
## \#5 Posted by: Grozniy Posted at: 2018-11-18T18:53:27.233Z Reads: 95

```
https://mbseurope.com/
https://www.sickboards.nl/
Ebay
```

---
## \#6 Posted by: Euformelo Posted at: 2018-11-22T22:08:30.431Z Reads: 77

```
Hm looked at that one, still to expensive.
What about [this one](https://www.ebay.co.uk/itm/Flip-Mountain-Vato-Gold-Foil-Deck-Purple-9-0/192670555262?hash=item2cdc0f5c7e:g:udgAAOSwmMNbx0tq:rk:1:pf:0) is 32.5inch to short?
```

---
## \#7 Posted by: brenternet Posted at: 2018-11-22T22:22:16.003Z Reads: 72

```
While you're here looking for advice. I'd start with the golden rule.

Buy cheap buy twice. Building a custom esk8 is almost always more expensive than buying a pre-made. If you skimp on quality and compromise on parts to save $10 here and $15 there you will be re-building that board in 3 months time.

Please trust.
```

---
## \#8 Posted by: Grozniy Posted at: 2018-11-22T23:09:50.879Z Reads: 66

```
That is not mtb deck.
Also @brenternet is right.
I don't understand how all the parts are expensive for you since you're opting for custom CNC gear drive that is at least 300€ :thinking: 
Give us your budget, what parts you already have
```

---
## \#9 Posted by: Euformelo Posted at: 2018-11-23T06:45:48.062Z Reads: 54

```
@Grozniy Hi Grozniy, thing is that I have access to CNC so its not that expensive for me.
All the parts are mentioned at beginning.
Thank you for you help
```

---
## \#10 Posted by: Euformelo Posted at: 2018-11-28T15:04:47.544Z Reads: 51

```
Hi Gents,

there is no MBS 95 on stock in the shop. Is [this](https://www.coronation-industries.de/shop/en/mountainboard-deck/10063-mbs-core-94-mountainboard-deck-only-axe.html) one ok or should I wait for 95?
```

---
## \#11 Posted by: mmaner Posted at: 2018-11-28T15:07:31.452Z Reads: 48

```
Thats a different shape from the 95, but it should work the same.
```

---
## \#12 Posted by: rich Posted at: 2018-11-28T15:28:07.781Z Reads: 47

```
Be careful to choose the correct deck because you should use 35° channel trucks. Some decks are made for kiteboarding which means for 15-20° skate trucks. If you mount a channel truck on a deck made for skate trucks the steering won't be too good.

If you want to save money buy MBS Matrix II trucks, they are also fine for gear drive.

5055 motors on 6s for 8" pneumatics? That doesn't sound good at all. I would buy 6374 motors before you design the gear drive and go with 10s or 12s, better NOW than later.

[quote="brenternet, post:7, topic:75036"]
Buy cheap buy twice
[/quote]

100% agree, or even 3 times :wink:
```

---
## \#13 Posted by: Euformelo Posted at: 2018-11-28T17:27:18.429Z Reads: 46

```
Thank you guys for helping, @rich if I go now with 6374 192Kv motors I need to change VESC and motors will be limited to 50A continous...? Do I need to change VESC also then?

Will try to find MBS 95 then, somwhere else in EU warehouse
```

---
## \#14 Posted by: rich Posted at: 2018-11-28T18:35:47.116Z Reads: 50

```
192kv - 200kv would be fine for 1:6 gearing or 150kv for 1:5 depending on your desired max speed.

6374 motors work with V4.12 but the vescs could get hot during summer. I recommend sensored FOC but don't know if the new Maytech can do it, the old version from last year didn't work in FOC.

99 Pounds for the Comp 95 deck with free shipping in europe:

https://www.powerkiteshop.com/mbs_comp_95_deck.htm

Buy some F5 bindings, too. But they don't have the Matrix II trucks in stock, can get it somewhere else.
```

---
## \#15 Posted by: Euformelo Posted at: 2018-11-28T19:08:01.329Z Reads: 44

```
Hi @rich thank you a lot for your help, just ordered the MBS 95 from that page. Also these 9374 motors 192KV are on Black Friday still so I got the really cheap.
Do you mind if I ask you more question in future if have to?

Kind regards
Euformelo
```

---
## \#16 Posted by: rich Posted at: 2018-11-28T20:12:11.466Z Reads: 42

```
No problem you are welcome!

Do you already have hubs and tires/tubes?

Because if not you could change your order to the complete set with Matrix II trucks, bindings and wheels.
https://www.powerkiteshop.com/mbs_comp_95.htm

Just to mention, it could be that you have to cut the deck a bit to have space for the drivetrains.
```

---
## \#17 Posted by: Euformelo Posted at: 2018-11-28T20:54:54.551Z Reads: 39

```
@rich Yes I already bought tires and hubs [tires](https://www.aliexpress.com/item/Tire-and-Inner-Tube-200X50-Full-Wheels-for-Electric-Scooter-Wheel-Chair-Truck-Pneumatic-Trolley-Cart/32888478355.html?spm=a2g0s.9042311.0.0.37194c4dlZdJnN).
```

---
## \#18 Posted by: Euformelo Posted at: 2018-12-18T20:03:25.388Z Reads: 34

```
Hi @rich
can you tell me your opionion about this. This is what I will buy:
DECK
https://www.atbshop.co.uk/mountainboard-accessories/trampa-35-long-kiteboard-deck
AND I DONT KNOW WHICH ONE SHOULD i BUY
https://www.atbshop.co.uk/mountainboard-accessories/trampa-infinity-truck-silver
OR
https://www.atbshop.co.uk/mountainboard-accessories/trampa-vertigo-cnc-channel-truck-black

Do you find a big issue that axles on these tracks are 12mm cause on my wheels are 10mm?

Kind regards
Euformelo
```

---
## \#19 Posted by: rich Posted at: 2018-12-20T14:25:03.147Z Reads: 30

```
Hey,
first of all which wheels do you have with 10mm bearings? Should be no problem to switch to bearings with 12mm inner diameter.

On this deck you probably have to do some cut outs for the drivetrain. For the gearbox and proper alignment of the gears you need a machined Trampa hanger or simply go with MBS Matrix II trucks
```

---
## \#20 Posted by: Euformelo Posted at: 2018-12-21T19:48:45.717Z Reads: 25

```
Hey Rich, thankl you again for answering.

I have these wheels: [Wheels](https://www.aliexpress.com/item/Tire-and-Inner-Tube-200X50-Full-Wheels-for-Electric-Scooter-Wheel-Chair-Truck-Pneumatic-Trolley-Cart/32888478355.html?spm=a2g0s.9042311.0.0.37194c4dlZdJnN).

So I will order the board from trampa and buy with it MBS Matrix II trucks.
Do I need to cut the board then or it is good with these trucks?

Kind regards
Euformelo
```

---
## \#21 Posted by: rich Posted at: 2018-12-21T20:43:43.654Z Reads: 21

```
If the outside diameter of your bearings is 28mm then you can switch to standard 28x12mm mountainboard bearings.

[quote="Euformelo, post:20, topic:75036"]
Do I need to cut the board then or it is good with these trucks?
[/quote]

This has nothing to do with the trucks, only with the deck. I would spend 25£ more and buy the Holypro deck, much better for electric MTB and no worry about cut outs.

I recommended the Matrix II trucks because they don't need to be cnc machined like Trampa's for gear drive. I would buy additional orange shock blocks as well but that depends on your weight, too.
```

---
## \#22 Posted by: Euformelo Posted at: 2018-12-24T15:08:33.242Z Reads: 14

```
Hi @rich I really appreciate your time that you spend on answering.

Will order Holypro deck + Matrix II.
I checked the wheels and they have a little bit bigger like 29mm.

Kind Regards
Euformelo
```

---
