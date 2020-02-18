# Dual receiever max settings?

### Replies: 13 Views: 326

## \#1 Posted by: J95hicks Posted at: 2018-12-24T19:02:30.880Z Reads: 56

```
About my setup... i am NOT running CAN, or y split. I am using two independent Focboxes with dual receievers. So both are the master essentially i believe. I have a 12S8P battery with a *100A*BMS. I am running one 190kv sensored motor and one 149kv unsensored.. i switched to the one sensored bc i wanted smoother start and it has helped but i feel its still lacking power(acc & hill climbing) and can give more but idk bc my setup is dif from the norm and my bms.... does that mean that i should add my max values together to determine my total allowable max bc each Focbox is pulling power independently and bc of my 100 amp bms?? Example... each motor max cant be more than 50a? What about battery max? ..Current setting are. Mot max/min:45/-45 batt max/min:30/-15 
Happy Holidays, and stay safe.
```

---
## \#2 Posted by: pookybear Posted at: 2018-12-25T04:20:40.975Z Reads: 42

```
I'm gonna have similar setup but 12s4p w dual 190kv motor. 

How do you change your Vesc settings? BT module? One for each Vesc?

Subscribed.
```

---
## \#3 Posted by: Andy87 Posted at: 2018-12-25T04:36:25.165Z Reads: 39

```
It you think you need to change your settings via bt and not via pc you need two bt modules without can bus.
```

---
## \#4 Posted by: Andy87 Posted at: 2018-12-25T04:40:15.073Z Reads: 36

```
If you have a 100a bms than the bat max is 50a per focbox, not motor max.
Motor max depends on your motor rating.

Just one question besides.
You run 2 different kV motors in one board.
Does it mean you also have different gearing on the motors?
If no, than that will sooner or later cause a problem. One motor is spinning faster than the other with the same throttle.
```

---
## \#5 Posted by: pookybear Posted at: 2018-12-25T05:01:44.475Z Reads: 31

```
What if I have canbus turned on and set it uart? Will I be able to change the settings via app? 

Sorry for hijacking the thread OP.

Happy holidays!
```

---
## \#6 Posted by: J95hicks Posted at: 2018-12-25T05:03:03.355Z Reads: 30

```
I manually program each vesc on my computer. And https://www.electric-skateboard.builders/t/uneven-dual-rear-drive/113....isnt this thread essentially about the same thing. No, same gearing. How would it cause issues?
```

---
## \#7 Posted by: Andy87 Posted at: 2018-12-25T05:04:15.526Z Reads: 28

```
I think you can use CAN only for data too.
Should work.
The question is, why you want to use two receiver instead of CAN.
There are some reasons, but not all make it really necessary.
```

---
## \#8 Posted by: pookybear Posted at: 2018-12-25T05:12:45.928Z Reads: 25

```
Well. I read about those crazy canbus nightmare stories. Plus, I want to have a backup just in case one FOC malfunctions.
```

---
## \#9 Posted by: J95hicks Posted at: 2018-12-25T05:13:35.691Z Reads: 25

```
Same reason i did mine this way too
```

---
## \#10 Posted by: Andy87 Posted at: 2018-12-25T05:29:10.101Z Reads: 28

```
Ok that sound good.
never thought from this point of view.
just under no load the motors with different kV will spinn uneven at same voltage.
so this would need a different gearing to achive the same top speed.
but under load things are different. The vesc will control the rpm and that should be fine, as long as you below the max speed of the low kV motor.
```

---
## \#11 Posted by: Andy87 Posted at: 2018-12-25T05:31:56.420Z Reads: 27

```
I never had issues with CAN and the dissconnect CAN while powererd on problem is also solved with the latest hw version from the focbox.

The backup in case one focbox is fried, is definitly a reason for to go dual receiver thou.
```

---
## \#12 Posted by: J95hicks Posted at: 2018-12-25T10:09:15.129Z Reads: 20

```
Yeah, its an interesting attempt for science. My kv isnt nearly as extreme as his iether and i doubt ill reach max top speed rated for my gearing. I think its like 35 mph for the 149kv motor... so setting both my motor maxes to lets say 60, they wont both pull too many amps from the battery at the same time and go over my 100 amp bms max?
```

---
## \#13 Posted by: Andy87 Posted at: 2018-12-25T10:14:35.100Z Reads: 20

```
you need to limit your battery side, not the motor side.
bat max shouldn´t be over 50a per focbox if your bms can handle only 100a.
how much amps you put on the motor side doesn´t make any difference for your bms.
motor amps, not batt amps
look for how much amps your motors rated (usually something between 60-80a) and set it how you feel and how the motors get hot or not.
```

---
