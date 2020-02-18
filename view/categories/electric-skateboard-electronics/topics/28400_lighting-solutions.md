# Lighting solutions?

### Replies: 9 Views: 1664

## \#1 Posted by: karosass1 Posted at: 2017-07-23T20:50:51.615Z Reads: 203

```
Obvious solution would be shred lights, but I want something more customizable as in rgb lights with some Bluetooth module that I could connect to by writing my own app or maybe there is some solution for it?

Note : I need it not just for the looks but for usefulness at dark as well. 

The questions:

How would I go around mounting either led strip or separate leds? I saw a person make 3d riser for that, but I'm not really sure about that supporting 90kg me. What about simply gluing led strip on riser? Waterproof one. 

What about powering it? VESC have 5V1A output for external stuff, which is not enough, so I guess additional power source?
```

---
## \#2 Posted by: malik98 Posted at: 2017-07-24T00:11:15.662Z Reads: 189

```
I ran a buck/boost converter off of my 8s lipo that dropped it to 12v. 
https://www.banggood.com/LM2596-DC-DC-Voltage-Regulator-Adjustable-Step-Down-Power-Supply-Module-With-Display-p-1005123.html?rmmds=myorder
```

---
## \#3 Posted by: rpn314 Posted at: 2017-07-24T19:03:20.617Z Reads: 161

```
Are you looking for underglow, turn signals, brake lights, or headlights?

And yes, you'll need an external source for anything substantial.
```

---
## \#4 Posted by: darkkevind Posted at: 2017-07-24T19:08:10.754Z Reads: 156

```
You don't need a buck/boost converter, just run an inline voltage regulator to take your voltage down from whatever your battery voltage is to 12v nA (where n is the number of amps you need to power your lights).

It's what I use for my 120A relay switch to turn my board on and off, although I step down from 33.6v to 24v.

https://www.digikey.co.uk/products/en/integrated-circuits-ics/pmic-voltage-regulators-linear/699?k=voltage%20regulator
```

---
## \#5 Posted by: karosass1 Posted at: 2017-07-24T19:31:45.972Z Reads: 143

```
Sorry, I wasn't specific enough. I want kind of combination of headlights, brake lights and underglow. But probably just a led strip won't be bright enough for headlights? I guess for starters I will settle on just headlights/brake lights.
```

---
## \#6 Posted by: darkkevind Posted at: 2017-07-24T19:33:17.000Z Reads: 135

```
Look here: http://www.electric-skateboard.builders/t/eskate-lights-thread/199
```

---
## \#7 Posted by: trancejunkiexxl Posted at: 2017-07-24T19:44:24.059Z Reads: 135

```
so can you use a secondary bec? or use one from powering rx
```

---
## \#8 Posted by: darkkevind Posted at: 2017-07-24T19:50:52.686Z Reads: 128

```
5-6v isn't going to be enough which is what most BECs put out.
```

---
## \#9 Posted by: trancejunkiexxl Posted at: 2017-07-24T19:52:12.627Z Reads: 123

```
[quote="darkkevind, post:4, topic:28400"]
inline voltage regulator
[/quote]

inline voltage regulator it is then XD
thanks for the valuable info
```

---
