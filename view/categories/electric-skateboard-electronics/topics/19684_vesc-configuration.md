# VESC Configuration

### Replies: 14 Views: 1873

## \#1 Posted by: Andy12 Posted at: 2017-03-25T20:50:24.594Z Reads: 150

```
Does anyone have some decent configurations for a 260kv motor. 
Want to go about 25 at max speed.
```

---
## \#2 Posted by: bullrider12 Posted at: 2017-03-25T20:54:40.672Z Reads: 152

```
http://www.electric-skateboard.builders/t/vesc-settings-for-maximum-potential-8s-260kv/10678
```

---
## \#3 Posted by: Andy12 Posted at: 2017-03-25T20:56:23.245Z Reads: 143

```
I use Multistar Batteries and I have it in Series, 6s
would it change the config at all
```

---
## \#4 Posted by: bullrider12 Posted at: 2017-03-25T20:59:18.787Z Reads: 139

```
It would change the Batt Max + Min and the Battery cutoff start + end. But there was an issue using 260 kv with 6s battery. I dont know exactly what is was, but maybe you can find it here:

http://www.electric-skateboard.builders/t/choosing-the-right-motor-kv-for-the-vesc/3125
```

---
## \#5 Posted by: Andy12 Posted at: 2017-03-25T21:01:25.453Z Reads: 126

```
what would you change it to.
```

---
## \#6 Posted by: bullrider12 Posted at: 2017-03-25T21:27:15.975Z Reads: 114

```
What is the c-rating of your battery?
```

---
## \#7 Posted by: Andy12 Posted at: 2017-03-25T22:46:42.341Z Reads: 109

```
I thinks it's 10c, how can you find out for sure
```

---
## \#8 Posted by: Andy12 Posted at: 2017-03-25T22:51:39.231Z Reads: 107

```
its for sure a 10c
```

---
## \#9 Posted by: Andy12 Posted at: 2017-03-28T14:22:46.223Z Reads: 96

```
Got any Configurations?
```

---
## \#10 Posted by: jaykup Posted at: 2017-03-28T15:25:24.923Z Reads: 90

```
10c = 10 x capacity

so if it's a 5,000mah battery, 10 x 5,000 = 50,000mah or 50amps.

So set battery max to 50A in that example above.

My suggestions:

motor max 70A
Motor Min -50A (adjust this if braking is too weak or hard)

Battery Max 50A (10c, 50A based on the example above - adjust for your actual battery capacity)
Battery Min -10A (2c, -10A based on the example above - adjust for your actual battery capacity)

Min Volt: 8v
Max Volt: 30v
Bat Cutoff Start: 20.4v
Bat Cutoff End: 19.8v
```

---
## \#11 Posted by: Andy12 Posted at: 2017-03-28T21:54:55.482Z Reads: 85

```
Sweet that's what i'll try and find out if it works. Thanks man.
```

---
## \#12 Posted by: Andy12 Posted at: 2017-03-28T21:56:48.583Z Reads: 85

```
Sorry I have 2 3s batteries that are multistar. Would that change the config at all or would it stay the same as above.
```

---
## \#13 Posted by: jaykup Posted at: 2017-03-29T22:26:57.361Z Reads: 74

```
If you are running 2 3s batteries in series then the above settings will work.  It's setup for 6s (2x3s).
```

---
## \#14 Posted by: Andy12 Posted at: 2017-03-30T16:07:13.587Z Reads: 62

```
nice new to this 
Thanks
```

---
