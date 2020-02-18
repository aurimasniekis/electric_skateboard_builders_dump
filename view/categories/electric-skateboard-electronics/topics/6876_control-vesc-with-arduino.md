# Control VESC with arduino

### Replies: 26 Views: 13742

## \#1 Posted by: Workaround Posted at: 2016-07-30T23:41:04.406Z Reads: 555

```
I have not been able to find a full tutorial on how to take apart a regular wii nunchuck(not wireless) and use an arduino chip to control a vesc.
```

---
## \#2 Posted by: Sir.Mighty Posted at: 2016-07-31T00:18:20.694Z Reads: 554

```
I was working on something similar, until my Drv chip decided to break.
I used UART to communicate between the rx arduino and the VESC using this library: https://github.com/RollingGecko/VescUartControl
Connecting it is simple, arduino rx to vesc tx and vice versa and selecting uart as the control mode on the VESC.

Especially look for the nunchuck part. Pm me if you need help with it.
```

---
## \#3 Posted by: Workaround Posted at: 2016-07-31T01:03:20.833Z Reads: 531

```
First I have not received my VESC yet it should be shipping out this week. So I can't test anything. But to clear up what I want to do is hookup HM-10 or NRF24L01+(I have more of these laying around) to communicate to the VESC. I need one for the vesc end and one for arduino side I'm thinking.

I can't find information on the data sent over from arduino to the VESC to get the motor to move. So I can make specific buttons do specific things.
```

---
## \#4 Posted by: zk8_builder Posted at: 2016-07-31T01:45:16.675Z Reads: 488

```
If you go on YouTube and search up great Scott electric longboard it is either part 2 or 3
```

---
## \#5 Posted by: Workaround Posted at: 2016-07-31T16:56:35.190Z Reads: 444

```
I want to use UART. Also Not a VESC he is using but I suppose it would not matter if I was using PWM(but his esc did not have breaks so I don't know if it would be the same). Something to note is that his code with the delay function can destroy your electronics cause the delay function stops sending signals which stops the motor from spinning then spins up faster then repeats this process of Stop and go fast.

Bit of a rant on why Great Scott's setup is incorrect. 

I'm not sure if I could find the data for reverse and brakes using the same methods he used.

I want to use UART so I could read data like speed and battery voltage from the VESC.
```

---
## \#6 Posted by: DougM Posted at: 2016-07-31T18:28:55.892Z Reads: 414

```
https://github.com/RollingGecko/VescUartControl

DougM
```

---
## \#7 Posted by: Workaround Posted at: 2016-07-31T18:30:29.743Z Reads: 390

```
That is the same link. It is the communication library not protocol
```

---
## \#8 Posted by: cjoliver Posted at: 2016-07-31T18:44:37.943Z Reads: 387

```
Please take time to look at what the community gives you, this link https://github.com/RollingGecko/ArduBoardControler
was in the links given to you above and seems to be what you're looking for
```

---
## \#9 Posted by: Workaround Posted at: 2016-07-31T19:12:19.003Z Reads: 377

```
I have read most of these links before starting my question. I'm still having problems understanding everything. It is not that I'm ignoring peoples help.
```

---
## \#10 Posted by: cjoliver Posted at: 2016-07-31T19:13:43.616Z Reads: 383

```
receiving arduino
https://github.com/RollingGecko/ArduBoardControler/blob/master/ArduBoardControler_Rx/ArduBoardControler_Rx.ino

controller arduino 
https://github.com/RollingGecko/ArduBoardControler/blob/master/ArduBoardControler_TX/ArduBoardControler_Tx.ino
```

---
## \#11 Posted by: Jeefberky Posted at: 2016-07-31T20:18:54.810Z Reads: 343

```
I have just created my contoller using the sketch and libraries from RollingGecko. He has a wiki page on his github on how to set it up https://github.com/RollingGecko/ArduBoardControler/wiki.

I have used a cheap chinese nunchuck and stripped most of the guts out of it. I only used the thumbstick-potmeter and the circuitboard for the c and z button.
I have placed an arduino nano in it and connected the potmeter and buttons to it. To power the arduino I used a 1s lipo with a power cell board from sparkfun.

I also want to use leds to know the battery level of the esk8, remote and connection status because RolingGecko added this functionality to his sketch.

It takes some patience<img src="/uploads/db1493/original/2X/0/0320589f06493768f9d290b84f9ce5cf10bcbfc4.PNG" width="690" height="328">

You could also send a ppm signal to the vesc with almost the same setup. But using the setup as shown above, gives you the ability to use the features as if you connect a Nyko Kama nunchuck to the vesc (Cruise control, switching motor directions and some telemetry features added by RollingGecko).
```

---
## \#12 Posted by: Workaround Posted at: 2016-07-31T22:33:20.331Z Reads: 324

```
That is very helpful diagram. I really appreciate that. So now some questions.

1. VESC side arduino is being powered by the VESC?
2. Controller side why do you have two potentiometers?(what are you using them for)
3. Do you have any code you used on the arduinos that I could use?
```

---
## \#13 Posted by: cjoliver Posted at: 2016-07-31T23:13:55.928Z Reads: 311

```
Is there an issue with code above?
```

---
## \#14 Posted by: Jeefberky Posted at: 2016-08-01T12:12:30.049Z Reads: 306

```
1. Yes
2. Those potmeters are the potmeters of the thumbstick. X and Y axis. I only use the Y axis for throttle control.
3. I used the code @cjoliver gave you.
```

---
## \#15 Posted by: Workaround Posted at: 2016-08-01T16:46:54.946Z Reads: 297

```
That code is probably what I to use for starting. I might be confused because I don't have my vesc yet to test things with.
```

---
## \#16 Posted by: Workaround Posted at: 2016-08-05T02:49:46.376Z Reads: 277

```
I should be getting my VESC by the end of the week. So I will make a new thread on a simple how to and add a link on this thread onces I have made that.
```

---
## \#17 Posted by: Workaround Posted at: 2016-08-13T01:28:44.467Z Reads: 264

```
How did you figure that was the correct wiring for everything. I have an Uno's that I'm making PCB boards for so I don't want to screw this up.
```

---
## \#18 Posted by: boards Posted at: 2016-08-13T02:51:22.326Z Reads: 252

```
I highly recommend connecting the VESC directly to a rf24 module, less room for fuck ups that way.
```

---
## \#19 Posted by: Workaround Posted at: 2016-08-13T12:27:10.620Z Reads: 252

```
I'm interested in Wiring to VESC like which pins are for what. It looks like in the code pins for potentiometer and buttons are not set. I have some NRF 24L01+ but have never used them so I'm new to how to wire them.
```

---
## \#20 Posted by: Jeefberky Posted at: 2016-08-13T18:36:59.805Z Reads: 250

```
@Workaround 
I think you are missing the config.h

In the config.h are al the connections listed. You can find the config.h for tx and rx here:
https://github.com/RollingGecko/ArduBoardControler/wiki/How-to-set-up-ArduBoardControl 
under the title, Pin settings, on the given URL.

I do not really know how the code exactly works but I know it mymics a nyko kama nunchuck ( I do not know this completely sure, but it looks like the controlls and behaviour are the same) and that it works flawless for me.
```

---
## \#21 Posted by: Workaround Posted at: 2016-08-13T18:53:16.693Z Reads: 239

```
I'm wondering about the buttons and potentiometers are not defined.
```

---
## \#22 Posted by: Workaround Posted at: 2016-08-14T01:24:22.996Z Reads: 235

```
@Jeefberky I figured out how the pins work. I must have missed that when looking at that link.
```

---
## \#23 Posted by: RollingGecko Posted at: 2016-10-03T22:51:54.476Z Reads: 212

```
Hi,

I'm happy to see that some people already started to realize my design. As I can see there are questions popping up. It could be much easier to canalize the questions and discussion to Endless-Sphere thread: [Endless Sphere](https://endless-sphere.com/forums/viewtopic.php?f=35&t=73812)

It would also be great you support me with the creation of a how to on the wiki page: [Wiki-Page](https://github.com/RollingGecko/ArduBoardControler/wiki/How-to-set-up-ArduBoardControl) So feel free to add the stuff or to send me the stuff so that I can add it.

@Jeefberky: It would be great if I could use your diagram! Something is missing here on the TX site. I use a voltage divider to measure the input voltage and to have a voltage alert for the TX.
```

---
## \#24 Posted by: Jeefberky Posted at: 2016-10-04T06:31:54.461Z Reads: 204

```
I send you a PM on Endless Sphere with the diagram. Keep up the good work!!
```

---
## \#25 Posted by: Wentworth Posted at: 2018-07-05T01:49:05.090Z Reads: 76

```
What is the role of the "Z" key and the "C" key? Cruising and reversing?
```

---
## \#26 Posted by: Kal-El_basically Posted at: 2018-10-31T18:59:21.060Z Reads: 46

```
Hey, im new to VESCs and I was wondering if you could use an arduino to wirelessly control a vesc with an IOS app called Blynk. Basically if Blynk can control Arduinos, and Arduino's can control VESCs, then cant Blynk be used as nunchuck substitution i guess. This is for a proof of concept like project so if anybody could help that would be great.
```

---
