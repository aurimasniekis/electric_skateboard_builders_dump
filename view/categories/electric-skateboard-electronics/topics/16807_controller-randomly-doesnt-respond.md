# Controller randomly doesnt respond

### Replies: 6 Views: 461

## \#1 Posted by: Ryanliu Posted at: 2017-01-28T07:50:38.728Z Reads: 71

```
Setup: Controller and reciever http://www.ebay.com/itm/172388976080?_trksid=p2057872.m2749.l2649&ssPageName=STRK%3AMEBIDX%3AIT
VESC: link not available anymore but it meets the motors wattage 
Motor: https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6374-149kv-brushless-outrunner-motor.html
Problem: The vesc responds to my controller at first then when i try to brake it loses connection briefly (or so it seems) 
the LED on the receiver stays on indicating that it is still connected.
Anyone know why this is happening?
```

---
## \#2 Posted by: ARollNation Posted at: 2017-01-28T20:03:46.699Z Reads: 54

```
What firmware version of the VESC do you have? Also make sure all your connections are solid and tight. You could be getting disturbances or noise from the environment. Do you have a ferrite ring around your signal servo wires?
```

---
## \#3 Posted by: SirDiff Posted at: 2017-01-28T21:16:01.206Z Reads: 49

```
That remote sucks, only works well if you are lucky. Maybe try it with another one
```

---
## \#4 Posted by: Ryanliu Posted at: 2017-01-29T20:18:06.693Z Reads: 33

```
i figured out that my max rpm at full break was 100. so i changed it to 100,000 just to see what happens and now the controller doesnt disconnect but the break is super sensitive to the point if i barely push the break it stops hard and my pulse width only read 40%. The pulsewidth moves consistently with my throttle so it isnt the throttle. I think my break force is really high or something. anyone know how to lower break force?
```

---
## \#5 Posted by: ARollNation Posted at: 2017-02-01T06:07:20.965Z Reads: 11

```
I was able to adjust mine in BLDC tool, it should be under the config tab. I basically used the values from the 'Part 3 Programming limits'. I believe my PW is around 30%, I believe that having a lower PW should lessen the sensitivity of the braking force. Complete assumption on my part, though.
```

---
## \#6 Posted by: Ryanliu Posted at: 2017-02-02T01:31:03.107Z Reads: 7

```
can u send screen shot of where PW is i cant find it in BLDC tool
```

---
