# How much power can you draw from a 4.12 VESC UART port?

### Replies: 30 Views: 956

## \#1 Posted by: evoheyax Posted at: 2017-12-30T22:49:31.520Z Reads: 140

```
Title says it all

Basically trying to figure out if I can power an Arduino Mega, with leds, from the vesc's uart port or is this just too much?
```

---
## \#2 Posted by: mmaner Posted at: 2017-12-30T23:04:28.739Z Reads: 139

```
I'm no expert but I believe it's 5v 1a.
```

---
## \#3 Posted by: scepterr Posted at: 2017-12-30T23:09:30.703Z Reads: 138

```
How much power would that be in mA?
```

---
## \#4 Posted by: evoheyax Posted at: 2017-12-30T23:21:26.969Z Reads: 132

```
Ok, thank you @mmaner!

@scepterr thats 1000 mA so it sound like it might be enough. I'll have to try I guess and see, haha.
```

---
## \#5 Posted by: scepterr Posted at: 2017-12-30T23:22:05.351Z Reads: 130

```
Lol no not how many mA is 1A LMAO
How many mA are your power requirements?

I can't remember exactly, the draw of the vesc itself is like 200-300mA?
```

---
## \#6 Posted by: Fiori Posted at: 2017-12-30T23:26:48.420Z Reads: 121

```
Seems you might need to step up the voltage. <img src="/uploads/db1493/original/3X/2/6/26b3ea16b5b8c54e9e0cf71caa152296dfa07240.png" width="690" height="80">
```

---
## \#7 Posted by: evoheyax Posted at: 2017-12-30T23:29:20.129Z Reads: 116

```
oh, haha. I'm not quite sure yet. It seems like the aurdino is about 200 mah, not sure about everything else.

Working on what I think could be the real solution for good headlights, brake lights, and tail lights, combined with multiple vesc bluetooth.

With the Mega, I can have up to 4 serial connections, so 4wd or 2wd could have data combined for sending to your smart phone.

Also will be integrated with an oled display to put on top of your board to give on board data.

Really, I would like to think of it as the central computer of the board. The vesc's control the motors still, but all data is passed to this central computer so we can use it for lights, displaying, and to combine data between vesc's to be sent to your smart phone.
```

---
## \#8 Posted by: scepterr Posted at: 2017-12-30T23:32:15.832Z Reads: 105

```
Don't you get access to all vescs via can if using Bluetooth only on master?
```

---
## \#9 Posted by: evoheyax Posted at: 2017-12-30T23:36:10.926Z Reads: 106

```
No, you only get data from the master vesc then. So if your using it on a 2wd or 4wd, your only getting data from 1 vesc.

If you check out the firmware code, specifically the commands.c file, you'll see that there is no way setup already to share data between the vesc's, beside erpm, which is used for traction control.

No one has yet to create a system that conbines all of the data together. You can "guess" you'll see the same current between the motors, but again, that's a guess. You won't get accurate numbers, and this is what some of the phone apps offer.
```

---
## \#10 Posted by: saul Posted at: 2017-12-30T23:54:10.468Z Reads: 100

```
i've used around 500-800ma from the servo line 5v. 
not sure if theres a difference on the uart pinout.
```

---
## \#11 Posted by: Der6FingerJo Posted at: 2017-12-31T00:05:26.868Z Reads: 97

```
[quote="evoheyax, post:9, topic:42336"]
No one has yet to create a system that conbines all of the data together. You can "guess" you'll see the same current between the motors, but again, that's a guess. You won't get accurate numbers, and this is what some of the phone apps offer.
[/quote]

https://github.com/RollingGecko/VescUartControl/pull/9 

this could help with the multiple vescs thing, but i haven't tested it yet.

Also, why don't you use the +5V from the PWM Port? I always did that with my arduinos and it should deliver 1A for sure.
```

---
## \#12 Posted by: evoheyax Posted at: 2017-12-31T00:14:04.853Z Reads: 83

```
Thanks for the link, I'm trying to get that code working right now actually. Been getting this error though:

fatal error: arduino.h: No such file or directory.

I had the leds up and working in minutes, but this piece has been a bit more difficult since I couldn't just install it like a library and have it work...

The reason for using the uart for power is because it'll mean less plugs. Trying to create a box essentially that has a bunch of ports for you to plug everything into. So master vesc + slave vescs each will have their own uart in port (master would then power the whole systems), then a front led port, back light port, and oled display port.
```

---
## \#13 Posted by: faithfulpuppy Posted at: 2017-12-31T01:02:20.622Z Reads: 76

```
>The vesc's control the motors still, but all data is passed to this central computer

Like a multirotor! Good thinking! This project has a lot of potential and im interested in seeing where it goes.
```

---
## \#14 Posted by: evoheyax Posted at: 2017-12-31T01:10:43.881Z Reads: 71

```
Thank you, good catch!
```

---
## \#15 Posted by: evoheyax Posted at: 2017-12-31T01:13:13.786Z Reads: 75

```
Just to show the lights, super easy to setup...

https://youtu.be/_PJtapzA2e4
```

---
## \#16 Posted by: GrecoMan Posted at: 2017-12-31T01:18:26.913Z Reads: 73

```
i really gotta figure out some way to split the uart port 3 ways...

wanna run bluetooth module
wanna use the firefly remote
wanna use some turn signals

decisions decisions
```

---
## \#17 Posted by: evoheyax Posted at: 2017-12-31T01:31:23.965Z Reads: 71

```
Well the Arduino Mega has 4 sets of serial input and ouput.

Mix this with some led lights, and the right controller, and there you go :P
```

---
## \#18 Posted by: GrecoMan Posted at: 2017-12-31T01:32:29.619Z Reads: 69

```
where dju get these lights?
```

---
## \#19 Posted by: evoheyax Posted at: 2017-12-31T01:37:04.687Z Reads: 68

```
These are adafruit neopixel sticks. Bought on amazon for $10 each.
```

---
## \#20 Posted by: scepterr Posted at: 2017-12-31T01:43:39.662Z Reads: 71

```
More cost effective option
http://amzn.to/2ChxA0n
Neopixel is just branded ws2812b
Edit:fixed link
```

---
## \#21 Posted by: evoheyax Posted at: 2017-12-31T01:46:47.631Z Reads: 69

```
Not in the size I want though. I need these small pieces for integrating into the deck. I have 2 sample hollow core decks coming in within the next month hopefully, so I'm hoping to put these into the ends of the board :)
```

---
## \#22 Posted by: scepterr Posted at: 2017-12-31T01:51:57.030Z Reads: 68

```
You can cut them to size
```

---
## \#23 Posted by: laurnts Posted at: 2017-12-31T01:52:27.721Z Reads: 68

```
Just buy one of these and attach it to your battery. It's cheap and provide decent to power any sort of things on different voltages. https://hobbyking.com/nl_nl/yep-20a-hv-2-12s-sbec-w-selectable-voltage-output.html
```

---
## \#24 Posted by: Wajdi Posted at: 2017-12-31T02:30:34.619Z Reads: 64

```
I'm working on something similar :stuck_out_tongue: 
It will be a central control station, and accepts the Photon receiver as an Add-on.
```

---
## \#25 Posted by: evoheyax Posted at: 2017-12-31T02:57:16.011Z Reads: 62

```
Well sounds like eskate is evolving :) glad to hear I’m not the only one with this idea :)
```

---
## \#26 Posted by: Der6FingerJo Posted at: 2017-12-31T12:43:59.398Z Reads: 58

```
[quote="evoheyax, post:12, topic:42336"]
fatal error: arduino.h: No such file or directory.
[/quote]

Sounds like some kind of library error, man i hate that with Arduino. Sometimes it helps to start from scratch using the example sketch provided by the library. 


I'm currently working on a nrf and Gt2B based OLED remote and settled for using only one VESC as is want to keep the receiver as small as possible. Since each VESC receives the same PWM Signal it should be fairly accurate to just count the relevant stats double.
```

---
## \#27 Posted by: evoheyax Posted at: 2017-12-31T16:16:45.946Z Reads: 53

```
If the motors are the same kv, then yes. But if the motors kvs are slightly different, you will pull different amounts of amps, and most are. Getting the same kv on the dot requires accuracy that most motor manufacturers can't replicate.

For example, they say a motor is 180 kv. The first could be 178 kv, the second might be 183 kv. 5 kv is enough to throw your numbers off a fair amount, especially if your drawing high amps or running higher kv motors.
```

---
## \#28 Posted by: evoheyax Posted at: 2017-12-31T16:29:37.032Z Reads: 49

```
Thank you for the idea, I will try that. THe whole reason though I was trying to stay away from something like that is becuase I wanted to keep things simple for end users to install.
```

---
## \#29 Posted by: Der6FingerJo Posted at: 2017-12-31T17:39:42.273Z Reads: 45

```
Correct me if I'm wrong, but the Vesc controls by current and not by voltage. You set the current the Vesc is supposed to put out so it shouldn't matter that much.
```

---
## \#30 Posted by: evoheyax Posted at: 2017-12-31T19:41:07.402Z Reads: 46

```
I have put 2 different kv motors side by side with 2 different computer hooked up to them, and seen a difference in amp draw. Maybe this is due to watt control mode, but I don't think its that safe of an assumption. If you use a higher kv motor, you'll need more amps to get the same torque at the same voltage.

Even if they were to be exactly the same, it would help for trouble shooting to see the data coming from each vesc. The fault codes, and other data is still useful.
```

---
