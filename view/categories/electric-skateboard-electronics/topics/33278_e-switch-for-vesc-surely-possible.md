# E-Switch For VESC - Surely Possible?

### Replies: 14 Views: 704

## \#1 Posted by: darkkevind Posted at: 2017-09-16T18:56:02.751Z Reads: 158

```
I was thinking, all these BMS' and some cheaper ESCs manage to put a tiny little switch in to turn the ESC (and basically the board and receiver) on and off, there must be somewhere on the VESC board we could intercept to cut the power to the components that would drain the battery should you leave it constantly on? I mean, cut the power to the parts that power the receiver and you're practically there right?

If you left the battery connected but managed to "turn off" the VESC, what harm would that do? The caps would be constantly charged I guess... is that a problem?

What are your thoughts? Perhaps there's a VESC guru that could comment?

@chaka @esk8 @trampa @JohnnyMeduse
```

---
## \#2 Posted by: Jinra Posted at: 2017-09-16T18:58:13.060Z Reads: 155

```
I feel like this wouldn't be possible without making the pcb bigger to accomodate the extra fets
```

---
## \#3 Posted by: darkkevind Posted at: 2017-09-16T18:59:23.016Z Reads: 151

```
Why would you need fets? You're just cutting power to the really low voltage, low amperage components.... to basically turn it... off :confused:
```

---
## \#4 Posted by: trampa Posted at: 2017-09-16T19:03:22.792Z Reads: 148

```
And if you forget to really depower it, your battery is dead in a couple of weeks. Happened even to Benjamin himself. Hobby RC stuff doesn't consider constantly attached batteries. You need a FET switch to really disconnect the batteries, so that no current will flow.

Frank
```

---
## \#5 Posted by: darkkevind Posted at: 2017-09-16T19:05:22.373Z Reads: 138

```
OK so this is what I was asking. What would drain the battery if the components that power the receiver  have their power cut? What else consumes when the receiver BEC isn't being powered, or consuming power? Another component on the board?

Ps. Thanks for chiming in Frank.
```

---
## \#6 Posted by: trampa Posted at: 2017-09-16T19:10:05.618Z Reads: 135

```
W a electric circuit, which doesn't consume a lot, but enough to slowly empty your pack. If it's powered, it consumes. 

Frank
```

---
## \#7 Posted by: darkkevind Posted at: 2017-09-16T19:13:20.605Z Reads: 125

```
OK so you're saying that basically all the components on the board will consume some voltage (unrelated to the BEC) and over time will drain the source?

Makes sense.

So how do the BMS' manage it? I haven't looked in to their schematic but do they use FETs? I know they do for the charging and discharge, but for powering on and off?
```

---
## \#8 Posted by: chaka Posted at: 2017-09-16T19:26:42.494Z Reads: 115

```
I prefer modular components. Eventually, I want to provide a second battery system solely for powering the the electronics, microcontroller reciever etc.. you see where I am going with this.
```

---
## \#9 Posted by: FredSaberhagen Posted at: 2017-09-16T22:09:01.335Z Reads: 98

```
That's called quiescent current draw and it's usually not huge but over time will eventually drain anything down.   You could totally do what you're describing with a FET but look up typical on resistances and figure out the current... lots of watts.  Usually people accomplish this with a couple FETs in parallel it just takes up space and adds cost. 

If you pursue this.  Recommend you use a gate driver IC so you can use a lower resistance NFET (not PFET)
```

---
## \#10 Posted by: darkkevind Posted at: 2017-09-16T22:17:24.617Z Reads: 95

```
Yeah I know I could do it with one or more FETs, I mean, we've got the Vedder anti spark switch right? And others of course. 

But I'm just thinking that we could stop the current/voltage flow to all the components that step down the voltage to run the BEC and the on PCB standby components (we don't want the LEDs on of course), with a physical break in the circuit that gives them they're power? By means of a little tiny switch.

The major current doesn't flow until the receiver tells the VESC to do it right? If the receiver never tells it to do it, but the battery is connected all the time, but not drawing power (because power to the little components has been cut), it shouldn't be draining anything right? Then turning the little switch on turns all that stuff on and away you go... No?
```

---
## \#11 Posted by: FredSaberhagen Posted at: 2017-09-17T02:36:48.134Z Reads: 78

```
You might still want the IC powered so your phase FETs are at known gate voltages... if you want to cut it off why not do it upstream like anti spark as you say?  What's the gain to adding choice of stuff to turn off?
```

---
## \#12 Posted by: pat.speed Posted at: 2017-09-17T02:56:32.693Z Reads: 76

```
So what your saying is that if I use that little switch on RC car esc it will still drain my batteries over time?
```

---
## \#13 Posted by: Hillso Posted at: 2017-09-17T05:23:50.759Z Reads: 65

```
I think many ESCs support on/off switching (without quiescent current draw).
A VESC (or any other ESC) already have large FETs between the DRV chip and the motor I assume, so maybe an additional small and lower current transistor can be added to the logic part of the ESC's circuit.
Can anyone with more EE knowledge can approve/disprove this?
```

---
## \#14 Posted by: darkkevind Posted at: 2017-09-17T09:26:40.070Z Reads: 54

```
I know the anti spark switch isn't expensive, but if VESC makers could integrate a switch, much like that of an FVT (or similar) ESC, to switch it on and off, there wouldn't be any need for an extra component to achieve on/off functionality, thus less components to go wrong, more space in your enclosure etc.

Like I say, some BMS' have them, and some other cheaper ESCs, small switches dealing with almost zero current and low low voltage turning the system on and off, so why not (if you don't have a BMS), integrate one in to the VESC? I mean, it costs enough! At least give us a bloody switch! No? 🤔

Even better, if someone could identify a singular place on the PCB to intercept the power to these components that would drain the source, people could DIY it if they wanted, (voiding warranty I'd imagine).
```

---
