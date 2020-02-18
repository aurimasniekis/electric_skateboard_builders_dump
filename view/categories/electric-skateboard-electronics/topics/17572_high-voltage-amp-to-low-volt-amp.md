# High Voltage/Amp to Low Volt/Amp

### Replies: 11 Views: 684

## \#1 Posted by: Sander Posted at: 2017-02-11T20:45:37.027Z Reads: 68

```
I am trying to make a Vedder's Switch that you can use a momentary push button to turn it on and off.
Im wondering if this is the right regulator that handles the current:

**Specs:**
Wide Input Voltage Range: Operation from **4.5V** to **50V**
Overvoltage Lockout Provides Protection Up to **60V**
Internal High Side and Low Side Power Switches
**20mA** Output Current

Link:
http://www.linear.com/product/LTC3632

So my question is can it handle 30 Amps without getting fried?

Thanks in advance,
Sander
```

---
## \#2 Posted by: Pedrodemio Posted at: 2017-02-12T12:08:15.151Z Reads: 50

```
No way, but what do you want to do with it? The switch is just a mosfet that open or closes the circuit

As for the momentary switch, I think there is a moded version somewhere that do that
This type of circuit is called soft latch
```

---
## \#3 Posted by: Sander Posted at: 2017-02-12T14:02:20.754Z Reads: 38

```
[quote="Pedrodemio, post:2, topic:17572"]
This type of circuit is called soft latch
[/quote]

I know that, but I wanna make that you use the power from the antispark switch to an atmega328 microprocessor that tolerate max 100mA. and 1.8 < 5.5V. But I dont know which regulator I shall use for that...

Mhmm, I meant not replacing the mosfet but adding a regulator that turns the voltage to 3.3/5 and 50mA output.
```

---
## \#4 Posted by: Pedrodemio Posted at: 2017-02-12T14:23:06.418Z Reads: 31

```
Most of the ESC's have an integrated converter

On VESC there is a 5v pin you can use, in general rc ESC you have 5v on the red and black wires that connect to the reciever
```

---
## \#5 Posted by: Sander Posted at: 2017-02-12T14:26:02.226Z Reads: 27

```
[quote="Pedrodemio, post:4, topic:17572"]
On VESC there is a 5v pin you can use
[/quote]

I know that, but then it will be more wires etc. So do you know any switching regulator that is fit to do the job? 3.3/5V and less then 80mA?
```

---
## \#6 Posted by: Pedrodemio Posted at: 2017-02-12T14:34:32.042Z Reads: 24

```
I will use LM2596HVS, since there are already made modules, but nothing stops you to integrate that on the switch PCB

The atmega sole purpose will be to operate the soft latch?
```

---
## \#7 Posted by: Sander Posted at: 2017-02-12T14:40:33.996Z Reads: 23

```
[quote="Pedrodemio, post:6, topic:17572"]
The atmega sole purpose will be to operate the soft latch?
[/quote]

Not only that, connection via UART to VESC, and has a 2.4GHz radio too, maybe bluetooth too on my next version so you can turn of the power with your iPhone etc.
```

---
## \#8 Posted by: Sander Posted at: 2017-02-12T14:43:22.035Z Reads: 23

```
[quote="Pedrodemio, post:6, topic:17572"]
LM2596HVS
[/quote]

What does the VESC really use to turn down the volt and amp?
```

---
## \#9 Posted by: emepror Posted at: 2017-02-12T16:03:53.368Z Reads: 22

```
If your going the custom route, use TI's webench tool to design a regulator for you, give it your input/output voltages and a current output and it'll do most of the design for you.
```

---
## \#10 Posted by: Pedrodemio Posted at: 2017-02-12T16:35:47.506Z Reads: 20

```
That's exactly the setup I'm using, but with the 5v from VESC, take care of a good filtering before feeding power into the arduino and radio module or you will have conection issues

The driver chip (DRV) has an integrated buck converter
```

---
## \#11 Posted by: Sander Posted at: 2017-02-12T17:13:54.205Z Reads: 22

```
[quote="Pedrodemio, post:10, topic:17572"]
That's exactly the setup I'm using, but with the 5v from VESC, take care of a good filtering before feeding power into the arduino and radio module or you will have conection issues
[/quote]

Cool, then I will still use that option for now.

[quote="Pedrodemio, post:10, topic:17572"]
The driver chip (DRV) has an integrated buck converter
[/quote]

I thought so, thanks anyway ;)
```

---
