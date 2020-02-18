# Just found a busted Razor scooter on the street

### Replies: 21 Views: 1279

## \#1 Posted by: longhairedboy Posted at: 2017-11-29T02:25:26.430Z Reads: 247

```
Any tips for running VESCs with a brushed DC motor? I think it will do it, i just don't know how the wiring works.
```

---
## \#2 Posted by: JLabs Posted at: 2017-11-29T02:40:10.359Z Reads: 238

```
You stole this from a poor little kid with a bowl cut didn’t you? 

https://media0.giphy.com/media/cwyIPOzZ8RjUI/giphy.gif
```

---
## \#3 Posted by: Rinzler Posted at: 2017-11-29T02:42:34.609Z Reads: 236

```
Found something on the interwebs, this text is copied and pasted, and it is not mine. Plenty of pictures in the link below. Why are you trying to do this, there are brushed ESC-s available, maybe you bring VESC sacrifices to our lord Skatan. **Hail Skatan**! 

 "I haven't tested this theory yet, but I would assume (with my somewhat limited knowledge of electronics, and having seen the response of a brushed motor on a brushless ESC) that the brushless ESC and motors are set up with a 2-phase alternating current. This would mean that the blue and red wires are always positive alternating on and off, and the black wire is always a ground. I'm going to test my theory tonight, but I believe placing a diode on the incoming blue and red leads to prevent them from shorting back on themselves would be an easy conversion from brushless to brushed without adding any significant weight, and without having to buy a different ESC. I'll update this thread if it works (or not). The final wiring would look like:

Note: If you're going to try this for yourself before I post results up here, I'd suggest you make a set of "jumper" leads to do it with; absolutely don't cut the leads off your ESC for it, as that will likely make your ESC useless for brushless application later, and you'll likely find yourself cutting them off again later. If it works, I would build the diodes into the motor leads, as the motor will then work with either a brushless or bushed ESC (providing my theory is right). To hook a brushed ESC to it later, just only use one of the leads for your positive input, and leave the other hanging (the diode will prevent it from shorting on anything).

As an alternate theory, just in case it is a 3-phase with all wires alternating between positive and negative, a series of 6 diodes should also level the current, which I will try if the 2 diode system fails to work as expected. The 6 diode system would be a lot more complex, but still totally do-able, and still while adding only an insignificant amount of weight. The 6 diode system's wiring would look something more like:

The second method I mentioned works swimmingly. Make sure you get diodes that can handle the appropriate amperage, or they'll overheat and melt through pretty much anything around them. In other words, you can't use 1000V/1.5A diodes for an 11.1V/30A ESC. You'll need diodes that can handle 30 amps for a 30 amp ESC. Also, don't shoot for a 600V/30A diode if you can find anything else, the closest to the proper voltage and amperage you can get is best. Mouser sells a rectifier diode that's rated 30V/30A that would be well suited for the task. The problem with getting the higher voltage diodes is that they will reduce your voltage. The 1000V diodes that I have here won't even let the motor spin up due to voltage drop."

The forum link: http://www.rcuniverse.com/forum/electric-rc-helis-167/1617089-brushed-vs-brushless-esc-question.html
```

---
## \#4 Posted by: b264 Posted at: 2017-11-29T03:00:52.725Z Reads: 204

```
For brushed DC, you don't need a VESC.

VESC is for a three-phase motor, also called a three-phase brushless DC motor (BLDC), even though it runs on AC and not DC...

You'll need a totally different controller, of which I know very little.
```

---
## \#5 Posted by: GrecoMan Posted at: 2017-11-29T03:02:19.512Z Reads: 203

```
chuck a 6374 on there!

although I know @chaka’s website states that his vescs can be used with DC motors... maybe he can tell you something
```

---
## \#6 Posted by: Colson003 Posted at: 2017-11-29T03:05:27.846Z Reads: 211

```
<img src="/uploads/db1493/original/3X/f/1/f12ca0df0c63e4c794c840aa4b1ec0e6b2c06aa6.jpg" width="281" height="500">
```

---
## \#7 Posted by: Kug3lis Posted at: 2017-11-29T03:34:31.346Z Reads: 181

```
AC is then voltage crosses zero to negative side... There are no negative voltage so its only PWM driven DC
```

---
## \#8 Posted by: b264 Posted at: 2017-11-29T03:58:25.586Z Reads: 181

```
All voltage is relative.  If that were true, then in that same sense, you could connect a 360V battery to your mains AC power line in your house and say the other mains wire is DC because it never crosses negative, relative to the other battery terminal.  It's not the absolute value that determines this, it's the **cyclical** electrostatic potential changing relative to time that makes something AC.  It is most definitely AC, true to the meaning of the words.  If you connect a *big enough* capacitor in *series* with *each* esc output, the motor could still run.  This cannot be the case if it was DC, it would stop once the capacitor charged.  Such as a brushed DC motor with capacitors in *series* with its supply lines.
```

---
## \#9 Posted by: longhairedboy Posted at: 2017-11-29T05:14:27.902Z Reads: 158

```
A and C. There it is, thank you. 

YEah anyone who's ever loaded bldc tool knows it can do it. The option is sitting there right in the middle of FOC and BLDC. 

Why? BEcause i have a whole bin of 4.12s and i don't need to buy anything. And because fun.
```

---
## \#10 Posted by: longhairedboy Posted at: 2017-11-29T05:32:06.844Z Reads: 150

```
i threw a bag of skittles, then @psychotiller's mom ran after them, so i then stole her scooter.
```

---
## \#11 Posted by: psychotiller Posted at: 2017-11-29T05:41:14.379Z Reads: 143

```
Makes sense, you probably like the dildo seat...
:joy:
```

---
## \#12 Posted by: Lawndart Posted at: 2017-11-30T03:00:04.920Z Reads: 108

```
Keep us updated. I have a razor e300 I'm fixing up. I got it for $60 and upgrade the esc to a 20amp model. There are 500w, and 400w motor that will drop right in, and a 1000w motor that fits with a little cutting and grinding.
```

---
## \#13 Posted by: longhairedboy Posted at: 2017-11-30T05:19:59.044Z Reads: 100

```
we found a massive sensored brushless inrunner we're going to try. not sure of the exact size of it. Came off a tronix off road board.
```

---
## \#14 Posted by: JohnnyMeduse Posted at: 2017-11-30T05:31:29.397Z Reads: 99

```
We all need to which one will be safer, between the turbo penny and ??? Turbo Razor??? Because why not also upgrading the battery?
```

---
## \#15 Posted by: Lawndart Posted at: 2017-11-30T05:43:50.671Z Reads: 95

```
I think there's a 40mph razor out there. Heard it mentioned in a scooter modding group. The razor e300 and e200 are popular scooters to mod. Alot of them can be gotten for as little as $20 bucks beacuse they had defective speed controller that fail long before the battery die.
```

---
## \#16 Posted by: longhairedboy Posted at: 2017-11-30T06:00:07.549Z Reads: 90

```
totally replacing this crap lead acid with a BMS and giant lipo pack. Don't have spare 18650s at the moment but we can get some big ass lipos off hobby king or some shit and use one of my old 4.12s. need to figure out the chain drive though. or see of we can go belt. 

or maybe put a pair of @psychotiller's six shooters on there and belt drive it.
```

---
## \#17 Posted by: longhairedboy Posted at: 2017-11-30T06:03:46.024Z Reads: 87

```
looks like its a 2000 watt ZWN-7055HB , JQ1610, whatever that means. brushless inrunner, sensored, but its got 5 sensor pins instead of 6. I wonder how that would wire into the sensor ports of the vesc.
```

---
## \#18 Posted by: JohnA Posted at: 2017-11-30T14:56:52.365Z Reads: 73

```
It’s possible it just doesn’t have the tempature sensor, so it’s probably wired 
Grnd, h1, h2, h3, 5v if I had to guess
```

---
## \#19 Posted by: longhairedboy Posted at: 2017-11-30T15:35:27.990Z Reads: 68

```
probably wouldn't kill anything to wire it up that way and try detection, yeah?
```

---
## \#20 Posted by: JohnA Posted at: 2017-11-30T16:54:50.936Z Reads: 55

```
I don’t think I’ve read of anyone blowing up their vesc in detection. So go for it!
```

---
## \#21 Posted by: Martinsp Posted at: 2017-11-30T17:07:45.671Z Reads: 48

```
VESC has in-line resistors on the input of hall sensors so they limit current on the signal lines. I would be more worried of blowing the halls than the VESC itself.
```

---
