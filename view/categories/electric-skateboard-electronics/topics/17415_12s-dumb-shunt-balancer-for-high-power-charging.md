# 12s dumb shunt balancer ((for high power charging))

### Replies: 14 Views: 1321

## \#1 Posted by: Hummie Posted at: 2017-02-09T00:00:24.287Z Reads: 121

```
With 12s balance chargers being so rare if not impossible to find, (I mean charging at 50.4 volts) I bulk charge at a wonderful 400 watts with one plug and balance on the side with two of these little things for ten bucks:
https://www.amazon.com/neewer%C3%82%C2%AE-li-polymer-battery-discharge-balancer/dp/b00epblwj8

but these types of things are super slow.  too slow. 


there's this one which is great but does 2 amps which to me is too much as the cost goes up and it's 100$ in the end.  


https://endless-sphere.com/forums/viewtopic.php?f=31&t=85837&p=1262594#p1262594
Anyone have advice on how to make a 12s version of this which could do maybe half an amp?  I'm trying to find a balance of size, amperage, and cost, and mid-point between these things would be ideal.  How does one go about getting something like this built into a little board i could add the components?  If someone could design it maybe we could get enough interest to get the boards made.  


umm I'll get this charger next time 
http://www.parts-express.com/mean-well-mw-se-600-48-48-vdc-125a-600w-regulated-power-supply--320-317
```

---
## \#2 Posted by: smurf Posted at: 2017-02-12T15:12:54.151Z Reads: 88

```
[quote="Hummie, post:1, topic:17415"]
12s
[/quote]

Found this wile looking for that.

http://www.chargery.com/cellSaver12S.asp

How about the thunder 1220 looks good to go to me. But I don't know if it's a hunk of junk or good.

http://www.exceedrc.com/75p-1220-charger.html
```

---
## \#3 Posted by: Hummie Posted at: 2017-02-12T17:57:16.579Z Reads: 80

```
i like to charge at 50.4 so I don't have to take my battery apart.  

those things that monitor the cells "cellsaver" are nice but don't balance unfortunately.   Still looking for a good dumb shunt.
```

---
## \#4 Posted by: Okami Posted at: 2017-02-12T18:27:36.450Z Reads: 70

```
http://www.banggood.com/AOK-3-in-1-150W-Discharger-Voltage-Tester-Balancer-For-Lipo-Battery-p-1051214.html?rmmds=category

Found this.. perhaps if you dis-assemble it .. it can be somewhat good..

of course, this is for 6s.. so im not sure does 2x of these units justify the cost.. though, it looks to be quite powerful :)

--

Here's a little note, for the 50W version of this version (they're also available in black both 50/150w versions):

> Unfortunatly, you cant leave the unit unattended if "discharge" is selected. After discharging to the voltage set, the light bulb goes out, but the unit still uses power. So after discharging a few smaller lipos, the where all "dead" after an hour (voltage far below 3V). So if the unit is ready discharging, disconnect it immediatly from your lipos. You cant leave the proces unattended. Photo: discharge setting at 3,8V. Voltage show after 15minutes (drop of 0,1V)
```

---
## \#5 Posted by: Hummie Posted at: 2017-02-12T18:50:54.392Z Reads: 56

```
i have 4 of those!  they're way too slow and will shut down after a while too.  if one could be made that will do higher power and 12s it'd be a solution.  I have a link above to someone on es who sells the 12s board for making one but it does 2 amps and costs 100$  too much and too much.  I only need maybe one amp discharge.  
with all the people out there needing to charge and balance 12s or 10s a good one of these would be great.  paired with a high wattage bulk charger it's the fastest simplest charging solution
```

---
## \#6 Posted by: Okami Posted at: 2017-02-12T19:14:28.899Z Reads: 50

```
The problem with these it seems they are more made for balacing for ''storage''.. this means, 'low-mid' point balancing, not top (4.1-4.2v)..

Perhaps, it can be set to 4.1v but I think I saw 3.9-4.0 typical..

Is 150w really too slow?

at ~50V that should come out at something like 3A per battery.. Maybe you got the 50W version (1bulb)?

Though, it still should be close 1 amp then, I think..

==

I also found 20w ''resistor type'' discharger.. but these gonna be even more slower..

Yes, I saw your post on ES.. Some middle ground for this would be really welcome..
```

---
## \#7 Posted by: Hummie Posted at: 2017-02-12T19:32:57.438Z Reads: 47

```
it will balance at whatever voltage, it just discharges the higher cells in the pack bringing them down to whatever the lowest is.  I have the bulb version too but it starts to defeat the purpose as it has awkward plugs that I'd have to add adaptors for.  
i don't know what wattage it truly discharges at but it's hella slow.

the guy on es, that board, it's ideal except too big and expensive.  a nice small 12s plug at 1 amp each cell would be ideal and someone who knows more than me could do it simply.  hoping someone can design the board and tell what parts to stick on.
```

---
## \#8 Posted by: smurf Posted at: 2017-02-12T19:35:02.783Z Reads: 44

```
Nothing about battery management seams simple to me.
These guys have a chip

http://liionbms.com/pdf/el01.pdf

http://www.seattleeva.org/wiki/Zener-lamp_regulator
```

---
## \#9 Posted by: Okami Posted at: 2017-02-12T19:44:21.566Z Reads: 45

```
@IDVert3X do you have any ideas about this?

You seem to be pretty educated on the electronics subject ;)
```

---
## \#10 Posted by: IDVert3X Posted at: 2017-02-12T20:43:45.984Z Reads: 41

```
Hi guys, if I understand you correctly, you need 12S balancing circuit that can do higher amps.

You can actually scale these things quite easily. If you need higher discharge power, you will need bigger resistors, mosfets capable of higher currents and adequate cooling. The energy wont magically disappear, it gets transfered into heat so just keep in mind that discharging at 0.5A can result in up to 25W of heat, which is quite a lot. You will need a hatsink and fan. The easiest way would be to thermally glue the resistors to a piece of metal with fins ( heatsink ) and placing a fan on the top of it. It don't have to be necessary loud, noctua fans for example are really quite.

I don't know what help do you expect from me, but feel free to ask.
```

---
## \#11 Posted by: Okami Posted at: 2017-02-12T20:56:26.256Z Reads: 38

```
This seems reasonable :) I think I already heard the idea abot using fans somewhere.. I think the smart chargers also use the fans to cool down the resistors when doing a discharge operation.
```

---
## \#12 Posted by: Hummie Posted at: 2017-02-12T22:06:36.591Z Reads: 38

```
https://hobbyking.com/en_us/turnigy-dlux-lipo-battery-cell-display-and-balancer-2s-6s.html
if this did 12s and could do it faster and in this size that'd be impossible I guess?



 Is there a way to wire it so all the power from the discharging cells could be combined to one circuit?  or is that necessarily a short due to the series connection.
@IDVert3X instead of resistors could I put something else in circuit that would be useful?  

a speaker or big light or ..what would work? an automaton
```

---
## \#13 Posted by: Okami Posted at: 2017-02-13T10:52:32.923Z Reads: 36

```
@Hummie But do you have the same exact model I showed in the banggood link?

with 3x 50W bulbs, it should have had a lot of discharging power.. The only problem would be the light / heat coming out of the bulbs..

To avoid the resistors heating or using larger size ones (which isnt also very practical) you would need to find your load elsewhere.. Speakers I think wont be powerful enough for compact size.. I dunno perhaps you could get something like 50W crammed into a space B6 charger.. then you would probably need some sort of amplifier and all of that stuff..

Bulbs and high powered motors seems to me like the best loads there are.. if someone knows something better, he can put it in here in the topic..

Also you would need to discharge cell groups individually, which might mean that to get higher voltage than 3.5-4.2v, you would need step-up booster, which can be ''activated'' for each cell group needing a drain or such..

--

I havent focused on this topic much individually but for me it looks like it is either - resistor with a fan cooling or using bulbs.. motors are finnicky in that matter you wont get high load/amps when running them at no load and you would probably need brushed ones for not needing sophisticated chips..
```

---
## \#14 Posted by: IDVert3X Posted at: 2017-02-13T14:57:33.150Z Reads: 29

```
There is a reason why resistive load is used to discharge these cells as it's the simplest, cheapest way you can do it. And it works great! For low power applications, there is usually a resistor and LED in series with the resistor. But after all, the light gets converted into heat as well, it's just better spreaded out. 

Stick with resistors, it's the best way to discharge individual cells, 5ohm 5W resistor for each cell should do the job. I would personally use 10W resistor due to bigger area to dissipate heat more quickly and this increasing the lifespan of whole device.

Speaker is stupid idea. Like, totally, stupid.
```

---
