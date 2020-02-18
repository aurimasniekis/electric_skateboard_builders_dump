# Building a perfect travel-safe battery

### Replies: 42 Views: 4109

## \#1 Posted by: Eboosted Posted at: 2016-12-27T05:31:34.245Z Reads: 268

```
One of the most exciting parts of electric skateboarding is traveling with your board, so for this scenario I'm looking to build travel-size batteries.

According to most airlines you need to follow these rules:

http://www.delta.com/content/www/en_US/traveling-with-us/baggage/before-your-trip/restricted-items.html

1. Battery must be removed from e-board
2. e-Board can fly on carry-on or checked baggage but without the battery
3. Battery must travel on carry-on luggage
4. Battery leads must be covered in tape
5. Should not exceed 160 watt/hour

According to FAA you need to follow these rules:
* FAA works closely with FAA, so they follow the same rules

https://www.faa.gov/about/initiatives/hazmat_safety/more_info/?hazmat=7

1. You can carry up to 2 spare batteries between 101-160 watt/hour
2. Battery terminals (usually the ends) must be protected from short circuit
3. Batteries must be carried on carry-on baggage

For a 160 watt/hr battery on 10S (37V) this is the closest option I coul find

One 10S1P pack made of HO HOHM Grown 26650 4307mAh Flat Top Battery
37V * 4307mAh / 1000 = 159.359 watt/hr
[img]http://i.imgur.com/Vh661aF.jpg[/img]

- Just below the maximum regulation of 160 watt/hr
- I'm concerned about battery sag
- The max continuous discharge for this battery is 23A (11.5A for each VESC on a dual setup)

What would you guys suggest?
```

---
## \#2 Posted by: Eboostin Posted at: 2016-12-27T05:58:23.258Z Reads: 254

```
Supposedly, you can bring as many 99Wh batteries as you like
```

---
## \#3 Posted by: ZachNYC Posted at: 2016-12-27T05:59:00.313Z Reads: 248

```
I am doing 3 4s3p batteries connected with xt60 series connectors that I will detach for planes.
```

---
## \#4 Posted by: ZachNYC Posted at: 2016-12-27T06:09:11.781Z Reads: 238

```
From what I have read, this is true.
```

---
## \#5 Posted by: Eboosted Posted at: 2016-12-27T06:34:36.443Z Reads: 236

```
According to the this FAA statement and if the battery capacity is between 101-160 watt/hr you can only carry two

"There is a limit of two spare batteries per person for the larger lithium ion batteries described above (101-160 watt hours per battery)."
```

---
## \#6 Posted by: Eboosted Posted at: 2016-12-27T06:41:25.847Z Reads: 223

```
Hey @ZAchNYC what battery brand are you going to use? If you are using Samsung 25R they have 2500mAh, so each 4s3p should have 111 W/Hr , you have room for more capacity to reach the 160w/Hr limit

What motor KV does you board has?
```

---
## \#7 Posted by: ZachNYC Posted at: 2016-12-27T06:47:08.596Z Reads: 217

```
I am very rarely traveling alone so I can have the people I'm traveling with take one of the packs and I should be fine. I am using Samsung 25r batteries, and my motor kv is 192. If and when I am traveling alone, I can just bring two of the packs and leave the other and the other series connector and I will be fine as well.
```

---
## \#8 Posted by: captainjez Posted at: 2016-12-27T06:56:01.349Z Reads: 212

```
I recently carried our Jed Board from Singapore to Sydney and back. I removed both battery packs which are well over 200wh each. I carried the batteries in my carry on inside Kevlar bags. Nobody flinched at either Sydney or Singapore airports.
```

---
## \#9 Posted by: Eboosted Posted at: 2016-12-27T07:00:32.836Z Reads: 210

```
According to @chaka on [this post](http://www.electric-skateboard.builders/t/choosing-the-right-motor-kv-for-the-vesc/3125), for that motor and a smooth running, you should be using a 42V 10S battery.

8570 RPM/50v = 170kv - 12s
---------------/42v = 200kv - 10s
---------------/33v = 260kv - 8s
---------------/25v = 340kv - 6s

I wonder how would this motor run on a 8s3p setup?
```

---
## \#10 Posted by: ZachNYC Posted at: 2016-12-27T07:11:43.620Z Reads: 199

```
@chaka stated that it was a "rough guide", and on the same post, @chaka also said that at 12s it could be pushed up to 200kv "but the top end would feel weak", which I am not worried about as I don't plan to be doing anything above 25mph.
```

---
## \#11 Posted by: ZachNYC Posted at: 2016-12-27T07:13:18.867Z Reads: 197

```
I don't know how the motor would fare with that battery, but I am still pretty new to all of this, so I wouldn't be the one to ask. I would just search through the forum for builds with that setup and see how it worked for others.
```

---
## \#12 Posted by: lox897 Posted at: 2016-12-27T07:40:01.799Z Reads: 191

```
A123 26650 is probably the perfect battery for travelling. You could build a 12S1P that would be exactly 99wh.
```

---
## \#13 Posted by: Michaelinvegas Posted at: 2016-12-27T17:53:08.154Z Reads: 177

```
Someone needs to make a pack like this

https://youtu.be/8b9ZYt6MzHc

It has dual voltage....think gets around the airplane issue by a switch that mechanically separates the battery inside the pack.
```

---
## \#14 Posted by: i2oadsweepei2 Posted at: 2016-12-27T18:25:14.222Z Reads: 169

```
The barking Spider!! :joy: :joy: :mask:
```

---
## \#15 Posted by: Eboosted Posted at: 2017-01-01T19:32:28.807Z Reads: 159

```
I made a design yesterday and I think I came up with the perfect idea. 

I'll build four 10s1p individual batteries connected in parallel, each battery should have 92.5 watt/hr (travel safe) 

As the board I'm building is a Loaded Vanguard, I might be having issues with flex as the battery would be longer than expected, so I will do 4 different enclosures, one for each 10s1p pack, that'll be mounted next to each but individually bolted to the board to allow flexiness, but connected by 12AWG silicone flex cable and Xt60 plugs. 

Do you guys think this would work?
```

---
## \#16 Posted by: SageTX Posted at: 2017-01-02T01:49:32.545Z Reads: 155

```
So you end up with a 10s4p board. Sounds like a Winner!!  

Bonus you can have as many batteries as you want since under the 99w/hr limit.
```

---
## \#17 Posted by: PXSS Posted at: 2017-01-02T02:50:02.968Z Reads: 151

```
Check out the last ~10 posts on this thread on a travel safe 12s3p battery. 
http://www.electric-skateboard.builders/t/first-build-loaded-vanguard-deck-1-turnigy-sk3-6374-192kv-12s3p-samsung-25r-vesc-x/14242/69

Would be a single enclosure.
```

---
## \#18 Posted by: ZachNYC Posted at: 2017-01-02T03:48:53.714Z Reads: 145

```
I've been meaning to ask, for the loop keys between the batteries, should I connect them with xt90s's? Also, wouldn't the wires on the batteries need to stay connected to the same connector? If so, couldn't/wouldn't the TSA see it as one battery as I'm sure it isn't their field of expertise?
```

---
## \#19 Posted by: PXSS Posted at: 2017-01-02T05:22:45.246Z Reads: 146

```
You could do each battery with its own XT90 and then make a loop key from 2 XT90s but that's expensive...
```

---
## \#20 Posted by: ZachNYC Posted at: 2017-01-02T05:28:13.040Z Reads: 141

```
Is it possible to make it with xt60's? I already have a bunch
```

---
## \#21 Posted by: PXSS Posted at: 2017-01-02T05:29:08.675Z Reads: 129

```
Depends on the current draw.
```

---
## \#22 Posted by: lox897 Posted at: 2017-01-02T05:30:31.531Z Reads: 137

```
Use antispark xt90s otherwise you will get a big spark

Edit: do you mean as a switch or just connecting the batteries?
```

---
## \#23 Posted by: ZachNYC Posted at: 2017-01-02T05:39:04.260Z Reads: 140

```
I meant for connecting the batteries
```

---
## \#24 Posted by: PXSS Posted at: 2017-01-02T05:41:34.007Z Reads: 140

```
XT60s are rated to 60A, XT90s are rated for 90...
Size appropriately
```

---
## \#25 Posted by: DilatedPupils Posted at: 2017-01-02T05:47:30.203Z Reads: 138

```
You should be fine with xt60 if you're just connecting the batteries together.
```

---
## \#26 Posted by: Eboosted Posted at: 2017-01-02T05:57:10.528Z Reads: 138

```
Let say, you arrived to you destination and want to connect each 10s1p batteries to the board, just pluging the XT60s together, are you saying you would have a big spark here?, I'm guessing you won't have a spark since all batteries are charged with almost the same voltage, or I'm missing something?
```

---
## \#27 Posted by: Blasto Posted at: 2017-01-02T06:02:14.870Z Reads: 133

```
holy fuck this guy is hilarious
```

---
## \#28 Posted by: PXSS Posted at: 2017-01-02T06:07:26.214Z Reads: 134

```
You still need a master loop key between the batt and esc to close the circuit. This is where the XT90 anti spark needs to be or any other anti spark switch.

@ZachNYC, your battery max output current is 60A so you should be fine with XT60s
```

---
## \#29 Posted by: Eboosted Posted at: 2017-01-02T06:14:32.572Z Reads: 134

```
Yeah the master loop key (battery switch) should be between battery and ESC, it would remain turned off while each individual 10S1P battery pack is being connected via the XT60s.

The only doubt I have is only the first battery pack would have it's balancer wires connected to the BMS, would that be ok?

[img]http://i.imgur.com/IoJjucW.jpg[/img]
```

---
## \#30 Posted by: ZachNYC Posted at: 2017-01-02T06:17:16.552Z Reads: 130

```
Sounds good, xt60s it is then.
```

---
## \#31 Posted by: jga Posted at: 2017-01-24T14:56:56.244Z Reads: 130

```
For information here are the exact IATA rules for batteries. Most of the airlines should follow them.
http://www.iata.org/whatwedo/cargo/dgr/Documents/LithiumBattery_PassengerFlyer.jpg
```

---
## \#32 Posted by: Eboosted Posted at: 2017-01-25T03:46:38.830Z Reads: 129

```
So, I just finished my 10S4P "travel safe" flexible battery pack.

1. Each pack has 8 Samsung 25R, 3.7v * 8 * 2.5Ahr = 74Wh (less than the 100Wh limit)
2. No limit of spare batteries
3. You don't have to declare it or be at the mercy of the TSA or airline representative

[img]http://i.imgur.com/SZfDJJc.jpg[/img]
http://imgur.com/mQwDrj8

I'll build an individual fiberglass case for each pack, so they could be easily plugged in at arrival to destination

https://youtu.be/bbdLbZDogqg
```

---
## \#33 Posted by: CamBo Posted at: 2017-01-25T05:42:20.854Z Reads: 124

```
Pretty sweet!  Do you have a wiring diagram for this?
```

---
## \#34 Posted by: Eboosted Posted at: 2017-01-25T05:43:59.745Z Reads: 125

```
Well you just need to replicate 5 of these packs:

[img]http://i.imgur.com/G6oOQzR.jpg[/img]

I'll try to make a wiring diagram
```

---
## \#35 Posted by: CamBo Posted at: 2017-01-25T05:48:32.886Z Reads: 123

```
Thanks! Can you post pics of the sides where we can see the ends of the batteries?
```

---
## \#36 Posted by: Eboosted Posted at: 2017-01-25T05:56:18.441Z Reads: 125

```
Sorry for the crappy wiring diagram, but you should get the idea:

[img]http://i.imgur.com/gJGEt0D.jpg[/img]
```

---
## \#37 Posted by: mortorojo Posted at: 2017-01-25T06:23:59.120Z Reads: 121

```
Im guessing you decided to not balance these packs?
```

---
## \#38 Posted by: Eboosted Posted at: 2017-01-25T06:33:38.114Z Reads: 121

```
I will balance them, the BMS will be positioned with the first pack (hence this pack will be bigger than the rest), each 8-pack will have 2 jst connectors at the side of the XT60s to be plugged in to the BMS upon arrival at final destination.

BTW, this is prototype.

But the "flying-with-an-eboard" dream is comming together, hope to get feedback from you guys!
```

---
## \#39 Posted by: jga Posted at: 2017-01-25T09:09:49.934Z Reads: 116

```
If i understand well, each group of four cells in parallel does not have any link with the other group of four in the same pack, but is connected in series with a group in the next pack?

How do you manage to have the jst connectors plugged into the BMS?
```

---
## \#40 Posted by: Eboosted Posted at: 2017-01-25T16:14:32.430Z Reads: 114

```
That's correct, the 4 cells in parallel at the left and the 4 at the right are not coonected directly.
'
For the balancer I'm using these jst connectors, so it should be pretty easy to unplug/plug them before/after traveling, each pack will have their own balancer cable soldered.

[img]https://images-na.ssl-images-amazon.com/images/I/71PNzVYYwwL._SL1200_.jpg[/img]
```

---
## \#41 Posted by: jga Posted at: 2017-01-26T07:44:00.099Z Reads: 105

```
Ok, that's cool. I did not know you had these individual small plugs to connect to the BMS.
I got confused because you have two black/red cables coming from both the positive and the negative of each pack.
```

---
## \#42 Posted by: Eboosted Posted at: 2017-01-26T14:26:42.085Z Reads: 101

```
You can check the details of the build here:

http://www.electric-skateboard.builders/t/never-summer-reaper-dual-tb-6355-10s4p-modular-travel-safe-battery-abec-11-97mm/16683/10
```

---
