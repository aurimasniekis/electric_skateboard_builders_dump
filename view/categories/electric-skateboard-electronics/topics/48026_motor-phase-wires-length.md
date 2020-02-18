# Motor phase wires length

### Replies: 17 Views: 1114

## \#1 Posted by: Skateman Posted at: 2018-03-03T14:18:44.755Z Reads: 247

```
 Hey guys. Wanted to find out what is the maximum length the motor phase wires can be between a VESC and the motors. Trying to go 4 ft. if that's possible. Does wire size and/or type matter? Appreciate any thoughts.
```

---
## \#2 Posted by: mmaner Posted at: 2018-03-03T14:21:34.926Z Reads: 250

```
Wtf are you building that you need 4 feet?  😀

I've heard of people having issues, but others say it doesn't matter. I have always tries to stay within 10in or less. I think @GrecoMan uses ling Ines once, maybe he can she's some light.
```

---
## \#3 Posted by: GrecoMan Posted at: 2018-03-03T14:49:41.265Z Reads: 244

```
[quote="mmaner, post:2, topic:48026"]
uses ling Ines once, maybe he can she’s some light.
[/quote]

are you drunk right now? 🤣

but yea, i run phase wires about 30” long. never had an issue
```

---
## \#4 Posted by: mmaner Posted at: 2018-03-03T15:08:06.697Z Reads: 230

```
Just in a hurry 😀
```

---
## \#5 Posted by: Skateman Posted at: 2018-03-03T15:10:03.767Z Reads: 226

```
Thanks @mmaner! I'm still working on my skates. I want to make a waist belt battery pack with vesc at that location too. I've read one shouldn't lengthen the battery leads too long unless you add capacitors along the ways. Even then it said that's not a good idea.

@GrecoMan  Heck no! It's only 9:00 am. I'm gonna at least wait till noon!  lol  Appreciate it. 30" does sound good. maybe I can get by with 36 or so. I'm 5' 11", so kinda looking at 4 ft.
```

---
## \#6 Posted by: Acido Posted at: 2018-03-03T15:15:25.971Z Reads: 221

```
Make sure that the wires are appropriate gauge and all same lenght, there is some tolerance but dont make one 1 meter and 2nd 2 meters and 3rd 20cm because then there could be some problems
```

---
## \#7 Posted by: GrecoMan Posted at: 2018-03-03T15:15:59.411Z Reads: 221

```
LOL

the drunk comment was directed towards @mmaner 🤣
```

---
## \#8 Posted by: Skateman Posted at: 2018-03-03T15:20:22.341Z Reads: 217

```
Oh, sorry. Thought my idea sounded like that.  lol

@Acido  The same length from lower back, (low as possible), to the wheels.
```

---
## \#9 Posted by: benjammin Posted at: 2018-03-03T17:46:59.252Z Reads: 198

```
I've heard long phase wires are ok, but they need to be bundled tightly together. Better to twist them iirc.
```

---
## \#10 Posted by: banjaxxed Posted at: 2018-03-03T20:47:06.409Z Reads: 188

```
No way to put the controllers off you? they get quite warm, also you should be able to compensate the long battery wire with extra capacitors.

I don't know about this
![belt|400x400](upload://whs3soDJXFXnPaCll8vV5eIh0bE.jpg)
```

---
## \#11 Posted by: Namasaki Posted at: 2018-03-03T20:56:11.200Z Reads: 181

```
[quote="Skateman, post:1, topic:48026"]
Does wire size and/or type matter?
[/quote]

Keep in mind that:
Smaller gauge wire = more resistance
Longer wire = more resistance.

If you go long go big as well.
Like 10ga. silicone.
Maybe even 8ga.
```

---
## \#12 Posted by: ThermalM16 Posted at: 2018-03-03T21:13:26.275Z Reads: 174

```
So generally it's not the best idea to run long wires. I was talking to Hummie and a few other people in regards to wire gauges. So the big issue with long wires is you cause a voltage drop at the end of the wire due to resistance within the wire itself. Generally most esk8 applications would run fine with wires as small as 15awg assuming the wires are a total of about 1 foot in length. 

For motor phase wires, running 15 AWG vs 10AWG or something wouldn't make any difference when they're only 6in long or so. You're talking about running something maybe 4 feet long or so I would recommend 10 AWG and insure all the wires are as close to the same in length as possible. Go for pure copper, silicone insulation with a high strand count. This will be the least resistance, highest flexibility, and durability. I would also highly recommend sleeving these cables in some sort of PET sleeve, or heat sleeve like [this](https://www.amazon.com/Hiwow-Sleeve-Fiberglass-Adjustable-Shield/dp/B075M7H891/ref=sr_1_1?ie=UTF8&qid=1520110969&sr=8-1&keywords=heat+shield+sleeve). Lastly, as a rule of thumb, higher voltages can travel in a smaller wire than lower voltages (this is mainly due to the average amp draw being lower). In other words, make your battery 10s or 12s and you won't run into issues. Good luck! 

Here's a [handy dandy calculator](http://www.solar-wind.co.uk/cable-sizing-DC-cables.html) that should work pretty well for your needs.
```

---
## \#13 Posted by: Cobber Posted at: 2018-03-04T00:11:51.673Z Reads: 153

```
i'd be conservative on your brake setting on your vesc.
```

---
## \#14 Posted by: Deckoz Posted at: 2018-03-04T01:05:13.881Z Reads: 148

```
[quote="mmaner, post:2, topic:48026"]
he can she
[/quote]

He can be a she. Indeed.
```

---
## \#15 Posted by: Skateman Posted at: 2018-03-04T01:18:45.699Z Reads: 143

```
Thanks guys, a lot of good info for building extended motor phase wires. I made a measurement and looks like 3 ft. will work and a good starting place.

Thanks @ThermalM16 for the calculator.

@Cobber, I use current control setting so I can have a reverse. I need the motors to go both directions.
```

---
## \#16 Posted by: Scoo_B_SK8 Posted at: 2018-03-04T06:56:54.780Z Reads: 123

```
all i can really say is, wow.  @banjaxxed painted the picture.  this application is above my pay grade, but curious as to what/if any safety features are in a bat/vesc belt, i.e. thermistor, Kevlar, self extinguisher?  

very interesting indeed. please post it when complete
```

---
## \#17 Posted by: Skateman Posted at: 2018-03-04T20:30:44.650Z Reads: 106

```
Well, a protective containment for the batteries is, at the very least, required. Not sure of what other forms of safety devices are available. Need to do some research. I'm reading about the backpack type battery pack for ideas. I surely would appreciate any thoughts and/or experiences you battery builder guys out there have. Maybe this is a project that is not feasible.
```

---
