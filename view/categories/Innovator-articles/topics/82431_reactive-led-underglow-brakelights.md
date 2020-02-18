# Reactive LED Underglow Brakelights!

### Replies: 28 Views: 1051

## \#1 Posted by: cubed Posted at: 2019-01-29T00:39:13.324Z Reads: 274

```
https://d3rd3i2xz0wkmj.cloudfront.net/f6/60/vid--441683542-e325f610-6ed8-4ab9-87cf-5660e4a9d7f3-640x360.mp4

Just saw this on reddit and thought I would share (with permission of the creator). Go check out the full guide on https://www.mcduffchannel.com/441683542

Anybody know how to make this work with a focbox?
```

---
## \#2 Posted by: ZachTetra Posted at: 2019-01-29T01:42:12.876Z Reads: 258

```
Send a message to whoever makes/distributes the focbox and ask for a circuit map of the focbox so you can isolate the 2 resistor ends that carry the speed/brake signals and solder to them instead, everything else is the same

Alternative is to get a multi meter and poke every resistor you see and measure the voltage when you accelerate and brake
```

---
## \#3 Posted by: devilzangelz Posted at: 2019-01-29T01:57:14.879Z Reads: 240

```
Second approach seems like a great way to fry a DRV chip... 

Please be careful!
```

---
## \#4 Posted by: ZachTetra Posted at: 2019-01-29T01:58:27.026Z Reads: 238

```
A multi meter will not cause a short if you don't connect anything high voltage

But make sure you don't touch 2 adjacent points with the tip
```

---
## \#5 Posted by: Pedrodemio Posted at: 2019-01-29T03:00:23.099Z Reads: 220

```
Safer and guaranteed to work is to connect and arduino to the UART port and them you can do whatever you want

Make it speed based, make the color change based on how much power you are using, endless possibilities
```

---
## \#6 Posted by: b264 Posted at: 2019-01-29T03:05:37.051Z Reads: 217

```
The FOCBOX is a version of the VESC circuit and it's digital, not analog.  No such resistor exists.

https://github.com/b264/bldc-hardware/blob/master/design/BLDC_4.pdf
```

---
## \#7 Posted by: ZachTetra Posted at: 2019-01-29T03:07:11.896Z Reads: 210

```
Are the Meepo ESCs analog?  I though they had those resistors
```

---
## \#8 Posted by: b264 Posted at: 2019-01-29T04:30:01.046Z Reads: 201

```
Probably not, but I'm not really sure as I've never used one or seen one.

The output is certainly digital, and I can't imagine the radio control being analog.  Not sure what kind of gate driver system they use, but it's highly unlikely.
```

---
## \#9 Posted by: sofu Posted at: 2019-01-29T04:59:52.770Z Reads: 193

```
Or you could get a module that specifically reads ppm data to manage lights, or you can put a small arduino to do the same thing... 

Something like this https://hobbyking.com/en_us/quadcopter-tri-color-speed-lighting-system-1-set.html
```

---
## \#10 Posted by: cubed Posted at: 2019-01-29T06:03:29.575Z Reads: 184

```
Would this just plug into the focbox directly? Or would some rewiring to a new connector need to be done.
```

---
## \#11 Posted by: sofu Posted at: 2019-01-29T06:15:06.431Z Reads: 173

```
You will need a Buck converter and to split the ppm cable so it also runs to the pcb
```

---
## \#13 Posted by: Winfly Posted at: 2019-01-29T07:08:09.158Z Reads: 167

```
if I were to do it, I would just take signal from PPM.
```

---
## \#14 Posted by: linsus Posted at: 2019-01-29T12:10:26.421Z Reads: 149

```
Just use an empty I/O on the STM32 on the VESC, set it to output when brake happens -> make a PCB that reads that signal and controls a LED, done. Repeat for turn signals for "left" and "right" (if you are more pro and have a nun-chuck obv,)

Bonus advanced:  add a button to nunchuck to toggle headlight.
```

---
## \#15 Posted by: b264 Posted at: 2019-01-29T14:55:53.205Z Reads: 138

```
[quote="sofu, post:11, topic:82431, full:true"]
You will need a Buck converter and to split the ppm cable so it also runs to the pcb
[/quote]

Or just use a separate receiver so it's not connected to the drivetrain.
```

---
## \#16 Posted by: b264 Posted at: 2019-01-29T14:57:31.096Z Reads: 139

```
That'd be great except accessing those extra empty I/O are nigh impossible.  Unless you want to remake the entire PCB.
```

---
## \#17 Posted by: linsus Posted at: 2019-01-29T14:58:40.446Z Reads: 138

```
your soldering skills needs improvement young padawan, but yes. Remaking the PCB would be ideal
```

---
## \#18 Posted by: sofu Posted at: 2019-01-29T16:09:16.992Z Reads: 137

```
Wait where else would you get ppm braking data if not from your original receiver?
```

---
## \#19 Posted by: b264 Posted at: 2019-01-29T16:10:23.404Z Reads: 135

```
From a second receiver paired to the same remote.
```

---
## \#20 Posted by: sofu Posted at: 2019-01-29T16:11:22.360Z Reads: 132

```
Which remote lets you pair two receivers at the same time?
```

---
## \#21 Posted by: Mich21050 Posted at: 2019-01-29T16:12:03.994Z Reads: 133

```
Gt2b, Mini Remote for example :smile:
```

---
## \#22 Posted by: sofu Posted at: 2019-01-29T16:18:41.134Z Reads: 133

```
Wow I wasn’t aware gt2b let’s you do that! learn something new every day... Which mini remote are you referring to?
```

---
## \#23 Posted by: Mich21050 Posted at: 2019-01-29T16:19:54.610Z Reads: 131

```
The "classic" generic chinese one.
Edit:
https://buildkitboards.com/collections/remotes/products/mini-remote
```

---
## \#24 Posted by: ducktaperules Posted at: 2019-01-29T17:28:08.606Z Reads: 123

```
if you wanted the light effects linked to wheel speeds or breaking power applied then the https://github.com/SolidGeek/VescUart arduino library will allow this data to be read out of the spare uart on the FOCBOX.

Might be worth searching the forum cause i remember someone did a similar thing before and posted the instructions to build your own

EDIT: check this out https://www.electric-skateboard.builders/t/synchronized-lighting-for-vesc/44795
```

---
## \#25 Posted by: neiru37 Posted at: 2019-02-05T11:10:52.702Z Reads: 101

```
[quote="Winfly, post:13, topic:82431"]
I would just take signal from PPM.
[/quote]

Same

https://www.instagram.com/p/BtfX9T1jBP7ccMClBPHkP5ZsPOlyHbVSd9w1Ew0/?utm_source=ig_share_sheet&igshid=1novzn4k2q6ou
```

---
## \#26 Posted by: akhlut Posted at: 2019-02-05T16:13:55.709Z Reads: 82

```
This is good stuff.  I like my synchronized lights, but a brake light would be very nice to have.

I'm not sure about how much current the Unity can supply on that pin though.  A SBEC might be the way to go.

Something like this
https://www.amazon.com/GARTT-Model-Airplane-Programming-Required/dp/B06WV9HPKT

might be better to drive the LED's and arduino with.

Even better would be to have an independent receiver paired to the remote so it's not connected to the unity at all.  Either that or an opto-isolated splitter.
```

---
## \#27 Posted by: neiru37 Posted at: 2019-02-05T16:25:50.915Z Reads: 77

```
Yeah I thought of that so I lowered the brightness to 40 (out of 255) so it pulls less (mili)amps.
```

---
## \#28 Posted by: Dornacht Posted at: 2019-02-05T17:26:58.671Z Reads: 71

```
I am working on one slowly, I’m just doing what a bunch of diy electric bikers do and use an accelerometer and Arduino, so it isn’t connected to the vesc.
```

---
## \#29 Posted by: Bobby Posted at: 2019-02-06T10:58:17.278Z Reads: 61

```
Would you be able to give a quick drawing on how this is done?  Im very new to electronics and have no clue what buck converter to get and where to connect it to... the sote said it draws piwer from the balance leads but im using a li ion battery
```

---
