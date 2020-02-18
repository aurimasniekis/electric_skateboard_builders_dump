# Voltage question

### Replies: 2 Views: 149

## \#1 Posted by: 702vegas Posted at: 2019-05-28T00:54:59.794Z Reads: 60

```
is the voltage after the capacitor to the pcb, using a tb vesc 4.12, supposed to be current battery voltage? i set it up in the program. setup the remote. went to see if i can get a slow rolling start with the throttle and didnt get the rpms up high, and the whole thing shut down, no lights just dead. checked connections and tested voltages on certain parts. i checked the voltage from capacitor wires to the pcb and read 2.4v. trying to search but not sure if i am using the right terminology
```

---
## \#2 Posted by: Gamer43 Posted at: 2019-05-28T02:18:26.369Z Reads: 51

```
VESC is dead, most likely the DRV8302.

@JohnnyMeduse offers a repair service. 

There's a short circuit somewhere, it's not uncommon for TB VESCs to die on first use, happened to my friends VESC, which I later fixed.

However, the other possibility is there is a problem with the BMS, disconnect everything from the battery and probe the voltage with a multimeter.
```

---
