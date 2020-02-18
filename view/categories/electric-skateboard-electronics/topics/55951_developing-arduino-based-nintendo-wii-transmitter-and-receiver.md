# Developing arduino based Nintendo Wii Transmitter and Receiver

### Replies: 4 Views: 292

## \#1 Posted by: jasonlove199450 Posted at: 2018-05-18T23:44:24.162Z Reads: 71

```
Just wondering who would be interested?? :) 

I have been developing a new PCB for the Nintendo Wii Nunchuck . Note the Nunchuck will need modifications for the pcb to work. e.g power switch installation and charger port installation and a small hole for the power indicator led.

Things You would need to add your self:

TRANSMITTER:
Nintendo wii nunchuck (for the housing)
arduino nano
Power switch
small 2s lipo Battery (possibly 1s)
Charging port
nrf2401

RECEIVER:
arduino nano 
nrf2401
male header pins

The plan is to have a small board you just solder the items to. this will help with people who would like a small compact programmable transmitter and receiver.

The Receiver outputs:
Esc
Z  
C
Brake Led output
PWM Under board led output for controlling 5V RGB led strips

The Z and C output could control underboard leds or possibly be a cruse control button depending on your skill of arduino code (a part that I'm not so good at)

The PCB board would come with a transmitter.ini file and receiver.ini file for you to upload to your transmitter and receiver once you have finished soldering on all your components which will get your new transmitter and receiver working with basic functions . 

Due to them only being fairly simply pcbs (transmitter pcb with an anolog stick and 2 buttons for the C and Z button and the receiver will be a bare bones pcb it would be very cheap.
```

---
## \#2 Posted by: Silent_bob52637 Posted at: 2018-05-19T00:02:49.969Z Reads: 57

```
I might be interested in a handful
```

---
## \#3 Posted by: erod998 Posted at: 2018-05-19T03:58:42.299Z Reads: 44

```
Definitely would be interested.
Currently building my longboard, so I would like to have a cheap controller like this. 
The PCB's should be super cheap since there aren't any components or many vias or SMD's.
I would try and change my code to support different sensitivities and top speed. Not sure how I could implement this.  
I would like the PWM output but not for RGB LEDs, but for a front LED light I could toggle with a transistor or two.
I have some SMD NRF2401's. I am sure the standard one could fit in the nunchuck but this maybe could help save space if need be.
Would the extended range version with external antenna, obviously in the deck, provide greater signal strength or reliability than two "normal" versions?

Also, if you don't like the nunchuck having two axis, I am pretty sure a drop of epoxy or something will stop the X axis, at least I think its the X axis. Inside, there is a little pin on the backside that I believe you can glue down and still keep full functionality. I know I held it with my finger and it worked, I guess the trick would be keeping the epoxy from seeping too far in.
```

---
## \#4 Posted by: jasonlove199450 Posted at: 2018-05-19T11:07:37.833Z Reads: 27

```
The pwm outputs for the RGB can be used for anything . All just depends on the code as it's just a pwm output. And about the nrf24 chips . Iv tested it with a prototype and the signal doesn't seem to be a problem with the non extended version and space isn't an issue . Also the anolog X axis is locked with suberglue so you only have the y axis control which is forward and reverse.
```

---
