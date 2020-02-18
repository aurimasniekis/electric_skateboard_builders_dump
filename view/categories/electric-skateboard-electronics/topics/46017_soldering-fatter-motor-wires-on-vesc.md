# Soldering fatter motor wires on vesc?

### Replies: 11 Views: 395

## \#1 Posted by: Hummie Posted at: 2018-02-10T08:02:46.601Z Reads: 107

```
is it risky to the rest of the board to take off the 12awg on the focbox and replace them?  wanted to do 10awg and longer.
```

---
## \#2 Posted by: Nordle Posted at: 2018-02-10T08:41:02.574Z Reads: 97

```
Shouldn't be a problem, touch the fets while you're doing this. If you don't burn your skin, they should be fine;) You won't need thicker wires on the motor side tough, even if you have crazy vesc settings. Longer dunno but you always could make extensions.
```

---
## \#3 Posted by: SOICDIP Posted at: 2018-02-10T09:03:26.124Z Reads: 97

```
[quote="Hummie, post:1, topic:46017, full:true"]
is it risky to the rest of the board to take off the 12awg on the focbox and replace them?  wanted to do 10awg and longer.
[/quote]

Like others will say, it won't really affect your output that much, as the difference is negligible. 

However, you should be able to replace wires without a problem, as long as your soldering iron can deliver enough power to melt the solder. Keep in mind that the wires will get very hot during soldering.
```

---
## \#4 Posted by: Schulerbible Posted at: 2018-02-10T09:36:45.200Z Reads: 84

```
12 AWG should be more than enough.
```

---
## \#5 Posted by: Acido Posted at: 2018-02-10T10:59:35.125Z Reads: 66

```
Provably not if the wires are long (from vesc to motor)
```

---
## \#6 Posted by: Nordle Posted at: 2018-02-10T11:13:51.086Z Reads: 65

```
Probably it doesn't matter anyways. AC from esc to motor isn't affected that much from inductance like it's the DC from battery to ESC...
just probably
```

---
## \#7 Posted by: Jammeslu Posted at: 2018-02-10T11:59:16.100Z Reads: 54

```
So How would the 14awg on the focboxes be? Should I replace them with 12awg ?
```

---
## \#8 Posted by: Nordle Posted at: 2018-02-10T12:46:23.291Z Reads: 52

```
No need imo
```

---
## \#9 Posted by: deucesdown Posted at: 2018-02-10T14:06:45.986Z Reads: 45

```
@Hummie if you go longer for the battery wires you may want/need more capacrtors. I think 12awg is sufficient for lengths used in skateboards.
```

---
## \#10 Posted by: SOICDIP Posted at: 2018-02-10T15:04:38.545Z Reads: 35

```
[quote="deucesdown, post:9, topic:46017"]
if you go longer for the battery wires you may want/need more capacrtors
[/quote]



Good point, especially if you're running your setup at 12S.
```

---
## \#11 Posted by: Nordle Posted at: 2018-02-10T15:20:04.315Z Reads: 31

```
No as your voltage gets higher amperage drops, for the same wattage. And the amps are causing inductance not the volts. As your voltage becomes higher your wires may be thinner and vice versa.
So especially for 6S and lower builds you need thicker wire.
```

---
