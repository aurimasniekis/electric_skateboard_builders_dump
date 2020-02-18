# VESC HW4.12 total dead-time of the MOSFETs?!

### Replies: 4 Views: 566

## \#1 Posted by: ThierryGTLTS Posted at: 2017-09-12T15:18:00.479Z Reads: 92

```
Hello,

I noticed that the dead-time of the MOSFETs seems to be composed of 3 parts.

1. HW part DRV8302 (or 01), 10K sets 80nS dead-time, 50µS the min possible + 3nS/1K of resistance.
2. In mc_interface.h #define mcpwm_dead_time_cycles 60, but I ignore the lenght of one cycle, help, please :!:
3. In BLDC Tool or VESC Tool, you can find dead-time compensation, preset to 0.08µS.

So is the total dead-time equivalent to the sum of those 3 parts, and how long (in nS) is the lenght of a cycle :?::!:

Have a Nice Day.

Thierry
```

---
## \#2 Posted by: ThierryGTLTS Posted at: 2017-09-14T07:52:45.993Z Reads: 57

```
Good Morning,

Is my question so hard to respond?!

For me it's important because I wanna change the Mosfets with others that have different switching characteristics.

Have a Nice Day.

Thierry
```

---
## \#3 Posted by: Nordle Posted at: 2017-09-14T07:54:55.544Z Reads: 52

```
www.vedder.se
you could ask there, good luck
```

---
## \#4 Posted by: ThierryGTLTS Posted at: 2017-09-14T10:54:42.693Z Reads: 48

```

   Here is the response !

1. HW part DRV8302 (or 01), 10K sets 80nS dead-time, 50µS the min possible + 3nS/1K of resistance.
2. In BLDC Tool or VESC Tool, you can find dead-time compensation, preset to 0.08µS allow the user to reduce the HW deadtime.
3. In mc_interface.h #define mcpwm_dead_time_cycles 60, and a cycle is about 6nS because of the 168MHz CPU clocking.

Have a Nice Day.

Thierry
```

---
