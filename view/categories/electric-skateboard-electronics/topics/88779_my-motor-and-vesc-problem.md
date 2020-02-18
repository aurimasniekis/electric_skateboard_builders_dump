# My motor and vesc problem

### Replies: 8 Views: 168

## \#1 Posted by: Swaight Posted at: 2019-03-30T14:57:03.160Z Reads: 48

```
My motor has a 5 pin sensored wire and my vesc has a 6 pin sensored connector is there a adapter I can buy to fix this or do I need to buy a different vesc or motor?
```

---
## \#2 Posted by: mccloed Posted at: 2019-03-30T15:18:46.394Z Reads: 43

```
Pictures of the connector would help. Some motor manufacturers don't use the temp sensor.
```

---
## \#3 Posted by: Steven1 Posted at: 2019-03-30T15:22:45.038Z Reads: 39

```
https:///products/vesc-sensor-wires
```

---
## \#4 Posted by: rojitor Posted at: 2019-03-30T15:25:45.983Z Reads: 36

```
Respect positive (red) and negative(black)
You just need a 6 pin connector. Your vesc probably has the name of each pin.

5v or vcc- red

Temperature or T -ignore this

H3

H2

H1

Ground or negative- black

You can remove the pins easily with a screwdriver and then place them into a 6 pin connector
```

---
## \#5 Posted by: Swaight Posted at: 2019-03-30T15:32:26.704Z Reads: 33

```
Thanks how does this look?![image|375x500](upload://z2W5Zh6x9WWiONfa4ZYEOaAEyP4.jpeg)
```

---
## \#6 Posted by: mccloed Posted at: 2019-03-30T16:39:07.296Z Reads: 29

```
Yup. That's what i figured. Should plug right into the sensor port. It just doesn't have the Temp Sensor on the motor so the missing wire is not necessary.
```

---
## \#7 Posted by: wafflejock Posted at: 2019-03-30T16:44:56.411Z Reads: 28

```
Assuming black is gnd and orange is 5V you should be good, be sure you plug into the right port on the VESC I accidentally used the wrong 6 pin header and it wasn't fully booting (not sure if something was shorted or it just detected an issue).  Luckily didn't fry anything there.
```

---
## \#8 Posted by: rojitor Posted at: 2019-03-30T20:10:54.125Z Reads: 16

```
Looks fine. Just make sure +&- are not messed.
```

---
