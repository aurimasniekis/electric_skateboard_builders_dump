# Charging in series question

### Replies: 9 Views: 587

## \#1 Posted by: Pickwick Posted at: 2017-07-22T20:33:34.894Z Reads: 49

```
Hello there. 

I have a 5x2S pack installed on my board, and as I was putting it all together I thought of something. 

I want to charge all the 5 packs individually through the balancing leads, but can you do that if the main leads are welted together??
I want to buy 5 of these small chargers and charge each battery through the balance leads as mentioned.  
https://hobbyking.com/en_us/turnigy-12v-2-3s-basic-balance-charger.html

I just want to know if it is possible to do it, without crashing the chargers.  

Thank you
```

---
## \#2 Posted by: Sander Posted at: 2017-07-22T20:55:45.342Z Reads: 42

```
Dont think so, you need to disassemble them from the series.
```

---
## \#3 Posted by: wafflejock Posted at: 2017-07-22T21:00:04.842Z Reads: 44

```
I only have two batteries so I just have the loop key between the two batteries so I can disconnect them from each other while charging.... Could do something similar but would need 4 of em to go between each of the batteries, better bet in this case is probably a decent BMS.

Believe balance chargers charge the whole pack through the main leads and trickle discharge through the balance leads if the cells get too far away in voltage but could be the other way around either way my charger needs both connected.
```

---
## \#4 Posted by: Pickwick Posted at: 2017-07-22T21:18:31.780Z Reads: 34

```
This small charger only charges through the balance leads.
Its just a problem for me with a BMS because I can't get one to my country without paying a giant amount of money .. 
But thanks
```

---
## \#5 Posted by: wafflejock Posted at: 2017-07-22T21:22:17.595Z Reads: 31

```
No problem, yeah I'm not a big fan of having that strapped on the board anyhow personally but can see @darkkevind's at home "BMS" here too if you have a pile of TP4056 around it can work but he mentioned issues with trying to concurrently have them all connected I would basically be worried about similar kinds of loops/connections being made unintentionally:

http://www.electric-skateboard.builders/t/temporary-charging-balancing-solution/27266/4
```

---
## \#6 Posted by: Pickwick Posted at: 2017-07-22T21:33:11.222Z Reads: 30

```
Interesting solution :stuck_out_tongue:
```

---
## \#7 Posted by: darkkevind Posted at: 2017-07-22T22:12:57.891Z Reads: 26

```
That was great to balance them all when I got them, but now i have a proper BMS connected and all sealed up nicely in some shrink wrap.

@Pickwick you most definitely can't do what you're asking. For one, you will only be able to connect one pack to your charger's balance leads at any one time, you will have to set whether it's 2s or 3s before charging and it will expect the voltage (of the main battery wires) to be somewhere in the 2s or 3s range.
Your battery in series will show up as 42v whereas it's expecting 7.4 or 11.1. It just won't work. 

However if you spur off each battery's main wires with another xt60 connector, you can leave them all connected and just connect to one at a time, including balance leads respectively...
```

---
## \#8 Posted by: lowGuido Posted at: 2017-07-22T22:32:06.380Z Reads: 26

```
https://youtu.be/O5gi35AtPSw?t=4m27s
```

---
## \#9 Posted by: Pickwick Posted at: 2017-07-23T07:52:59.639Z Reads: 22

```
Thank you.
```

---
