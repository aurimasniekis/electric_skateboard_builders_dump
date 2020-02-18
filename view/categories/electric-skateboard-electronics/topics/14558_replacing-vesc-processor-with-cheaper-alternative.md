# Replacing VESC processor with cheaper alternative

### Replies: 3 Views: 2111

## \#1 Posted by: bertoncelj Posted at: 2016-12-12T18:27:40.954Z Reads: 164

```
Hello. I am new around here, and week ago I started to look for ideas to build, electric longboard. I found builds online when they use much cheaper components meaning ESC for around 30 €. But when I came to eSk8 site, here builders/ makers strongly suggest taking VESC, but it come with a price tag, which I am not happy about. 
When I look up VESC I saw, there a 3 main components:
- Processor STM32F4 64LQFP
-  Mosfet driver DRV8302 
- 6 MOEFETs IRFS7530

My idea is to bring overall price down, replacing custom 4 layer made board, with a STM32F407VG Discovery board. I will make a electric circuit with just Mosfet driver and FET on it and connect it with my STM32F4 Discovery board, so at the end I will have to separately boards. One will be mine with Mosfet Drivers, FETs, electronic and another off the shelf made STM32F4 Boards wired together.  I can get those free STM boards like STM32F3 discovery, STM32L0, STM32L1... My thoughts are, why should I buy processor, mounted on a board and higher my overall cost. 
I look into firmware of VESC and started to dig out information which pins are connected to mosfet driver DRV8302. If I get it correctly VESC have a great code solution for acceleration and breaks to act linear and smoothly, it also got temp. sensor, RF connectors and this code is what it make him unique for power 90kg person on a board . 
I can make myself RF controller with STM32F4 and temp. measurements, on/off... But now I must connect processor with MOSFET Driver and is this the tricky part? I imagine here you must add this "linear accelo. and breaking code" and synchronize all together  to make it work smooth. I look in firmware, and can't find where this is added. 

My questions are, is someone replace VESC processor with their own cheaper solution? I have simple BLDC motor, is there some other alternative to MOSFET Driver DRV8302? Is there a similar project out there?
```

---
## \#2 Posted by: hexakopter Posted at: 2016-12-12T22:08:01.978Z Reads: 127

```
[quote="bertoncelj, post:1, topic:14558"]
- 3 MOEFETs IRFS7530
[/quote]
There are 6 of these MOSFETs[quote="bertoncelj, post:1, topic:14558"]
My thoughts are, why should I buy processor, mounted on a board and higher my overall cost.
[/quote]
Because then the PCB becomes smaller and the traces shorter.
```

---
## \#3 Posted by: rpn314 Posted at: 2016-12-13T18:37:17.886Z Reads: 91

```
You will almost guaranteed spend more developing you're own system than using the VESC that's currently available. Benjamin Vedder (the guy who developed it, which is the "V" in VESC) started exactly where you're thinking. I'm sure you could make small variations that would have different trade-offs, but I would be shocked if you ended up with anything significantly cheaper. No offense. Vedder has been developing the VESC for many years and is currently finishing VESC 6.

Going the complete custom ESC route is not easy and using off the shelf discovery boards (which vedder started with) will most definitely take up much more space, which our boards are often already short on. And I'd even add that to get the reliability and consistency that we need to power these monsters you'll eventually end up on a custom PCB as well.

All of his work is availble on GitHub, so you can see how much work he's put into it
- [VESC Hardware](https://github.com/vedderb/bldc-hardware)
- [VESC Firmware](https://github.com/vedderb/bldc)
- [BLDC Tool](https://github.com/vedderb/bldc-tool) (the program we use to update the parameters)

As for other projects, besides the VESC 6 the only other one that I've seen even in the same realm is being developed by Raphael Chang (see [this](http://www.electric-skateboard.builders/t/raphael-chang-bms-and-esc/8952?u=rpn314) thread)
```

---
