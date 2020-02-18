# LIPO Balance Charger for 6s Turnigy Batteries

### Replies: 10 Views: 132

## \#1 Posted by: ghols Posted at: 2019-11-26T04:13:53.098Z Reads: 36

```
Hi everyone,

So I tried using the search function to find the answers I've been looking for, but every thread just devolved into people talking about how easy it is to solder a bms or how to diy a power supply.

I'm looking for a bone simple ac/dc charger that can charge 2 6s 5AH or 10AH LIPO's at a reasonable rate. Like within 4 hours. Ideally, under $200, tbh the cheaper the better.

If anyone can help me out, that'd be dope. Thanks!
```

---
## \#2 Posted by: Benjo Posted at: 2019-11-26T07:40:02.602Z Reads: 34

```
Ready made dual chargers are either pretty crappy or very expensive.

Thats maybe not what you want to hear, but my solution is as follows: 2x ISDT Q6 Pro chargers (one of the best out there, a lot of customization and 300w each) and a 600w computer PSU. Cut all yellow (12v) and black (GND) wires, solder them to 2 XT90 connectors, bridge the single green wire to GND to make the PSU always turn on and plug the XT90 into the ISDTs via a an XT60 adapter. This takes ~15min to complete and then you have a fully modular, 600w dual charger for lipos, liions etc. with 14A each. That should charge 2 10Ah packs in less than an hour.

Edit: price is about 2x50+50=150€
```

---
## \#3 Posted by: Slak Posted at: 2019-11-26T13:07:59.447Z Reads: 31

```
@Benjo 
If you mean 300W under 25.2V, how do you get 14A ?

300 / 25.2 = 11.9
```

---
## \#4 Posted by: Benjo Posted at: 2019-11-26T13:21:12.506Z Reads: 29

```
The charger is rated for 14A output max. You won't get 300w with just 12v input, that's true. But you could also get a 24v psu then you have 24*14=336 > 300
```

---
## \#5 Posted by: Slak Posted at: 2019-11-26T13:28:06.453Z Reads: 26

```
[quote="Benjo, post:4, topic:104248, full:true"]But you could also get a 24v psu then you have 24*14=336 > 300[/quote]
I see what you meant but in your "two 300W chargers and a 600 PSU to charge two 6S Lipo" scenario, 14A is not and will never be reachable :) That's all I say, so the OP (@ghols) doesn't think he will get 14A with your solution. But 10A is enough anyway for a 10Ah lipo (means 1C) and usually too much for a 5Ah Lipo (means 2C)
```

---
## \#6 Posted by: ghols Posted at: 2019-11-26T14:39:44.568Z Reads: 25

```
So I’m going to need a charger that can output a minimum of 1c and in this case 10 amps? Plus the a wattage that would get to 10 amps. So 10x25.2 for 252 watts. So if I were to charge at these specs, I could charge a 10ah battery in 1 hour? I’m still learning so be gentle if my math is all jacked up.
```

---
## \#7 Posted by: Slak Posted at: 2019-11-26T16:58:40.255Z Reads: 23

```
Yeah, almost all good !
The charging process is not linear so it will take something around 1,3 hours. This is the factor (1,3) we agreed on/use on the French forum for this calculation on lipos (don't know for li-ion and honestly, I don't care), some may say more or less than 1,3 but it's not 1 hour anyway, a bit more.

My examples : I can charge my 8Ah 9S lipos build with a 2A or a 6A power supplies.
8Ah / 2A = 4h then 4h * 1,3 = 4h18min for the 2A
8Ah / 6A = 1,33h then 1,33 * 1,3 = 1h44min for the 6A
```

---
## \#8 Posted by: mjaffee Posted at: 2019-11-26T19:47:11.069Z Reads: 19

```
I’d recommend the ISDT D2. My batteries are 10mm bullets, so I had to make/buy an adapter to XT60. Its small enough to be portable with a built in AC inverter and has dual channels. I don’t run a BMS on my board because I prefer to charge the batteries off board.
```

---
## \#9 Posted by: ghols Posted at: 2019-11-29T01:33:41.645Z Reads: 13

```
Awesome, I'm looking into it. I'm still debating between the hassle of LIPO vs Li-Ion so I'm still on the fence. I'm thinking if I go with LIPO's this would be a good choice. How long have you had it? Any quirks to look out for?
```

---
## \#10 Posted by: mjaffee Posted at: 2019-12-01T07:01:54.124Z Reads: 7

```
Nope, its been working great. I use them with lipos vs li-ions. Simple swap in swap out. 18650 cells can work too, you just may have to run an extension to the main battery wires and balance cables (or some hot swap system). 

For me, The D2 eliminates the need for a balance charger when charging but doesn’t manage the battery use since there’s no bms. Long story short, a lot of uneven cell voltages.
```

---
