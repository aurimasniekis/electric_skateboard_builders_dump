# Why higher voltage is more power

### Replies: 3 Views: 286

## \#1 Posted by: Hummie Posted at: 2018-06-26T16:21:49.330Z Reads: 127

```
Why do I get Better acceleration w full charge (higher voltage ) on current control?  I thought w pwm the voltage the motor sees is decided by only the current limits
```

---
## \#2 Posted by: skatardude10 Posted at: 2018-06-26T16:41:06.454Z Reads: 117

```
Pretty sure it's because current x voltage = power/watts. Higher voltage = more watts. Set a current limit, max that limit, the power will still drop as voltage in the pack drops.

I notice that as well. That's why if I'm just cruising, I set a wattage limit to the minimum pack voltage I'm willing to to ride down to, minus 3v to account for voltage drop, multiplied by my max amp limit, to get consistent acceleration during the entire ride. If I'm just going out for fun, I go on a full charge with no wattage limit and get crazy acceleration at the beginning.
```

---
## \#3 Posted by: linsus Posted at: 2018-06-27T14:04:01.428Z Reads: 61

```
Well, if you wanna go all nerdy about it. A BLDC motor is essensially alot of inductor coils connected together. So what characterizes an inductor? Compared to its counterpart, the capacitor that Draws current to keep a voltage, an inductor draws voltage to maintain current.

Going more complex into why x happens at y time I wont do here. But if you're really intrested go to the library and check out some of the books about motors and generators. The Tech isnt exactly groundbreaking new and theres tons of stuff to read. Having the fundamentals for Electronics does help quite alot Before that tho.
```

---
