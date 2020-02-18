# Vesc Uart stopped working

### Replies: 32 Views: 2354

## \#1 Posted by: Paulf Posted at: 2017-06-24T21:20:43.194Z Reads: 185

```
So basically the uart on my vesc just stopped working
Everything else works perfectly but I can't use uart anymore with my Bluetooth module (with any app) nor with an arduino, it just doesn't work
The vesc looks fine, every component seems to be in place
The weird thing is that it has been working intermittently for a couple of days but now it doesn't work anymore at all
I've triple checked connections... 
Has anyone got an idea about what could be the issue, has anyone already experienced that?
```

---
## \#2 Posted by: Sander Posted at: 2017-06-24T21:24:30.742Z Reads: 179

```
Check the baudrate of the UART, it might have done a reboot.

I think it should be at 115200.
```

---
## \#3 Posted by: Paulf Posted at: 2017-06-24T21:31:08.457Z Reads: 169

```
My baudrate is at 9600 but Im sure that's how it's always been and I'm pretty sure that's how it should be in order to use with my Bluetooth module
I'll try 115200 anyways
```

---
## \#4 Posted by: Sander Posted at: 2017-06-24T21:42:31.545Z Reads: 163

```
I thought 9600 is the default when it resets, Where did you buy the bluetooth thing and what baudrate did they tell you to put it on?
```

---
## \#5 Posted by: Paulf Posted at: 2017-06-24T21:48:48.970Z Reads: 158

```
My module is a standard hm-10
But I've also been using the uart of my vesc with an arduino in order to retrieve informations such as voltage, or speed 
And the vesc doesn't respond to my arduino anymore 
(I'm using 9600 baudrate for this) 
Is the uart hardware of my vesc damaged?
```

---
## \#6 Posted by: Sander Posted at: 2017-06-24T21:51:43.338Z Reads: 145

```
Are you clicking "Read Default Config" on the UART Baudrate tab?
btw, where did you  buy the bluetooth? By default they are 9600, if you bought it from the swedish guy it is 115200.

With the arduino you need to have the same baudrate as the vesc, like if its 9600 on vesc you need to set Serial.begin(9600);

And to retrieve information from the vesc you need to have
if (VescUartGetValue(VescMeasuredValues)) {
}

in the code.
```

---
## \#7 Posted by: Paulf Posted at: 2017-06-24T21:55:52.955Z Reads: 138

```
My module is from China 
I know all of this and this is exactly what I'm doing in my code 
And all of this (bluetooth module and arduino code)  was working a few days ago
I've already reset my vesc to default configuration 
I think that it probably is an hardware problem on the vesc side...
```

---
## \#8 Posted by: Sander Posted at: 2017-06-24T21:56:41.609Z Reads: 131

```
Do you have selected it as UART in the App Configuration?
```

---
## \#9 Posted by: Paulf Posted at: 2017-06-24T21:57:34.888Z Reads: 130

```
Yes I have ppm+uart selected
```

---
## \#10 Posted by: Eboosted Posted at: 2017-06-24T22:03:19.142Z Reads: 125

```
Does the red led from the hm-10 turns on when you turn on the board?
```

---
## \#11 Posted by: Paulf Posted at: 2017-06-24T22:10:07.152Z Reads: 125

```
Yes, the problem is not about power its about the communication 
I can even connect to the Bluetooth module but it doesn't display any data as it's not communicating with the vesc
```

---
## \#12 Posted by: Eboosted Posted at: 2017-06-24T22:46:22.307Z Reads: 120

```
Make sure the connections are TX on the vesc yo RX on the module and viceversa, verify the connections with a multimeter. 

Doble check the connection is ppm + UART, do that only on the master VESC, try 9600 on baud rate, delete all cached data on vesc monitor app on your phone. 

Reboot the vesc and try again. 

If the problem is still there, switch the master VESC to slave and viceversa, setup everything again on BLDC tool and try to connect. 

If nothing still happens they your hm-10 needs to be replaced.
```

---
## \#13 Posted by: Jebe Posted at: 2017-06-25T07:48:27.965Z Reads: 113

```
What version vesc firmware and the app?  Did your app update? Baud has to be 9600. I ordered two units, one worked one didn't.
Initially the app worked straight away with the first release ackmaniac firmware, then updated the app, and it stopped working. Had to load the newer firmware and it's working again.
```

---
## \#14 Posted by: Paulf Posted at: 2017-06-25T12:22:23.298Z Reads: 106

```
I do have the last ackmaniac firmware version but thre problem is not about the Bluetooth module nor about ackmaniac app
The problem is the vesc which doesn't send data over uart (I have tested it with several Bluetooth modules which I know are working and with an arduino, all of these things where working normally a few days ago but stopped working eventhough I didn't change anything)  
I'm pretty sure the uart port of my vesc is somehow fried :/...
```

---
## \#15 Posted by: TarzanHBK Posted at: 2017-06-25T12:31:01.105Z Reads: 106

```
Have you checked for faults in the BLDC tool?
Did it bring something up?
Check with a multimeter if 3,3V and 5V are available on your uart port, otherwise it might have a defective resistor somehow. Make sure not to cause a short with your multimeter tips.
```

---
## \#16 Posted by: Paulf Posted at: 2017-06-25T12:34:24.193Z Reads: 105

```
Yes, it doesn't report any faults
5v and 3.3v are available
```

---
## \#17 Posted by: Paulf Posted at: 2017-06-25T12:35:42.467Z Reads: 102

```
Very weird... It has been working for like 5 minutes and now it doesn't work again...
```

---
## \#18 Posted by: TarzanHBK Posted at: 2017-06-25T12:37:49.713Z Reads: 100

```
Hmm haven´t heard of that before... maybe @JohnnyMeduse can chim in here and has some ideas.
```

---
## \#19 Posted by: rpn314 Posted at: 2017-06-25T15:18:51.187Z Reads: 101

```
The TX and RX pins go straight to the microcontroller (no other components in between that could blow, other than the trace itself). Have you tested continunity between the solder points and the pins on the microcontroller chip itself? RX is pin 29 and TX is pin 30 (count counter clockwise, starting where the white dot on the chip is). Here's a few screenshots from the datasheet that should help find the pins (they're rotated from each other, but you get the idea)
<img src="/uploads/db1493/original/3X/f/5/f55f158b070151d77f1749aef0166f370ffc4406.png" width="561" height="500"> <img src="/uploads/db1493/original/3X/9/e/9e6da1e87f14b78beb1a928a08e844caffb9e7c0.png" width="646" height="500">



If that doesn't do it, I think you may need something like a logic analyzer to really find this ghost. Its possible that you're seeing 5v/3.3v when probing it with a multimeter, but that crumbles under load (thus indicating that the the converters may be dead)
```

---
## \#20 Posted by: Paulf Posted at: 2017-06-25T16:30:48.623Z Reads: 95

```
Thanks! I have already tried to check the continuity but I thought it was pins 14 and 15 
I'll try with 29 and 30 as you said
I'm pretty sure the 5 and 3.3v are good because I could power a Bluetooth chip from there
```

---
## \#21 Posted by: rpn314 Posted at: 2017-06-25T16:55:50.521Z Reads: 92

```
The kicad schematic from vedder's github lists 29 and 30...

[quote="Paulf, post:20, topic:26101, full:true"]
I'm pretty sure the 5 and 3.3v are good because I could power a Bluetooth chip from there
[/quote]

Hm....you can tell it's powered because of a light I assume? (Since you already said connecting to it is the problem). It is possible that it's still not getting enough power when under load (i.e. When it's transmitting since that requires a lot more power than an LED or something) and the light stays on because of a capacitor or something.... frankly I'm just shooting in the dark now. I hope it turns out to be more of a Casper ghost and not a dementor like being. But to find any of that out, you'd need an o-scope or logic analyzer to really see what the signals are doing.
```

---
## \#22 Posted by: Paulf Posted at: 2017-06-25T17:18:43.583Z Reads: 90

```
Im pretty confident it's powered, I can even connect to the Bluetooth module (but I can't retrieve any information)  with my phone which mean there is enough power to establish a wireless connection, I can even power an atmega328 from this power source 
I have just reassembled my board as I need it but as soon as I get some time I'll check the continuity with 29 and 30, thanks for your help!
```

---
## \#23 Posted by: JohnnyMeduse Posted at: 2017-06-25T17:29:03.304Z Reads: 93

```
If there where a problem with 5V or the MCU, you won't be able to connect to the VESC on USB, so I think your problem is most likely to be on the bluetooth connection or even the module itself, check to see if every wire is connect to the right spot, maybe post some picture.

Regards
JF
```

---
## \#24 Posted by: Paulf Posted at: 2017-06-25T17:45:47.184Z Reads: 89

```
Definitely not the Bluetooth module, it's working for another project of mine 
And the fact that the vesc doesn't respond to my arduino through uart (it used to) really makes me think the problem is in the vesc side
```

---
## \#25 Posted by: Paulf Posted at: 2017-06-25T17:46:54.621Z Reads: 87

```
Everything works perfectly through USB so most realistic issue to my mind is a problem with the trace...
```

---
## \#26 Posted by: Eboosted Posted at: 2017-06-26T04:59:15.128Z Reads: 83

```
Why don't you switch the slave to master VESC as stated on my previous message?
```

---
## \#27 Posted by: Paulf Posted at: 2017-06-26T05:08:46.335Z Reads: 83

```
I do have a single drive, I only have one vesc...
```

---
## \#28 Posted by: Eboosted Posted at: 2017-06-26T05:14:43.219Z Reads: 84

```
Switch VESCs from your other project and try again
```

---
## \#29 Posted by: Paulf Posted at: 2017-06-26T11:12:36.335Z Reads: 80

```
Unfortunately my other project is not about electric skateboard at all ... I only own one vesc :/
```

---
## \#30 Posted by: Paulf Posted at: 2017-06-30T18:31:24.928Z Reads: 78

```
It indeed was the trace!...
Managed to resolve the issue with some fine soldering directly on the chip
```

---
## \#31 Posted by: Moza Posted at: 2018-09-20T16:16:35.806Z Reads: 41

```
Hi. I have the same problem. I am using the ackmaniac app to monitor the stats on vesc 4.12 via bluetooth module (standard fw is up to date).

Worked fine for a few months then all of a sudden uart stopped. The app reads the battery max amps and motor max amps but voltage, current, duty etc doesnt show. 

Works from micro usb and I have checked continuity between stm pins and uart plug pins.

I have changed bluetooth module.

Anyone have any ideas?
```

---
## \#32 Posted by: QGruschkof Posted at: 2018-11-28T18:48:20.401Z Reads: 32

```
I checked my volatge under load and it suddenly droped to 2.4 volts instead of 3.2 volts so my ble modul is thinking tahtb  there is no signal at all. how to repair this
```

---
