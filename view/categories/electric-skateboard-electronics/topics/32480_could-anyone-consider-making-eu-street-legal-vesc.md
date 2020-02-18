# Could anyone consider making EU Street Legal VESC?

### Replies: 6 Views: 773

## \#1 Posted by: svenboard Posted at: 2017-09-06T23:34:45.214Z Reads: 132

```
Hey there everyone,

I know this might not be the right place to post, then again it seems the better VESC (OK, ESCs based on Vedders ESC) makers hang out here, so I might catch them all instead of looking up contact info.

Might also be interesting to see what the community thinks.

So: Having looked at the schematics for the VESC, I see it's fairly easy to add an adjustable 4.7-12.v 1A output for head lights and break lights.

This would mean that the VESC would make the skate/longboard EUstreet legal (Something I think we European riders should honestly care about if we want regulations to allow us to be on the roads like in other countries. Right now there is no regulation on electric skateboards, one can only imagine it falls under the same ones as for electric bicycles / kick scooters)

Sure, one could buy RC parts or do it with an Arduino but the question is why?

You'd need: 
1. Batteries (1-2s) **OR** a voltage regulator since you dont want to feed the lights your 3-12s. 

2. And a battery enclosure.

3. RC Switch taking up 1 CH on your tx/rx (for head lights, whereas I'm pretty sure the VESC keeps track of time since it monitors watt usage etc, it could easily switch on the lights based on date and time OR one could program the VESC so that if the breaks are applied when the board is standing still for X seconds, it recognizes that as a light switching input and one could rotate through different modes) **UNLESS** you want to have the headlights turned on all the time / add a mechanical switch.

4. UBEC/SBEC to convert the voltage, unless you manage to find lights that take the specific voltage the battery delivers, limiting your options (For example bicycle lights rarely run on 3.7v iterations)

5. Some controller that detects when breaks are applied.

6. Wires.

7. Space.

8. **_Time_**.


So why not add this? I can't imagine it would be more than 4-5 USD of parts and I am fairly certain it is not much work to modify the firmware (Heck, I could give it a shot)

Another feature could be adding a secondary output for LED lights.

Also: Why doesn't the VESC feature ABS technology?



What do you EU users thinks?
```

---
## \#2 Posted by: florensvb Posted at: 2017-09-07T08:34:59.612Z Reads: 100

```
[This is specifically for german esk8 laws, but there might be tons of interesting information for you!](http://www.electric-skateboard.builders/t/german-esk8-laws/4369)
```

---
## \#3 Posted by: TehAtheist Posted at: 2017-09-07T09:29:48.133Z Reads: 89

```
In Belgium we don't need all this. Just ride slower than 18km/h and your fine. Ride faster and ... Well you're illegal but nobody cares really, as long as you don't drive like a maniac. And with a bluetooth module and the permitr app, I can limit my board to 18 km/h within seconds.

Currently making front & rear lights + ledstrip, with mechanical switch and a step-down convertor attached to my main battery. (10€)
I don't see why you'd want a separate battery pack for the lights. Unless you're going for super night vision and high wattage lights ;)
```

---
## \#4 Posted by: WARMAN Posted at: 2017-09-07T10:04:21.364Z Reads: 76

```
In the uk any electrical vehicle that is not taxed or insured should not go above 8mph so if you see the police I would slow down!
I tend to stick to quite roads and avoid main roads if I can.
```

---
## \#5 Posted by: TehAtheist Posted at: 2017-09-07T10:12:18.496Z Reads: 71

```
I ride in the city and I've driven past tons and tons of cops, with my loud SK3 motor unsensored no FOC. Trust me, if I ride by, you know it's not a regular board :sweat_smile: . Not a single one has ever stopped me.

Once a cop on a bicycle overhauled me and my friend, the woman said: "I wish I could hook myself to you, but I'm not allowed to do that -*Sigh*-" and she took a left then. So the fact that the police officer just made a joke right next to us, makes me pretty sure that it's legal in Belgium.

But then again, it's possible that it greatly differs in other country's.
```

---
## \#6 Posted by: WARMAN Posted at: 2017-09-07T11:09:17.360Z Reads: 54

```
That's the law for the uk..not saying I abide by it I never stop for police I fly past them with a dual 30+  but if you get caught in town and can't make a quick getaway might wana slow down!
```

---
