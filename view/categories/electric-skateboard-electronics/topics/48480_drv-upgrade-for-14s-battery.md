# DRV upgrade for 14S battery

### Replies: 16 Views: 1317

## \#1 Posted by: Takis Posted at: 2018-03-08T10:14:03.822Z Reads: 201

```
Hi everyone , i have an old VESC (Maytech 4.12) which i will repair STM32F and VP232. I have my ebike running with 14s with stock controller at 25amps, i want to change the stock controller with the VESC so i can run over 25amps (40 i guess). The DRV8302 can work with 6-60V my battery 14s can go up to 58.8V (no regen from the motor). I have two questions , is there any upgrade i can do to the VESC ? and if its any way i can use over 60-70Volts on the VESC ,(I will add heatsinks in DRV STM32F and VP232 and on the FETs as well. Thanks
```

---
## \#2 Posted by: pat.speed Posted at: 2018-03-08T10:25:59.544Z Reads: 198

```
Don't think so otherwise we would be making them that way.
```

---
## \#3 Posted by: Takis Posted at: 2018-03-08T10:41:39.254Z Reads: 193

```
I had read that VESC 6 could handle 14s so i guess it can be done in the 4.12 as well ;)
```

---
## \#4 Posted by: Martinsp Posted at: 2018-03-08T10:44:38.081Z Reads: 187

```
Well, you could use it as it is, the absolute max of either DRV (02 or 01) is 65V but it would surely take a little bit of reliability away. Also, not sure how it could handle the voltage spikes, maybe if you dont use motor as an ebrake you might be fine.
Refference:
http://www.ti.com/lit/ds/symlink/drv8302.pdf
http://www.ti.com/lit/ds/symlink/drv8301.pdf
```

---
## \#5 Posted by: b264 Posted at: 2018-03-08T10:45:28.432Z Reads: 165

```
Hardware 6.4 still uses the DRV830x chip which still maxes at 60V.  That's a hard 60V and subject to manufacturing tolerances of up to 10%.  The motor windings also have back-EMF which adds voltage too.  I don't even recommend running the VESC hardware on 12S.  You definitely shoudn't push it past that and there is no chance it can do 14S.

There is [a project to raise the specs](http://www.fightingrobots.co.uk/threads/13621-300a-vesc-in-the-works-feature-suggestions-wanted) but these 16S 200A units cost £400
```

---
## \#6 Posted by: Takis Posted at: 2018-03-08T10:46:16.840Z Reads: 160

```
It wont have motor braking it has freewheel in many parts (its bottom bracket motor)
```

---
## \#7 Posted by: Vanarian Posted at: 2018-03-08T10:46:48.933Z Reads: 159

```
Ask Rogier Wolff from BitWizard / rew on Vedder's forum. He has built a LM5109 based VESC ; the chip itself is good up to 100v but the controllers are still geared for 60V.

@marcos on Vedder's forum has made big version with separate power board. No amp / village limit (like you can put it on a motorbike or a car) but not suited for a skateboard (massive sizes for IGTB).
```

---
## \#8 Posted by: Takis Posted at: 2018-03-08T11:29:23.027Z Reads: 148

```
Thats expensive as hell , i can buy a programmable  ESC with the half of its price from Alien Power system
```

---
## \#9 Posted by: Okami Posted at: 2018-03-08T15:10:56.625Z Reads: 126

```
I think focbox can "survive" 13s. I suspect 14s might be already too much, especially for somewhat "brittle" maytech esc.

E: consult @Deckoz he runs 13s on focbox, i think 

So yes, your only option might be the new vesc 6 alternatives (B box / Escape) or figuring out how to improve mosfets and other parts to reach higher voltage
```

---
## \#10 Posted by: Deckoz Posted at: 2018-03-08T15:21:32.314Z Reads: 115

```
Y'all are forgetting he's running an ebike

14s setup with current and no brakes is a standard config and easily done... On a focbox, or vesc6 derivative. 

It's the regenerative braking that makes 14s not possible for esk8 unless we have mechanical brakes like bikes.
```

---
## \#11 Posted by: Takis Posted at: 2018-03-08T15:23:41.262Z Reads: 113

```
Exaclty no regen braking thats where my hope is !
```

---
## \#12 Posted by: Takis Posted at: 2018-03-08T15:24:27.414Z Reads: 114

```
Anyway as soon as i get the parts and start that project i will keep you updated about it !
```

---
## \#13 Posted by: squishy654 Posted at: 2018-03-08T16:19:04.294Z Reads: 102

```
Would it be possible to remove this EMF on the phase wires? with some torroids and 7 wraps? I wonder if that fact can be negated..
```

---
## \#14 Posted by: Deckoz Posted at: 2018-03-08T16:58:34.106Z Reads: 95

```
EMF is needed for the ESC to keep synchronization with the motor so no...you cannot get rid of the BEMF.
```

---
## \#15 Posted by: Takis Posted at: 2018-03-08T17:48:44.947Z Reads: 84

```
it will be with hall sensor ;)
```

---
## \#16 Posted by: b264 Posted at: 2018-03-08T17:53:41.452Z Reads: 84

```
[quote="Okami, post:9, topic:48480"]
your only option might be the new vesc 6 alternatives (B box / Escape)
[/quote]

B-box and ESCape do not run higher voltages.
```

---
