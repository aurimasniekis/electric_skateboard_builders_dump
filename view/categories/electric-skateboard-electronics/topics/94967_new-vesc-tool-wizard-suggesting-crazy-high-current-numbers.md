# New VESC tool Wizard suggesting crazy high current numbers

### Replies: 22 Views: 641

## \#1 Posted by: Eboosted Posted at: 2019-05-25T22:45:46.183Z Reads: 172

```
I just downloaded the new VESC Tool from Vedder website.

https://www.vesc-project.com/vesc_tool

The new wizard asks now much more information than before and it's very intuitive however after runing it I get weird high current values suggested by the wizard itself.

Please take a look at them:

motor current max 67.73A
motor current max brake -63.73A
Battery current Max 99A
Battery current regen -60A
![image|690x436](upload://cZZiuasILpDI5QHiCOJBll7eUv5.jpeg) 
![Clipboard01|677x500](upload://woV6RUJ8VeU3CJzdvutkZktRrH7.jpeg) 

These numbers are nutz, I wonder if I need set them up manually or just leave them as suggested by the wizard?, for now I just manually use these settings, just to e on the safe side:

motor current max 80A
motor current max brake -70A
Battery current Max 40A
Battery current regen -12A

On the other hand after runing the wizard I see the the Motor Type is still in BLDC not FOC as stated on the wizard.

Anyone could help me making sense of all these?
```

---
## \#2 Posted by: BigBrit Posted at: 2019-05-25T22:51:25.709Z Reads: 165

```
Yes, read the VESC tool thread.  We were just discussing both these problems with Frank yesterday

https://www.electric-skateboard.builders/t/all-new-2019-vesc-tool-release/83619/568
```

---
## \#3 Posted by: Eboosted Posted at: 2019-05-25T23:16:26.571Z Reads: 159

```
I'd like to keep using this FW but it seems it's not a good option just yet.

I'm looking the reverse after pushing the trottle twice that I had with @ackmaniac FW, but I can't stand the low speed brake lock any longer.

In the meanwhile I'll try @skatardude10 fix :slight_smile:  

https://www.electric-skateboard.builders/t/latest-firmware-for-regular-focboxes-with-low-speed-brake-lock/94941/6?u=eboosted
```

---
## \#4 Posted by: mutantbass Posted at: 2019-05-25T23:24:12.433Z Reads: 148

```
Same here but you can change those values after so its not a big deal. Just change it from bldc to foc and it works fine.
```

---
## \#5 Posted by: rojitor Posted at: 2019-05-26T08:57:26.445Z Reads: 140

```
I had trouble with it. I got the "too old firmware " message. I updated as usual but after reset the same message over and over. I updated 5 times in a row. No luck. I flashed the vesc with st-link and it worked after that. I am not sure where the problem was. Never happened before
```

---
## \#6 Posted by: trampa Posted at: 2019-05-26T13:09:38.349Z Reads: 120

```
You had no bootloader installed. No need for an ST link. You can upload the bootloader via vesc tool.
You can also use a second vesc to act as a programmer. Interconnect gnd, Io, clk, power up both units, open SWD Prog tab, hit connect, select hardware, flash.
```

---
## \#7 Posted by: trampa Posted at: 2019-05-26T13:19:12.163Z Reads: 116

```
[quote="Eboosted, post:1, topic:94967"]
motor current max 80A motor current max brake -70A Battery current Max 40A Battery current regen -12A
[/quote]
These settings are wrong.


Better: motor max 67A
Motor regen:-40A
Batt max 50A 
Batt regen:-35A 

Batt regen needs to be high enough to give you good brakes at speed. It's a value that will never be seen by your battery for more than a very short time. Amps drop fast during braking. 

The new tool puts HW4.xx to BLDC to avoid HW damages. You can change that to FOC later.
```

---
## \#8 Posted by: Eboosted Posted at: 2019-05-26T17:57:19.087Z Reads: 91

```
[quote="trampa, post:7, topic:94967"]
These settings are wrong.

Better: motor max 67A Motor regen:-40A Batt max 50A Batt regen:-35A
[/quote]

I didn't state those values on my first post. 

The new VESC Tool automatically sets weird maximum current values, these values are for the first time assigned by the tool, usually the user is the one that state current limits during ESC setup. 

I wonder why Vedder chose to assign there limits automatically.

Maybe the tool needs polishing at this time
```

---
## \#9 Posted by: trampa Posted at: 2019-05-26T19:07:11.043Z Reads: 81

```
Vesc-Tool can now figure out the max Amps your motor can take reliably. You don't need to drop in any values you guessed. 67A is what your motor can swallow reliably.

With regards to batt max: If you would drop in 1000A, motor max would be the limiting factor. You can't pull more than 67A in our case. 

Batt max regen is a bit theoretical, since you can't push -60A realistically. That would be 3000W braking on a 12S system. You can't do that without you flying while your board stops. Naturally Amps are limited by your thumb. 
The only scenario that would put a lot of strain your battery is an extended high speed run on a very very steep hill. Basically a hill that is steep enough to keep you at high speeds, although you apply hard brakes. In that case you need a big fat amp swallowing pack anyway. Riding such a steep hill without proper brakes is no option. 
At 50% duty, you can't push more than -33,5A (-67A motor regen/2), and doing so, your speed would soon be at 25% duty and your down to -16.75A.
On Regen we usually see short spikes, which decrease fast in value. That's no problem for modern LiIon cells. 

You can lower the values manually if needed (advanced tab). For the now VESC-Tool assumes that your battery performance matches the motor performance, which makes sense in a way. If you want 5000W output power, your battery should be able to deliver that. 
We could also assume that per 1000mAh of battery capacity we can pull 5 Amps.
For a 12S4P 12000mAh Q30 pack that would result in 60A batt max.
```

---
## \#10 Posted by: mishrasubhransu Posted at: 2019-05-26T23:33:22.325Z Reads: 63

```
It assigns the motor current based on the size of the motor(that you select) and on the resistance of the winding. Size decides heat dissipation and winding resistance decides heat production. You can always reduce those limits if you don't want that big of an oomph.
```

---
## \#11 Posted by: trampa Posted at: 2019-05-27T07:30:09.629Z Reads: 50

```
Heat losses of 60W are very realistic for a wide range of motors we use in e-skate. So it's fairly easy to determine the max Amps. Stator saturation might be at a bit higer Amp values, but it's not wise to go close to saturation. If VESC-Tool finds out 67A, it might be possible to push 75A without going into saturation, but at 75A the motor is operated beyond thermal capabilities.
```

---
## \#12 Posted by: Pimousse Posted at: 2019-05-27T07:57:50.489Z Reads: 49

```
[quote="trampa, post:9, topic:94967"]
For the now VESC-Tool assumes that your battery performance matches the motor performance, which makes sense in a way.
[/quote]

VESC Tool needs to comply with the most ways, not only one.
How many people are using a dual setup with Li-ion ?
Like dual on a xS4P or sometimes less !
Auomation for amp "guessing" is really dangerous 
And trust me : I have a lot of private messages since I published a VESC Tool tutorial on YouTube. A lot of people are really confused by those crazy values generated automatically.

Need to report it to Benjamin.
```

---
## \#13 Posted by: taz Posted at: 2019-05-27T08:13:53.925Z Reads: 44

```
I find the suggested values for the motors very close to what I set them if I don't want to deal with constant overheating issues. :ok_hand:

The battery suggestions, although fine in some of my cases can be high and if I were Benjamin or you (which I am neither), I would choose the conservative approach of the previous vesc tool and leave it up to the user to increase them.
```

---
## \#14 Posted by: trampa Posted at: 2019-05-27T08:26:13.215Z Reads: 42

```
 Unfortunately most users use way to low Batt regen settings and way to high Motor regen settings. These values should be balanced ( e.g. -45A MR and -35A BR). We will look into a solution to determine Batt capabilities automatically.
```

---
## \#15 Posted by: taz Posted at: 2019-05-27T08:29:39.452Z Reads: 42

```
Agreed. The problem lies with the fact that many are using discharge BMSs.

Especially the ones that have the same connection for charge / discharge , would shut down if a too high regen value is used leaving the board without brakes.

I know your feelings on discharge BMSs and I share them but I feel it is better to take an approach that would suit the majority.
```

---
## \#16 Posted by: visnu777 Posted at: 2019-05-27T08:31:50.986Z Reads: 39

```
I use a way too low (-50/-10 dual) setting myself, never had any problems with it, my brakes are perfect for me (and no, I'm not going flat lands, more the opposite)
```

---
## \#17 Posted by: trampa Posted at: 2019-05-27T08:31:57.343Z Reads: 38

```
[quote="taz, post:15, topic:94967"]
Especially the ones that have the same connection for charge / discharge , would shut down if a too high regen value is used leaving the board without brakes.
[/quote]

discharge BMS is sort of dangerous if it is not very beefy and reliable. Those kinds of BMSs are not really available today or mega expensive.
```

---
## \#18 Posted by: Pimousse Posted at: 2019-05-27T08:32:55.641Z Reads: 40

```
35A BR ?
So 70A for a Dual ? What kind of battery (mostly Li-Ion largely used nowadays = 4A per P) can handle that ?
```

---
## \#19 Posted by: trampa Posted at: 2019-05-27T08:34:20.165Z Reads: 40

```
You should up the Batt regen to get better linearity and better grip at speed. Try it out yourself and don't be afraid that you will blow your battery. These are spikes and not constant Amps.
```

---
## \#20 Posted by: taz Posted at: 2019-05-27T08:34:43.531Z Reads: 42

```
All of them since it is just for a few seconds they will see that current.

I use -40A regen per vesc in my Trampa with a 12s7p 30q.

With -50A per motor it makes for very powerful yet smooth brakes.
```

---
## \#21 Posted by: mishrasubhransu Posted at: 2019-05-27T10:10:16.357Z Reads: 38

```
[quote="Pimousse, post:12, topic:94967"]
> For the now VESC-Tool assumes that your battery performance matches the motor performance, which makes sense in a way.

VESC Tool needs to comply with the most ways, not only one. How many people are using a dual setup with Li-ion ? Like dual on a xS4P or sometimes less ! Auomation for amp “guessing” is really dangerous And trust me : I have a lot of private messages since I published a VESC Tool tutorial on YouTube. A lot of people are really confused by those crazy values generated automatically.

Need to report it to Benjamin.
[/quote]

Is it though. I think it sets the battery amp based on the Ah of the Battery. I remember it setting much lower battery Amp when I had set the Ah to 5 than when at 10Ah
```

---
## \#22 Posted by: BigBrit Posted at: 2019-05-27T10:47:27.614Z Reads: 32

```
Totally agree with this, I use -30A per vesc for regen on a 10S8P, this is max brake and you only see it for a split second.  If you dont set this value high enough on 200mm wheels you dont feel any brakes.
```

---
