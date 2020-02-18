# SAFE OR DUMB ? VESC 4.12 FOC seems to work with 12S + low KV motors

### Replies: 3 Views: 807

## \#1 Posted by: JullianS Posted at: 2017-06-30T07:48:34.647Z Reads: 196

```
Hi guys,

I have used for a while a 12s Battery plus a 130kv Hub motor (2 of them before one one them fell appart for other reasons), using those on a daily basis without getting any DRV Faults at all, even in 12S FOC with cheap Maytech VESCs 4.12... 
I am now running an even lower 75kv Hub motors that my company is testing, and still, nothing wrong, with the same VESCs. 

I tried to reason this therory with Kv/RPM/BatteryVoltage mathematics, but it just made me more confused...

Am I a crazy person just asking to get his face smashed on the ground or is FOC only problematic with High Kv satellite motors ?
```

---
## \#2 Posted by: Maxid Posted at: 2017-06-30T08:17:16.711Z Reads: 193

```
I have two US made Enertion 4.12 VESCs that I hooked up to Jacob Hubs (<90kv).
Riding them with FOC at 10S caused one of them to show DRV errors that lead to the VESC restarting - it still worked and I did not realize this during skating. Only by using @Ackmaniac's Android App was I able to tell that there was something going on. It did not burn the DRV but could have in the future - I switched back to BLDC mode.

FOC stays a risk - even with Hub motors.
```

---
## \#3 Posted by: Michaelinvegas Posted at: 2017-06-30T08:57:04.681Z Reads: 181

```
I run single carvon 85kv at 12s FOC on an enertion FOCbox

7 months so far zero issues. It's how I initially set it up and haven't changed any settings.
```

---
