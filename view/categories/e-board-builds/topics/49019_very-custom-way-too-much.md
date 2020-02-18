# Very custom, way too much?

### Replies: 25 Views: 1564

## \#1 Posted by: Happylizzard Posted at: 2018-03-13T21:54:11.147Z Reads: 333

```
Greetings from Czech Republic!

I'm here with my first build and I must admit that I've started this "project" about a year ago, as you can see I've got basically nothing finished (not sure about what parts to order and how to mount it/slap it on the board).

Now I understand I need to do these things:

**Connect the motor with the weels** using a belt drivetrain, however I've got Rogue trucks which I've never seen on any build, is it even possible to create a drivetrain for them?
Now for the motor I was planning on using the [Axi V2], however the it's 305rpm/V which could be hard to gear down?
Has anyone done a drivetrain with a gear ratio this big?

Now I understand that I should **use a VESC** as it's specifically enginerded for electric longboards. The motor's max (60s burst) is 56A, does it _really_ mean 56A in the real world? Can VESC even handle that (different versions with different max A?).

I'll also have to get a **reciever** of some sort and origin, as I'm only sixteen I'm planning on not dying on my board asap :smile::cry:. What is the _most reliable connection between me and the VESC_??? I really wouldn't cheap out and just get some wii home-brewed reciever. Is the most reliable system the GT2B?

However the most problem I see with the **battery overall**, I have 12x A123 26650 cells (43.2V max) the motor's recommended voltage is 6-8S lipo (33.6V) what should I do? Does the VESC have a step-down voltage function? I really will need a reliable BMS for these cells but all BMSs I can find are really cheaped out looking boards, is there any way of stealing the boosted's BMS?

**Thank you so much for your time and effort** :pineapple:!

All best


 (https://www.modelmotors.cz/product/detail/276/) [_DSC5942|690x460](upload://maWRCEwcsWRk8uANqS8D9Mvwexe.JPG)![_DSC5943|690x460](upload://8fDYiqjmWFBQWs47IWCoxpbVAI7.JPG)![_DSC5941|690x460](upload://r0pvdZDTBpBIpSkvbiALXkkHc3z.JPG)![_DSC5945|690x460](upload://lmS7L1Yy3mM1NkU1PmIbWYFuWGC.JPG)![_DSC5939|690x460](upload://aFEyLxaEnbaRFAW8WMpulySIoWW.JPG)![_DSC5941|690x460](upload://r0pvdZDTBpBIpSkvbiALXkkHc3z.JPG)![_DSC5942|690x460](upload://maWRCEwcsWRk8uANqS8D9Mvwexe.JPG)![_DSC5939|690x460](upload://aFEyLxaEnbaRFAW8WMpulySIoWW.JPG)![_DSC5943|690x460](upload://8fDYiqjmWFBQWs47IWCoxpbVAI7.JPG)![_DSC5945|690x460](upload://lmS7L1Yy3mM1NkU1PmIbWYFuWGC.JPG)
```

---
## \#2 Posted by: TranxFu Posted at: 2018-03-13T22:08:02.438Z Reads: 301

```
You'll either need to change the motor or the batterys. Your motor KV is too high for your 12s voltage. It'll fry the vesc. Have a look at <200ish kv motors.

EDIT:

Most reliable remote -> GT2B. Yep, not the most compact but there are DIY mods for it. 
And no 60A burst is not the real-world application. It'll be around 5-15amps continuous when riding the board. Going uphill is a different story. 

There are good options for BMSs. No need to rip off the boosted board bms.


=>>> do more reading :)
```

---
## \#3 Posted by: bimmer Posted at: 2018-03-13T22:09:08.665Z Reads: 286

```
Nope you didn't read anything and just went out and bought stuff.

Your batteries will last 3 miles.

Your motor will fry a Vesc.

Your trucks need a custom mount.

You could do it all and go 6S at 100a discharge it could work but still... it will be more bad than good.
```

---
## \#4 Posted by: chuttney1 Posted at: 2018-03-14T00:04:47.963Z Reads: 235

```
My rebuttal to the two above comments about having a high KV motor. MoeStooge has this setup running well last time I read. As long you geared it correctly you cannot blow up the speed controller. However, a 192kv motor is fine.



http://www.electric-skateboard.builders/t/inner-gear-direct-drive-gearbox/44512/81?u=chuttney1
```

---
## \#5 Posted by: bimmer Posted at: 2018-03-14T00:13:13.028Z Reads: 216

```
Gearing has absolutely nothing to do with blowing the speed controller.
The vesc 4.12 can handle 60.000 erpm devide by 7 pole pairs 8570 rpm.
At 40V his motor will do 13000 RPM and absolutely fry a normal old vesc.
```

---
## \#6 Posted by: Cobber Posted at: 2018-03-14T00:23:41.152Z Reads: 214

```
I don't know anything about your motor but...

I'm doing 540kv 10P 12S at the moment 

the Stooges set up above is 850kv 4P 8S

my eRPM will be just under 120K

Only VESC 6 based hardware can handle the eRPM or go with a RC controller like Moe

many things are possible but not always practical
```

---
## \#7 Posted by: Deckoz Posted at: 2018-03-14T00:36:38.737Z Reads: 199

```
Or 28pole hub motors(torqueboard) vs 14 pole...will have double the erpm..
```

---
## \#8 Posted by: ARetardedPillow Posted at: 2018-03-14T02:12:55.785Z Reads: 188

```
Why would you pay 153 euro for that motor, for exactly how long have you been reading this forum
```

---
## \#9 Posted by: Schulerbible Posted at: 2018-03-14T02:32:29.029Z Reads: 186

```
"Why would you pay 153 euro for that motor" ..... where you could have spend your money on an APS 6384 outrunner (around 200 KV)!?
```

---
## \#10 Posted by: ARetardedPillow Posted at: 2018-03-14T03:36:02.698Z Reads: 184

```
Almost 2 APS 6374 motors lol
![image|443x251](upload://uc2bzeIxlPX3Bgginv70lz9O4oC.png)
![image|386x500](upload://nh6KfHMDjsmRncZeoykkUKPthWN.png)
I can't find the reasoning behind this
```

---
## \#11 Posted by: linsus Posted at: 2018-03-14T10:34:41.355Z Reads: 157

```
You can always change the KV of the motor..  can be done quite easily without rewinding the motor. Almost all outrunners are connected using a delta-connection. By removing the heatshrink of the motor wires, they can be split up and reconnected in a star-connection. This reduces the KV by a factor of sqrt(3) = 1.73.
```

---
## \#12 Posted by: Schulerbible Posted at: 2018-03-14T11:22:48.768Z Reads: 154

```
You mean this right?

![image|602x270](upload://j7YY1V5r3jPfQ3oSxtqlPWPdHYa.jpg)
```

---
## \#13 Posted by: linsus Posted at: 2018-03-14T12:16:52.173Z Reads: 141

```
That is a Delta and Star Connection, yes.
```

---
## \#14 Posted by: Happylizzard Posted at: 2018-03-14T14:26:02.544Z Reads: 133

```
Thank you very much for all the info I missed. I'm definitely going to read more about VESC and it's limitations (erpm). I'll take a look a look at the motor and it's limits (high rpm namely). For now I have to unfortunately finish some school work.
```

---
## \#15 Posted by: TarzanHBK Posted at: 2018-03-14T14:32:00.927Z Reads: 129

```
is there a tutorial about that somewhere i missed on youtube?
```

---
## \#16 Posted by: linsus Posted at: 2018-03-14T14:47:03.857Z Reads: 127

```
Might be, I'm an EE so i studies a few Courses on Electric Power and motors back in uni. 
The BLDC motor is essensially the same as a 3 phase AC motor. (without the commutator obv)
Read up abit on it if you're intrested, the actual wiring change shouldn't require much prestudy however. It's practically three terminals.
```

---
## \#17 Posted by: TarzanHBK Posted at: 2018-03-14T14:48:54.259Z Reads: 124

```
I searched for it, but all i found so far (not intensive searching ;) ) brings up to fully rewind a motor, not just rearranging leads
```

---
## \#18 Posted by: linsus Posted at: 2018-03-14T15:11:19.926Z Reads: 130

```
If you look at the Picture that some Bright guy posted above, you can see that wounds inside the motor is drawn as an inductors(the curly things). If you where to dissaseble your phase wires going out from the motor, they should consist of two strands of Cables if Delta wired. Leaving you with 3 pairs of strands when fully dissasembled. Now, using these 6 strands you connected them as a star configuration (right part of the Picture) and there u go, lower kv(by a factor of 1.73)
```

---
## \#19 Posted by: TarzanHBK Posted at: 2018-03-14T15:40:52.588Z Reads: 125

```
alright, cool thanks for this small tutorial, i´ll look into this a bit more soon :slight_smile:
```

---
## \#20 Posted by: Happylizzard Posted at: 2018-03-14T22:52:05.722Z Reads: 123

```
So If I want to keep this motor I'll have to rewire it to a star configuration.
If this reduces the KV by a factor of 1.73 does it increase the torque accordingly?

If I do this:
- motor's max recommended voltage is 8s lipo = 33.6V = 9.3 Lifepo cells 
If I used 9s (1p only - not enough cells) A123 26650 = 32.4V max
Motor - 305 rpm/V = 32.4*305 = 9882rpm (note however that the voltage drops almost immediately withe these cells = less rpm)
If the motor had 7 pole pairs (I'll ask the manufacturer)
than 9882rpm * 7 (let's assume) = 69174 erpm
If I rewire the motor it's 69174/1.73, right? = 40.000 erpm

Now the regaular VESC could handle this if I understand corretly
```

---
## \#21 Posted by: pennyboard Posted at: 2018-03-15T01:58:38.447Z Reads: 105

```
As far as I know @MoeStooge doesn't use VESCs. He had a different ESC last time I saw his board, if I remember correctly
```

---
## \#22 Posted by: MoeStooge Posted at: 2018-03-15T02:29:14.397Z Reads: 101

```
Been pleased with the Mamba XL-X. Has a very tunable tool box, data logging, adj amp ceiling, throttle/brake curve adj.. has no erpm limits and will feed 200a at 8s..
```

---
## \#23 Posted by: Cobber Posted at: 2018-03-15T02:42:58.376Z Reads: 103

```
[quote="MoeStooge, post:22, topic:49019"]
Been pleased with the Mamba XL-X
[/quote]

I might ;) have a extra pair laying around if anyone in Au wants a set, pm me.
```

---
## \#24 Posted by: pat.speed Posted at: 2018-03-15T04:59:17.161Z Reads: 98

```
Yes, you could actually use all the cells in a 12s setup, I doubt it will damage the motor. I run my 6s motor on 12s just fine
```

---
## \#25 Posted by: linsus Posted at: 2018-03-16T10:14:29.985Z Reads: 80

```
Think you have some reading to do on motors. :) Dont look for all short answers, try to understand as much as you can before doin something you're uncertain of.

http://vedder.se/2014/10/chosing-the-right-bldc-motor-and-battery-setup-for-an-electric-skateboard/  <-- pretty good read regarding kv, current and how its related.

Regarding pushing the voltage. 10S is prob fine on a 8S motor. But eventually it will saturate. Meaning it can't amplify the magnetic field in the motor any further. Thats a behaviour you'd generally want to avoid as its not good for the motor and wont give you a good riding experience (vibration and stuttering). So try load the motor under 10S and see if it saturates before riding as normal, falling under full load aint fun.
```

---
