# Bad acceleration - shuttering AT start (Sensored Motor)

### Replies: 5 Views: 415

## \#1 Posted by: dichter84 Posted at: 2017-07-18T16:05:23.164Z Reads: 75

```
Hi guys, 

I have a Problem with my APS Sensored Esc at my mountainboard.. 
Every time at startup my motors start shuttering, the acceleration ist fine for a few turns of the motor, but then the motor starts shuttering (feels like it lost comutation), then the esc does nothing for about  3 seconds, it does not accelerate or brake... After those 3 seconds i can accelerate and brake again... 

This happens only at startup at Slow Speed. When i have some speed everything works fine. 

Can someone tell me what i did Wrong, or what the Problem could be? 


Thanks for your help guys!
```

---
## \#2 Posted by: Eboosted Posted at: 2017-07-18T16:38:28.048Z Reads: 70

```
Did you make motor detection? Were the hall sensors detected?
.
```

---
## \#3 Posted by: Martinsp Posted at: 2017-07-18T17:10:34.623Z Reads: 62

```
Try checking your connections to the sensors (wires, connectors etc..). Had this happen when the VESC didnt "know" where the motor is, in my case the motor would not turn at all... The reason for your problem is that, I assume you are running hybrid on BLDC, so when you get over the set ERPM (default 3000) the VESC ignores the sensors so if they are not plugged in it does not care. When you are not above the set ERPM it does not see the sensors therefore does not spin the motor correctly... 
Hope this helps :)
```

---
## \#4 Posted by: dichter84 Posted at: 2017-07-21T17:44:02.507Z Reads: 44

```
i'm not using a vesc, its an alien esc...
conections are all fine, everything works, except of the start up. maby its the point where the esc switches from sensored to sensorless comutation that does not work well?
```

---
## \#5 Posted by: darkkevind Posted at: 2017-07-21T20:01:33.015Z Reads: 38

```
Sorry to hijack this thread, but I'm having a problem where my VESC seems to be cutting out (and nearly throwing me off!) When I'm accelerating fairly vigorously. It comes back after a few seconds, is that starts happening to me too?

@Eboosted
```

---
