# Solar Charging Questions

### Replies: 10 Views: 1198

## \#1 Posted by: Koto Posted at: 2017-03-26T07:23:30.286Z Reads: 133

```
Okay, so I'm trying to make a solar charger for my batteries. i have 2 8s 5000mAh batteries and I'm thinking of getting 5watt solar panels. How many solar panels do i need to charge both in 5hours? do you have a better solution?

thanks,
_xXKOTOXx_
```

---
## \#2 Posted by: smurf Posted at: 2017-03-26T10:00:37.264Z Reads: 130

```
Sounds like a fun little project to make.
Use a few panels to charge a lead acid battery all day everyday. Then just charge your lipos with the hobby charger from the big battery. How much actual power you get from a solar panel depends so many factors.
You will only get the full 5 watts on the equator at noon.
```

---
## \#3 Posted by: rpn314 Posted at: 2017-03-26T16:59:22.279Z Reads: 107

```
@Koto I love your idea, by my rough calculations, you need at least 34 panels to charge them in around 3 hours

If you charge once cell at 2.5A (0.5C, probably take 2.5-3 hours) at 33.6V you need 84 watts (2.5 amps * 33.6 volts = 84 watts). So to charge 2 batteries you either double the watts to 168 or you double the time it takes to charge. And of course, as @smurf said, you're really only going to get that 5W on the equator at noon (or during the summer at noon of wherever you live, when there's no clouds)

Some reference material for you:
http://www.tjinguytech.com/charging-how-tos/wattage-for-charging

http://www.csgnetwork.com/batterychgcalc.html
```

---
## \#4 Posted by: Namasaki Posted at: 2017-03-26T20:33:32.199Z Reads: 87

```
Are you talking about charging your Lipo batteries directly from the solar panels and if so, how will you balance them?
```

---
## \#5 Posted by: RogerD Posted at: 2017-03-28T09:15:10.998Z Reads: 69

```
If you plug the panel into a solar regulator, which goes into a car battery, which goes to power your lipo charger , and you charge at 2 amps at 33.6v (5 hours for 10,000Mah battery total), then that = 67.2 Watts.

If it is always bright sun, then you can expect around this from a 100Watt panel. I'd use 2 x 100w panels in this setup to give some headroom.

Charge any faster than 2Amps and your solar won't keep up.
```

---
## \#6 Posted by: Koto Posted at: 2017-03-29T06:29:50.347Z Reads: 57

```
Thanks for the help, I just realised that I said 8S batteries instead of 4S! Anyway, I was wondering if their is a way to charge the lipo while the lipo is being used to power the motor? Thanks!
```

---
## \#7 Posted by: rpn314 Posted at: 2017-03-29T12:31:56.202Z Reads: 51

```
As in while it's being ridden? Yes, probably in a few years. Today, solar cells cannot collect enough energy per in^2 and for their given weight to have it make any difference while you're riding.
```

---
## \#8 Posted by: jaykup Posted at: 2017-03-29T14:45:15.548Z Reads: 48

```
(16) 5 watt solar panels to recharge the batteries in an hour.  Assuming your battery life ride time is an hour, this would give unlimited range from around 10am to 2pm during periods of full sun.

Lots of variables could move that number from 10-20 panels, either way, not going to work.

Yeah, it's just not really possible to use solar panels to extend range any significant amount.

Best bet is to just get more batteries.  Either mounted on the board or carried in a backpack as spares.
```

---
## \#9 Posted by: Koto Posted at: 2017-04-07T09:19:52.940Z Reads: 39

```
@rpn314 @Namasaki @jaykup would i wire in series or parallel? Also, how do you think the panels should charge (eg. box of pannels that fold out, or on the board etc)?
```

---
## \#10 Posted by: rpn314 Posted at: 2017-04-08T19:49:42.863Z Reads: 27

```
The best solution for you is to mount panels on your house, store the energy, and then charge off the stored energy. It is not currently practical to have a portable solar charging solution for us. You can barely charge your phone with current standalone portable solar solutions, you're just not going to get the power you need to charge in any reasonable period of time.
```

---
