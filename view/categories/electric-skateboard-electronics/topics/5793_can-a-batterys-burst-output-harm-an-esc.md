# Can a battery&rsquo;s burst output harm an ESC?

### Replies: 11 Views: 1833

## \#1 Posted by: Brando Posted at: 2016-07-09T01:17:23.379Z Reads: 64

```
I am planning on using a 120A ESC with two 3s zippy 5000mAh 20C batteries. 5Ah x 20C = 100A which is well under the ESC limit of 120A, but the battery features a burst ability of 30C, which sets it's output at 150A. That exceeds the 120A limit of the ESC. Will this cause harm or will the ESC just not request that many Amps?
```

---
## \#2 Posted by: edwardlui531 Posted at: 2016-07-09T02:38:49.277Z Reads: 59

```
I believe you have to look at your motor and what is the max power\
p=I*V that way your know what the max current. 

120A is probably plenty for esk8
```

---
## \#3 Posted by: Stevemk14ebr Posted at: 2016-07-09T02:44:40.549Z Reads: 56

```
the esc will only draw as much current as required to pull the load. You could have a 1,000,000 amp burst battery and still be fine if you pulled a tiny load.
```

---
## \#4 Posted by: laurnts Posted at: 2016-07-09T02:45:11.080Z Reads: 57

```
Yes battery burst can dmg ESC. Still you want to get battery that can output more current than your ESC need, otherwise youll be over using and damaging your battery. Practically the motor or ESC is the one who decide how much amps to pull.

Same to your house electricity. You want to have high kwh so you can turn on most home appliances. But having them in high kwhdoesnt mean it will fry all home appliances.
```

---
## \#5 Posted by: Brando Posted at: 2016-07-09T02:58:12.329Z Reads: 47

```
Makes sense. So il be using the diy 2650W 80A motor with the diy 120A 12s ESC. For a 5000mah pack, what c value should I go for? I was hoping I could make 20c work. Theoretical 5000mah at 20c would give me 100A with a burst of 150A. Certainly this is enough for a 80A max motor?
```

---
## \#6 Posted by: laurnts Posted at: 2016-07-09T03:54:07.445Z Reads: 45

```
5000mah 20c is okay. I am currently using 5000mah 25c, but I have them in parallel so 10000mah 25c. In which it can supply 250A. I have to say 5000mah 20c is a soft start (soft acceleration board). But if you want an aggressive start with the jolt if you punch the throttle, you want higher c rating / start making your batteries into parallel setup.
```

---
## \#7 Posted by: Stevemk14ebr Posted at: 2016-07-09T04:05:02.949Z Reads: 43

```
Amps = C rating * Capacity (in Ah)

Amps = 20C * 5Ah
Amps = 100

100A supply > theoretical max pull of 80A

You are fine. Use math guys, it's not hard.

@laurnts it's smarter to put your batteries in series. They will provide double the voltage and require less amps for the exact same power. This will generate less heat and he would get EXACTLY the same range as well as startup power. This assumes of coarse he were to travel at the same speed, obviously series allows his board to go faster but if goes the same speed he will get the same range.

Watts = energy (how far you can go)
Watts = Amps * voltage
You can double the amps, or the volts. If you double the amps you get more heat which is less efficient. If you double the volts you get less heat and the same amount of power.
```

---
## \#8 Posted by: Brando Posted at: 2016-07-09T04:09:04.561Z Reads: 38

```
Thanks for the clarification @Stevemk14ebr , but I actually did do that math in my last post 😀 . Still, always good to double check my work. Ill be buying the parts shortly
```

---
## \#9 Posted by: anorak234 Posted at: 2016-07-09T07:15:29.365Z Reads: 30

```
I'm pretty sure max draw from most motors is 60 Amps. The reason we all go overkill on ESC's is so that it doesn't overheat. I'm running a zippy setup with a 150 amp right now, but I've done 120 before with no problems
```

---
## \#10 Posted by: Hummie Posted at: 2016-07-09T07:34:10.461Z Reads: 28

```
The motor will get just as hot for a given performance Regardless of Voltage. The esc will benefit from higher voltage though as wil the batteries
```

---
## \#11 Posted by: laurnts Posted at: 2016-07-09T08:18:48.008Z Reads: 26

```
I agree that putting the batteries in series does reduce the amount of heat the ESC produce. However you might miss the fact that parallel setup help reduce the load of battery during discharge. Which means with parallel setup the batteries runs cooler, but the esc runs hotter. In series, the esc runs cooler, the batteries runs hotter.

This is even worst if you have low c rating batteries and you do only series connection. Pretty sure you'll swap battery faster than swapping your esc. I'm not trying to scare you, but most ESC could handle heat more than batteries could handle heat. Lithium is very sensitive to overcharge and overdischarge.

I didn't mention anything about doubling the range. Batteries are carrying same watt hour (energy), what ever setup you use, it will still store and deliver the exact amount of energy.
```

---
