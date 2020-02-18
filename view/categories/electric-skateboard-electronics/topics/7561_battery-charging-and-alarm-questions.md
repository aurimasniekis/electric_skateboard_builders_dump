# Battery Charging and Alarm Questions

### Replies: 11 Views: 1509

## \#1 Posted by: ecuadorche Posted at: 2016-08-12T18:19:27.704Z Reads: 100

```
i have a battery here are the specs

Its a 5S 15c 4000mAh battery  on it says 18.5V i put these in series for 10s i have two identical ones

Ideally what is the most each one should be charged to max and at what speed or amp or c's and whats the least i should drain these to

i also have those little alarms for lipos what should i set them to so i can know when im close to half way so i can turn around and drain the battery i also have two of these one for each battery

Help and recommendations are welcome
```

---
## \#2 Posted by: JLabs Posted at: 2016-08-12T18:33:39.567Z Reads: 97

```
Safe lipo Max charge is 4.2v per cell, and minimum if 3.0v per cell (I recommend around 3.2). Not sure what other questions your asking, but if you clarify a little I would be more than happy to help.
```

---
## \#3 Posted by: ecuadorche Posted at: 2016-08-12T18:36:28.004Z Reads: 92

```
how fast should i charge them? and what should be my total voltage for whole battery

if i want to find a mid point for range what should i set my alarm to??? like if i want to know im half way on power can i set my alarm for a particular voltage???


thanks again for the help
```

---
## \#4 Posted by: JLabs Posted at: 2016-08-12T18:40:16.207Z Reads: 87

```
If you look at the battery specs it should tell you a safe maximum charge, 2 to 5 amps recommended (unless yours cannot be charged higher than 4)

I wouldn't set your alarm half way because then it would beep the whole way home and it wouldn't tell u when the battery gets TOO low. I would set it at 3.3v/pc so it gives you a little more ride time. You can always stop riding and look and the monitor and if your around 3.7v/pc your half way.
```

---
## \#5 Posted by: sl33py Posted at: 2016-08-12T18:54:21.098Z Reads: 87

```
@ecuadorche - Depending on your charger and how high amperage it can charge at (i have the 306b which can do 30, but rarely does) - I try to slow charge at .25-.5C  so 1/4 or 1/2 the Ah.  So your pack is 4Ah or 4000mAh - so 1 C would be 4 amps charging.  I would slow charge at 1 or 2 amps - which increases pack life and is easier on the battery (less heat etc.).

Nice thing about having higher amp charging is when you get home and want to ride before it gets dark!  Being able to charge your pack (each pack will state it's max C charge rate) at higher C is perfect for a quick charge and then go ride.  Did this last night - sunset ride w/ GF at Alki.  quick 30min charge and out the door (not even 2C, but fast enough).

Looking at the Turnigy 4000mAh 5s pack - it has a max charge rate of 2C - so i could charge it at 8 amps, but normally would still do 1 or 2 amps for 1/4 or 1/2 C.

Speaking of C - 15C on this pack will only equal a claimed 60Amps continuous discharge capability.  I personally doubt the marketing department of all battery manufacturors...  So i shoot for a *minimum* of 100Amp discharge capability.  Expecting roughly half that in real world use.  Using an inexpensive (not lab grade, but hey...) inline watt meter on my boards i've rarely seen more than 45A peak draw - so i feel like this is a reasonable short draw use and shouldn't over-tax my packs.

Get a small battery voltage alarm - a few bucks on HK or Amazon:
[img]https://images-na.ssl-images-amazon.com/images/I/41C4qo8ZncL.jpg[/img]
www.amazon.com/Venom-Voltage-Monitor-LiPO-Batteries/dp/B0064SHG0Y
any like this - you set the voltage to alarm at a cutoff point (i usually use a conservative 3.7v or 3.6v).  It also will cycle through the pack showing your cell's individual voltages.  Plus total voltage.

Your 5s pack should be 21v fully charged (5 * 4.2v).  Nominal voltage (for calculating Wh) and what they show on the pack will be 3.7v *5 = 18.5v.

HTH - GL!
```

---
## \#6 Posted by: ecuadorche Posted at: 2016-08-12T18:59:30.581Z Reads: 73

```
My charger is a Tenergy tb6b and i have these batteries https://www.commonsenserc.com/product_info.php?products_id=101

and these alarms

http://www.ebay.com/itm/NEW-RC-Lipo-Battery-Low-Voltage-Alarm-1S-8S-Buzzer-Indicator-Checker-Tester-LED-/231871034687?hash=item35fc97353f:g:~V8AAOSwYIhWkUjX
```

---
## \#7 Posted by: sl33py Posted at: 2016-08-12T19:12:34.302Z Reads: 69

```
Those alarms are exactly what i'm talking about.  BTW i frequenly fill one of the beepers w/ hot glue to muffle it a bit - they're LOUD.

Those batteries - can't find the specs, so you'll have to call the company to ask.  I'd also look on the battery itself - seems a bit ridiculous to not state max C.  I'd be cautious and stick to 1C if unknown (or obviously less like i mentioned).

If you haven't actually bought them yet - maybe check out some of the packs on HK to compare.  Better specs shown for every battery.

GL!
```

---
## \#8 Posted by: ecuadorche Posted at: 2016-08-12T19:16:08.418Z Reads: 66

```
they say max charge rate is 4 amps what is that in C?
```

---
## \#9 Posted by: sl33py Posted at: 2016-08-12T19:40:34.907Z Reads: 64

```
1 C.  Your C is related to your pack capacity.  Yours is 4 Ah (4 amp hours) or 4000mAh (4000 milli amp hours) (same thing).  So 1c *4Ah = 4Amps charge rate.  Like i said - usually a good conservative estimate of max charge rate.  More and more i'm seeing 5c and 8c capability, but i still rarely charge much faster than .5 to 1c.
```

---
## \#10 Posted by: ecuadorche Posted at: 2016-08-12T19:41:30.880Z Reads: 62

```
im charging these at 3.0 amps
```

---
## \#11 Posted by: sl33py Posted at: 2016-08-12T21:43:24.223Z Reads: 50

```
.75 C - that should work well and not beat up on your pack too much.  If you can take the time .5 or 2a would be even better for long term pack life.  From what i've read at least.
```

---
