# First Board: Need Help and Advice! Loaded Tesseract, Smooth Ride, Long Range

### Replies: 5 Views: 1058

## \#1 Posted by: wagadugu Posted at: 2016-07-06T21:11:07.048Z Reads: 140

```
Hi Guys!

This is my first E-Board i'm creating, i'm going to admit I am splurging a fair amount and am looking to have this board last me for years, there's parts i'm aiming to finalize and some I haven't found quite what i'm looking for so feel free to chime in and give advice!

[Documentation / Parts](https://docs.google.com/spreadsheets/d/1joKuP4vqS1t_ur04H5aLkm3V-3Cca8ERk3elRjhwASE/edit?usp=sharing)

The goal of the board is to have one that can travel great distances, last long and be as shock absorbant and steady as possible for Toronto's hilly / bumpy sidewalks / roads.

I weigh around 100 pounds

**The Goal**
I'm aiming for a board that can go around a solid 20km on a single charge with a decent amount leftover (used for both work and for round trip casual commuting)

**Things i'm currently searching for the best solution for:**
**Batteries:**
I plan on linking up around 400-500$ worth of 18650 Panasonic batteries with PVC Anode Protection. Since I plan on using this for commute purposes and potentially charging this at the workplace, I am determined to spend the extra money for the extreme long distance increase along with my ability to safely ensure the board will not cause any form of damage in the workplace (ex. spontaneous combustion). As rare as it is for a Lipo to spontaneously combust, I refuse to take that risk for any employer I work for.

Does anyone have any idea how to best link up these batteries, i'm not entirely sure the best method to link up so many batteries together from a physical architecture standpoint and so far my research has come fruitless besides understanding to shrink wrap it. So far i'm looking into linking them into a series of 6 and parallel of 7 to get 22.2V and 21,700 mAh of capacity for runtime.

**Casing**
Was thinking of using foam with slits sealed in fiberglass and a carbon fiber sheet for durability, flex and space

**Remote / Control solution**
I have no clue, looking for something like a boosted board remote, small and easy to use for 1 hand that I can operate like car, forward to accelerate (with a cap) and back to progressively break, multiple buttons for various set speeds would be really nifty. From my understanding it looks like a mix between a VESC thing and having a good remote with buttons.

I'm probably missing things as all of this is new to me and I am learning on the fly so feel free to ship me any advice if you think I missed something!
```

---
## \#2 Posted by: Namasaki Posted at: 2016-07-07T06:10:18.490Z Reads: 122

```
[quote="wagadugu, post:1, topic:5678"]
Things i'm currently searching for the best solution for:Batteries:
[/quote]
@barajabali Makes custom battery packs
```

---
## \#3 Posted by: treenutter Posted at: 2016-07-07T16:32:30.046Z Reads: 99

```
[quote="wagadugu, post:1, topic:5678"]
I plan on linking up around 400-500$ worth of 18650 Panasonic batteries
[/quote]


@wagadugu That estimate seems high for 6s7p. At $5 a cell that'd be $210USD.

Also; that is a lot of cells; soldering them together will be a huge task. Are you planning to buy a spot welder? If not I'd consider having your pack custom made by @barajabali or another pack builder.
```

---
## \#4 Posted by: wagadugu Posted at: 2016-07-07T17:59:38.979Z Reads: 93

```
@namasaki @treenutter Thanks for the great advice! i'll be contacting barajabali soon and seeing how that goes :)

@treenutter  In terms of the price, I was intending on buying [Deal Extreme 18650 3100 mAh Panasonic with PVC](http://www.dx.com/p/panasonic-3100mah-18650-li-ion-battery-transparent-pvc-anode-protection-with-case-green-4-pcs-292082#.V37HI7grKUk) in bulk to get them at 37.69 cad per 4 (i'm Canadian) This way I can make sure I can maintain the quality and ensure their longevity. The extra PVC protection and CAD currency bump it up to the 400$ range CAD for me :( (Edit: put wrong link, mybad!)

I was also thinking of this alternative battery I found on deal extreme, much cheaper and looks reliable but I'm unsure about the quality of the product [Deal Extreme 18650 3400 mAh Soshine battery with PVC](http://www.dx.com/p/soshine-li-ion-18650-3400mah-anode-protection-batteries-with-case-black-4-pcs-365820#.V36b6rgrKUk) Bulk order at 19.08 CAD. What do you guys think?

**Question!**  also @barajabali 
I was also considering an alternative method to making pack building much easier where I would be able to buy a bunch of [Deal Extreme 4 slot 18650 battery case](http://www.dx.com/p/diy-4-slot-18650-battery-holder-with-pins-black-287251#.V36XKLgrKUk) to hold the batteries and using the appropriate wiring and soldering to link them all into 6s7p (or something else but, that's the goal) and then once everything is attached and soldered together, shrink wrap it.

Still definitely exploring if I could get the great assistance of a veteran like @barajabali for help though :slight_smile: 

My main concern with this is size (haven't fully gotten the time to draw blueprints yet for visualization) since it would definitly take more space having the casing and the wires on the back of it. 

My other main concern is the conductivity, I remembering hearing online that when it comes to these things, you really want to use pure nickel plates instead of a part-steel part-nickel plate because the conductivity difference is significant. This is definitely the biggest deciding factor for me since I 100% intend to over-engineer this battery for some pretty extreme distance.

What do you guys think?
```

---
## \#5 Posted by: sl33py Posted at: 2016-07-07T19:16:11.003Z Reads: 76

```
I defer to those more experienced than me - especially when it comes to 18650 packs which i don't know much about...

However - I would definitely talk with some folks here about your battery choice.  I looked at the 3100mAh Panasonics and did not see the discharge amps rating.  I think this is critical in our use case.  Most are 10A, some are 20/25/30 (usually higher Amp has lower capacity and a lot more $).  I have those soshine protected 18650's for my TM30 flashlight - great cells, but again i don't think you want button cell, nor protected!

The ones i see folks here using are the LG HD2's and similar.  Hopefully @barajabali can comment and give you his preferred cells.

Your range requirement really isn't "extreme".  I get 10-12 miles easily on my Marbel, and on my GF's single motor Vanguard w/ 8s 8Ah setup it's pretty close (and swappable if i need more range).  She rides slower so i lap her quite a bit on a ride...

I'd start by looking up the info on the Watt Hour to KM estimates.

I would not try to use the 18650 case - for 2 main reasons - size/weight, and amp handling/capacity.  Plus it advertises as "shrapnel" - no thanks!  I'll avoid that on any board i ride...  hehehe
[img]https://lh3.googleusercontent.com/-Ehr-TShH6ws/V36ptEsqbeI/AAAAAAAAslY/Z1pDCxRe0SseaOMszmVTd8lJ5HwwaqdDACCo/s599/Stainless%2BSteel%2BShrapnel.JPG[/img]

Joking aside - you need a certain gauge of wire or nickel strips to handle the amperage of these cells to power your board - you don't want to melt these or have issues.  Instead spend that $ on someone building the pack correctly witht he right gauge wire/strip to handle the amps you need. 

it adds complexity and weight you don't want.  I'd want the smallest/lightest and thinnest battery pack possible.  The whole, or at least a primary, point of the 18650 cells is the 18.x mm thickness dimension making them super sleek/stealthy!!

I'll be following to see what the experts suggest - hope this helped as well.
```

---
