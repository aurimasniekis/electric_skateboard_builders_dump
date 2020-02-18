# Rotor Position Detection: Hall Effect vs Encoder

### Replies: 1 Views: 667

## \#1 Posted by: KMeyerson Posted at: 2016-07-23T06:41:00.456Z Reads: 83

```
While I wait for my new can to be milled, lets talk sensors.  Most motors come with sensors at this point or operate reasonably without them. 

I've been playing with different designs and can't shake the feeling that encoders need to be more protected.  I can either fit three, inexpensive sensors on a PCB with 15 mechanical degree spacing (required for my 120 edeg positional requirement) or a small, single sensor PCB that has to sit less than a millimeter away from a rapidly spinning set of magnets.

Encoders are practically more sensitive, but our (VESC) support for them is limited and Boosted clearly knew what they were doing.  Hall Sensors are relatively inexpensive and can take a serious beating before they're damaged and tend to have a greater range than Encoders. Encoders are an all in one solution but often have positional requirements for us (aligned to rotor axis, tracking magnets in line/perpendicular, etc).

I'm leaning towards the classic Hall Effect since they're universally accepted as a standard and mechanically/electrically robust and understood, but I'd like to hear some thoughts. Who wants encoders?
```

---
