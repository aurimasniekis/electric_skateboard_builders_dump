# Fried my ESC, need help upgrading

### Replies: 25 Views: 669

## \#1 Posted by: Skatejitsu Posted at: 2019-03-12T19:31:09.786Z Reads: 123

```
Over the past year, I built a 10s8p battery and custom enclosure for my Evolve Bamboo GT.  I've been running Racestar 140Kv motors ever since one of my original Evolve motors died, even prior to the upgrade.

Everything's been running solid until today, when my board came to a halt and smelled like burnt electronics.  

I opened up the board and there's an obvious burn mark where one of the motor's yellow wires attach to the board.  I'm assuming this ESC is toast at this point (?).

1 - Did I do anything, or is there anything I should check that would have caused this?  Or is it simply the stress of running a hilly trail?  Did the motor just stress too much and it ended up killing the board?   I have proper voltage coming from my battery still.

2 - If this thing is toast, I'd rather upgrade than swap out with stock Evolve stuff.  Since I have this mega 10s8p battery, what could I buy in order to run 200Kv motors?  Can I keep the evolve BMS that is currently in the board and just buy a new ESC, or do I need ESC and a new BMS?  I'm assuming new ESC means new remote too, or is there something that works with my R1 Evolve remote?

![fried-esc|690x461](upload://6FGQz8Mkqqz4tUKuIRNXEwak0Cz.jpeg)
```

---
## \#2 Posted by: ZachTetra Posted at: 2019-03-12T19:43:07.567Z Reads: 110

```
I mean there's at least 4 Unitiy's brand new for sale rn
```

---
## \#3 Posted by: Skatejitsu Posted at: 2019-03-12T19:48:52.589Z Reads: 106

```
Sorry for my ignorance, I don't follow this forum closely enough to know... where would I go to buy one of these 4?
```

---
## \#4 Posted by: ZachTetra Posted at: 2019-03-12T19:51:03.791Z Reads: 105

```
This should show all of the ones currently still available

https://www.electric-skateboard.builders/search?q=unity%20category%3A17%20order%3Alatest_topic
```

---
## \#5 Posted by: Skatejitsu Posted at: 2019-03-12T19:54:23.433Z Reads: 103

```
Oh gotcha, thanks.  So if I get a Unity ESC, can I keep using the original Evolve BMS?  And does that Unity talk to an Evolve remote, or do I need to replace that?
```

---
## \#6 Posted by: ZachTetra Posted at: 2019-03-12T19:56:54.520Z Reads: 97

```
You should be able to use the stock BMS as long as it has the same connector as the Unity, I believe the Evolve remote pairs to the ESC directly so you'll need an aftermarket remote/receiver pair
```

---
## \#7 Posted by: Skatejitsu Posted at: 2019-03-12T19:57:20.891Z Reads: 93

```
Ok thanks!
```

---
## \#8 Posted by: ZachTetra Posted at: 2019-03-12T20:00:37.996Z Reads: 86

```
Are you able to pay $350ish for the Unity rn?  They're $280 new from Enertion but it'll be mid May when they ship out
```

---
## \#9 Posted by: ZachTetra Posted at: 2019-03-12T20:03:26.651Z Reads: 84

```
This guy is selling a new Unity and a decent remote, he said he had a pending sale Friday but never updated, it's a bundle with a battery rn but he may separate them again

https://www.electric-skateboard.builders/t/12s3p-unity-and-remote-bundle/86357
```

---
## \#10 Posted by: Skatejitsu Posted at: 2019-03-12T20:04:40.387Z Reads: 81

```
yeah, price is fine.  I just messaged one of the guys that has one for $350.  I'd rather pay the premium and have it sooner than later.
```

---
## \#11 Posted by: Octave Posted at: 2019-03-12T20:05:17.967Z Reads: 79

```
Before you go buying a new vesc why not try solder on the yellow lead properly its half hanging of the pad. It doesn't look like components are damaged.
```

---
## \#12 Posted by: Skatejitsu Posted at: 2019-03-12T20:06:21.700Z Reads: 77

```
Stupid question, but is this one of those things that "just happens"?  I assume that burn mark where the yellow wire connected to my old board just means it tried to draw too much current?  Or is it more likely a fault in that motor that caused this?
```

---
## \#13 Posted by: Sn4pz Posted at: 2019-03-12T20:07:40.775Z Reads: 70

```
I was under the impression the evolve BMS is extremely restrictive.... I don think you can use it with the Unity, ESP cuz you cant use the remote :thinking:
```

---
## \#14 Posted by: Skatejitsu Posted at: 2019-03-12T20:12:35.712Z Reads: 69

```
I was wondering about that. It is still attached to the pad but not by much. I'll throw some solder on and see what I get.  There is a component near it that looks like it could be damaged but it's hard to say for sure.
```

---
## \#15 Posted by: ZachTetra Posted at: 2019-03-12T20:13:57.143Z Reads: 64

```
Is the BMS connected to the ESC?
```

---
## \#16 Posted by: Sn4pz Posted at: 2019-03-12T20:16:35.250Z Reads: 65

```
well from the BMS would be the power connecter to the ESC, Im just going off of previous knowledge where people have done ESC swaps and they ditch the whole evolve ecosystem
```

---
## \#17 Posted by: ZachTetra Posted at: 2019-03-12T20:19:14.129Z Reads: 66

```
If the BMS only has the power leads, the leads can be replaced with the XT60 male that match the Unity and all is good

If the BMS has data wires that go to the ESC then the BMS has to go too...if the cells are li ion then the cells can be kept but you'll need pigtails to connect them to the new BMS...you could keep the ports and charger if you know the BMS can handle it
```

---
## \#18 Posted by: Octave Posted at: 2019-03-12T20:23:02.925Z Reads: 69

```
Evolve don't like when you try to upgrade your board
https://www.electric-skateboard.builders/t/im-an-outlaw-burn-noticed-a-fugitive-from-a-facebook-group/35452
```

---
## \#19 Posted by: Skatejitsu Posted at: 2019-03-12T20:56:54.533Z Reads: 64

```
Well I soldered that yellow wire back on solid but something is definitely screwy still.  The power switch doesn't work at all.  Not sure if something in the switch itself is messed up or the ESC, but the positive that should be dead when the switch is in the off position is constantly hot.
```

---
## \#20 Posted by: Skatejitsu Posted at: 2019-03-12T22:01:53.022Z Reads: 60

```
What BMS should I get to replace the Evolve one if I do buy a Unity?  There are UART wires that go from the Evolve BMS to the ESC so I guess I have to replace that too.
```

---
## \#21 Posted by: Sn4pz Posted at: 2019-03-12T22:08:30.125Z Reads: 55

```
You can use any BMS, as thats where evolves 'electronic coupling' starts.

All BMSs require the pos and neg from the battery, as well as the balance wires. You can order a BESTECH bms from @JLabs (remember to choose the correct one (there is one for 12s and one for 10s) ) which wont have any UART port. 

Once you connect the power from the BMS to the ESC, granted everything evolve is removed, you can use any BMS, ESC or remote youd like... as long as they work with the hardware you choose :)
```

---
## \#22 Posted by: Kram720 Posted at: 2019-05-20T09:58:55.464Z Reads: 39

```
I had similar happen, my wire fell of.
Under load it got hot the solder melted.
Luckily for me I just soldered it back on and all was good
```

---
## \#23 Posted by: Kram720 Posted at: 2019-05-20T10:05:18.523Z Reads: 40

```
Going to do the same battery config 
But put a fan on the motor controller to keep it cool, at the moment I run 200kv motors which is why I melted the solder connection.  I was doing a pretty gnarly single track hill climb. Stupid me. 
Was thinking about upgrading the fets on the Mc
```

---
## \#24 Posted by: PixelatedPolyeurthan Posted at: 2019-12-10T19:43:50.413Z Reads: 21

```
Wow, if only i had read this before... Same thing happend to me. The yellow wire unsoldered itself and then my board would not turn on but the esc would get hot on one particular point when the power switch was turned on (no blue light came on though).
The lesson is to resolder all the joints with proper solder and flux.
```

---
## \#25 Posted by: PixelatedPolyeurthan Posted at: 2019-12-11T09:26:26.688Z Reads: 16

```
Did you get sorted out in the end @Skatejitsu?
```

---
