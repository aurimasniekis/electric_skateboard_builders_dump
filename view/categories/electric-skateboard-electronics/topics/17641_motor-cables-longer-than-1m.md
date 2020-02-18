# Motor cables longer than 1m?

### Replies: 8 Views: 803

## \#1 Posted by: TarzanHBK Posted at: 2017-02-13T11:43:21.734Z Reads: 103

```
So I have an upcoming project "Toddler wagon" where I need to bridge about one meter from battery and Vesc to two motors.
What do you guys think about this distance from vesc to motors? Any experience or advise? Possible or do I need to do some modification?
```

---
## \#2 Posted by: SirDiff Posted at: 2017-02-13T12:06:04.489Z Reads: 99

```
Somebody said you would need bigger capacitors on your vesc if you go over 12 inches of cables from battery to vesc, I don't really know about motor cables though
```

---
## \#3 Posted by: Pantologist Posted at: 2017-02-13T13:22:19.366Z Reads: 87

```
Yeah that's correct...

 I think the resistance of the wires for the motor phases will mess up Vesc motor detection though.
```

---
## \#4 Posted by: TarzanHBK Posted at: 2017-02-13T13:26:22.603Z Reads: 83

```
yep from battery to Vesc for sure, but in this case they are close, only the motors are farther away, so I´m not sure what to do here..
```

---
## \#5 Posted by: TranxFu Posted at: 2017-02-13T13:26:33.840Z Reads: 79

```
on the battery-vesc side, are the 3x 680uf not enough for lengths up to 50cm ?
```

---
## \#6 Posted by: TarzanHBK Posted at: 2017-02-13T13:27:41.403Z Reads: 83

```
should be ok in bldc, but could cause some trouble with foc.
```

---
## \#7 Posted by: TranxFu Posted at: 2017-02-13T13:31:44.924Z Reads: 83

```
Oh alright thanks mate ! Do you happen to know if there will be any difficulties if a cable goes from one battery pack(10s4p) to the other one and the cable in between is approx 50cm ? 
E.g. a split enclosure with the 10s4p splitted between both enclosures.
```

---
## \#8 Posted by: TarzanHBK Posted at: 2017-02-13T14:18:57.558Z Reads: 73

```
you´ll definitely create some electrical noise with this. Some Vescs don´t mind, some blow theire DRV.. it´s still a mystery why.. But upgraded capacitors are not bad in this case and should bring any disadvantages. 
So I would simply throw a second capacitor board in there. Some people did this before and don´t seem to have problems with longer cables anymore.
http://www.electric-skateboard.builders/t/add-vesc-capacitors-for-battery-cables-longer-than-12inch-30cm/12506/15
```

---
