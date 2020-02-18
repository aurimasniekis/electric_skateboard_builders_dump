# Arduino for anti spark switch?

### Replies: 12 Views: 571

## \#1 Posted by: jasonlove199450 Posted at: 2018-06-04T03:15:23.109Z Reads: 163

```
I've been wondering if it would be possible to use an arduino micro wired to a 240v relay such as this one 

https://www.ebay.co.uk/itm/5V-or-12V-1-2-4-8-16-Channel-Relay-Module-Arduino-Raspberry-PI-ARM-AVR-DSP-PIC/262722739443?hash=item3d2b7edcf3:m:mewvpRdfNf5lyx157fF9xGQ
 
I understand that the arduino will need power 24/7 but I plan on using a voltage regulator to drop the 45v (12s) power down to 5v for the arduino. and once the arduino is turned on it will turn on the relay which will turn on the longboard.
```

---
## \#2 Posted by: DougM Posted at: 2018-06-04T03:53:25.136Z Reads: 146

```
It'll work but it might not be the best approach.  The anti-spark switch that Vedder designed is much more graceful.  it's out on github somewhere.

*unless*  - you want to be able to turn on your board remotely with your phone.  Then the Arduino has some merit.  but that would require some additional components.

But a relay is pretty archaic compared with a FET.  Plus the kind of relay you'd need to drive full current would be pretty hefty.  More like a contactor than a relay.
```

---
## \#3 Posted by: Trdolan03 Posted at: 2018-06-04T06:48:41.715Z Reads: 119

```
Following. The idea of being able to turn on/off your board remotely is really cool. I wonder if there is a way to add that the the current anti sparks that torqueboards sells.
```

---
## \#4 Posted by: pat.speed Posted at: 2018-06-04T07:05:15.353Z Reads: 108

```
Very easily all you would need is an arduino and relay/ fet and the a button on your remote that when pressed moves the relay/fet to the closed position as would the push button that come with the antispark switch.
```

---
## \#5 Posted by: Quezacotl Posted at: 2018-06-04T07:47:29.178Z Reads: 95

```
Or better yet, add a modem/wifi, so you can turn the board on via internet! And make it public, so anyone can turn your board on.

But seriously jason, what are you trying to archieve? Powering arduino to power the board makes arduino just an unnecessary dummy middleman.
```

---
## \#6 Posted by: Nordle Posted at: 2018-06-04T08:30:51.191Z Reads: 84

```
Instead of a voltage regulator (because it would be always draining your battery), i would use a seperate small battery for the arduino, wich could be charged by another circuit once the board is really turned on.

Could also add some feature to that arduino, so that it is connected to ne negative discharge from a bypassed (because low current cheap version) BMS, so the board also would turn of if the BMS detects inbalanced cells. Overcurrent is handled anyways by the Vesc.
```

---
## \#7 Posted by: jasonlove199450 Posted at: 2018-06-04T22:28:53.061Z Reads: 62

```
I have a custom made programmable controller so i would like to be able to turn on my transmitter and have my board turn on as soon as my transmitter connects to the board. which yes i understand will mean my receiver will need to be on 24/7. my receiver is the arduino.
```

---
## \#8 Posted by: DougM Posted at: 2018-06-05T00:25:12.537Z Reads: 55

```
The receiver is already an Arduino?  Then it actually would be pretty easy.  You will need a modified version of Vedder's anti-apark switch that can take logic-level input and turn the FET on.  The modification is just an NPN transistor and some resistors.  Then the arduino can use one of the digital IO's to turn on the transistor, which will power the board up.

If you are going to use a regulator to keep the Arduino powered up, look into sleep mode and also make sure you are using a switching regulator because a shunt reg will put a pretty significant drain on your batteries.  I like Nordle's idea of having another battery - it would be pretty easy to have just one more 18650 with its own dedicated charge circuit that only operates when the big battery pack is plugged in.
```

---
## \#9 Posted by: Trdolan03 Posted at: 2018-06-05T07:14:14.925Z Reads: 48

```
[quote="pat.speed, post:4, topic:57743, full:true"]
Very easily all you would need is an arduino and relay/ fet and the a button on your remote that when pressed moves the relay/fet to the closed position as would the push button that come with the antispark switch
[/quote]
This would be in leu of the led switch not the actual anti spark PCB right?
```

---
## \#10 Posted by: pat.speed Posted at: 2018-06-05T08:26:07.112Z Reads: 42

```
Yes, you would still need the normal antispark
```

---
## \#11 Posted by: skelstar Posted at: 2018-06-06T00:56:50.583Z Reads: 26

```
I'm doing the same (controller)... have a FET switch on it's way that you would normally wire a low-voltage button to, but now I'm thinking about an Arduino.

Just have to think of a reason to justify doing it now :)
```

---
## \#12 Posted by: Trdolan03 Posted at: 2018-06-06T01:09:51.979Z Reads: 25

```
Would it be possible to have both options be available (Arduino/Bluetooth and led switch) for turning on the board which is not dependent on the other? (they could be used individually)
```

---
