# Has anyone figured out how to make Smart Turn On work on a custom esk8?

### Replies: 21 Views: 1285

## \#1 Posted by: EverBlade21 Posted at: 2018-05-21T00:31:20.155Z Reads: 256

```
As the title said just wondering if someone was able to make this a thing, alot of offiicial esk8s have it but I'm curious if the DIY community can replicate it. Smart Turn On basically means you can turn on your remote and go, but correct me if I'm wrong
```

---
## \#2 Posted by: Kug3lis Posted at: 2018-05-21T00:36:28.066Z Reads: 256

```
Basically your board is always on ;)
```

---
## \#3 Posted by: Jc06505n Posted at: 2018-05-21T00:45:40.478Z Reads: 247

```
I don’t know any pre-builds that have this ability. Maybe you’re thinking of Push to start?
```

---
## \#4 Posted by: EverBlade21 Posted at: 2018-05-21T00:55:01.053Z Reads: 240

```
Maybe? I'm pretty sure the raptor 2 has it? or the mellow board?
```

---
## \#5 Posted by: sunnyD Posted at: 2018-05-21T01:27:14.219Z Reads: 225

```
Correct me if I’m wrong, But you are referring to the remote turning on both the controller and Eboard. I think a push to start is a good alternative for this as I have not seen and “smart” turn on features.
```

---
## \#6 Posted by: Jc06505n Posted at: 2018-05-21T01:39:18.214Z Reads: 208

```
Well @onloop would know , but it would be a feature that all Focboxes have. Mellow requires push to use similar to unsensored Drives. 


But no , lie @Kug3lis said , that would require you to always have your Board on, similar to how the Xbox One and PS4 are always on. and that’s not practical for boards like these. 

A better implementation are push to start that DIYEboards ESC’s have 

As well as the ability to shut off the board via remote like the Boosted V2 has.
```

---
## \#7 Posted by: EverBlade21 Posted at: 2018-05-21T03:13:21.811Z Reads: 175

```
Thank you so much, that makes a lot of sense and I appreciate you explaining that. Personally I couldn't care less about a feature like that because for me its not that hard to bend over and plug in an xt90 or push a power button. But I'm looking to selling my boards to friends and people ik and I've seen that people really love this feature in pre-builts. Thanks again and anyway we can make our DIY esk8s better or on par with pre-builts I'm curious.
```

---
## \#8 Posted by: Quezacotl Posted at: 2018-05-21T06:13:12.015Z Reads: 159

```
I have left my board turned on for couple of days accidentally, few times, and while i have measured the voltage, it has practically drained nothing.
So i think leaving the board in always on doesn't matter if you are using it often. So that concludes that the smart-on could be mostly useless feature.
Better would be smart-off :D
```

---
## \#9 Posted by: Mikenopolis Posted at: 2018-05-21T06:24:06.905Z Reads: 154

```
Smart turn on is on Meepo and InBoard M1

On a Meepo. You can turn off the board but if you roll the wheels the board will wake up (I’m pretty sure that’s how it works)

The InBoard M1 USED to be on ALL THE TIME. you’d turn on the remote and the board will connect and be ready to ride. There’s no on/off button on that board. Problem with that is the board is constantly searching for the Bluetooth connection and on Monday I would have a dead board after a weekend of not using the board. I advised them of Meepo’s use of wheels to turn the board on and InBoard’s recent update added that feature. It no longer looks for the BT connection unless a wheel is turned. Now I lose 20% battery over the weekend instead of 90% like before.  

TL;DR you will lose battery life having this feature
```

---
## \#10 Posted by: L3chef Posted at: 2018-05-21T06:30:59.007Z Reads: 142

```
[quote="Mikenopolis, post:9, topic:56134"]
You turn off the board but if you roll the wheels the word will make up
[/quote]

Sry my finglish doesn't understand this sentence. Word will make up?

Whelp
```

---
## \#11 Posted by: Mikenopolis Posted at: 2018-05-21T06:36:14.735Z Reads: 132

```
Oops. Cellphone auto correct. BOARD. WAKE
```

---
## \#12 Posted by: L3chef Posted at: 2018-05-21T06:42:01.516Z Reads: 126

```
Ah well that makes sense :grinning:
```

---
## \#13 Posted by: Maxid Posted at: 2018-05-21T06:54:45.944Z Reads: 127

```
http://www.electric-skateboard.builders/t/why-is-there-no-on-off-switch-integrated-in-a-vesc/55753

Sleep mode with a switch could work but the VESC does not support it. Having push to start would require even more work. But yeah: this feature would be nice to have
```

---
## \#14 Posted by: Quezacotl Posted at: 2018-05-21T12:02:55.134Z Reads: 111

```
Hmm.. accelerometer with Arduino or something, connected to sparkswitch input, with adjustable on- and off-delay. Shouldn't be hard to make, even with my bad coding skills.
```

---
## \#15 Posted by: Jc06505n Posted at: 2018-05-21T13:18:05.057Z Reads: 102

```
Would you even need all that? Dosen't ESC's receive small power when you run the wheels? (I could be wrong) Just have software that utilizes a condition where if Powered, turn on.
```

---
## \#16 Posted by: drassak Posted at: 2018-05-21T13:24:19.155Z Reads: 100

```
Killed 2 battery packs because of this, the vesc and receiver drain the battery due to their LED mostly. if you leave your board turned on for a week with a 30% full battery you'll find it dead drained.
```

---
## \#17 Posted by: Quezacotl Posted at: 2018-05-21T13:43:04.453Z Reads: 92

```
True, but like drassak said, the VESC LEDs and receiver drain the battery too quick, so the function can't be within VESC.
```

---
## \#18 Posted by: Acido Posted at: 2018-05-21T14:20:56.278Z Reads: 84

```
use a turnigy remote on off switch and wire it on a bms e switch
so turn on your remote, send a signal with ch2 or whatever the switch uses, the switch then closes the circuit, and when its closed bms sends power to the vescs and motors
its not so complicated and people have done it
```

---
## \#19 Posted by: EverBlade21 Posted at: 2018-05-22T02:37:42.818Z Reads: 63

```
so this so far seems like it makes the most sense and seems super convenient, but can someone explain how the power switch would even work in this case? I mean there is no shot that one of these little guys can be connected directly on the power line right?
```

---
## \#20 Posted by: Acido Posted at: 2018-05-22T09:34:19.165Z Reads: 52

```
They are not connected to main wires
They are connected to a bms
```

---
## \#21 Posted by: sebaszz Posted at: 2018-05-22T10:27:20.932Z Reads: 39

```
If you store your board vertically , you can use some kind of reed switch (with a timer delay for non flat surface during your ride). Putting your board onto the ground it energize itself. As a backup for longer storage period use a simple XT90 disconnecting switch in serie.
```

---
