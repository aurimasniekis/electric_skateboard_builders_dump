# \[Troubleshooting\]\[E-MountainBoard\] What am I Doing Wrong?

### Replies: 6 Views: 209

## \#1 Posted by: Davewesh Posted at: 2019-06-07T17:33:41.470Z Reads: 68

```
<p>Alright guys, I am at my wits end here. I apologize for the lack of info to start since I am at work I don&rsquo;t have the means to pull the VESC Tool Config, but I can recall most of the points here.</p>
<p>Problem:</p>
<ul>
<li>Poor Start up Torque</li>
<ul>
<li>I MUST be on flat land otherwise it will fault</li>
<li>I Cannot 'gun it' at all or it will fault.</li>
<li>Most of the time, I need to Shuffle the board to get it to move/</li>
</ul>
<li>Motor (VESC) Stall at Max Throttle</li>
<ul>
<li>Once I get moving and I can peg the throttle, the VESC will fault.</li>
<li>Even at full Throttle if I even look at some grass, the VESC will fault (not really but it will chew through my speed then fault after about 50-100 feet).</li>
</ul>
<li>Brakes are Terrible</li>
<ul>
<li>If I hit the brakes it will slow me down however, if I slam on the brakes - it will slow me down until it faults out again.</li>
</ul>
<li>Inclines (couldn&rsquo;t give a angulation) are a joke</li>
<ul>
<li>Going back to scrubbing speed and eventually faulting.</li>
</ul>
</ul>
<p>Specs:</p>
<ul>
<li>My Weight: 225LB</li>
<li>MBS Atom 90</li>
<li>Torque Boards 6374 x2 (<a href="https:///products/electric-skateboard-motor-6374-190kv">https:///products/electric-skateboard-motor-6374-190kv</a>)</li>
<li>HDT 15MM Wide 20Tooth Drive</li>
<li>HDT 15MM Wide 84Tooth Driven</li>
<li>MBS Wheels/Tires (200MM) (8")</li>
<ul>
<li>Factory Setting @ 36 PSI (Should I go higher?)&nbsp;</li>
</ul>
<li>10S1P LiPo 8AH 25C</li>
<ul>
<li>SPIM08 LiPo</li>
</ul>
<li>FlipSky VESC 4.20 Dual</li>
</ul>
<p>Firmware Settings:</p>
<ul>
<li>FOC - Sensored</li>
<ul>
<li>Each Motor Individually Detected</li>
<li>Each Motor Hall Sensors Detected</li>
</ul>
<li>General Settings</li>
<ul>
<li>Motor Max 50-80 AMP</li>
<ul>
<li>(I've had it in that range with no changes)</li>
</ul>
<li>Motor Regen Max -40 AMP</li>
<ul>
<li>Batteries are 15C charge capable</li>
</ul>
<li>Battery Max 100 AMP</li>
<li>Voltage Cutoff (defined via VESC Calc)</li>
<li>Min and Max Voltage (defined as default 5v~ to 57v~)</li>
</ul>
<li>Input Settings</li>
<ul>
<li>RC Remote (for now)</li>
<li>PPM with Current no Reverse</li>
<li>Traction Control = False</li>
</ul>
</ul>
<p>Nothing else stands out to me on this right now, but this is what ive got. I know that the Motors I have are designed for 12S and therefore may be inefficient at 10S voltage but I can't imagine that-that would be an issue. As well I made sure that when I last tested the board that battery voltage was (off load) sitting at around 42V (41.3).</p>

<p>Really at a loss here as from everything that ive seen I should be capable of tearing it up on pretty much any surface right now but it seems like its neutered. Im sure that my weight has something to do with the expected performance - but so much so that this thing chuggs all the time?</p>
<p>Any input would be fantastic, Thanks Guys and Gals!</p>
```

---
## \#2 Posted by: Balta_6 Posted at: 2019-06-07T17:47:45.407Z Reads: 55

```
Yeah, it's the vesc 4.20, I bet it's not the PLUS version that came after to correct all the cutouts
It's a known issue, look it up here, you should only set 30A max per motor, it will should be better (no cutouts for me on a AT board, not MTB tho)
But breaking I don't know why it's so weak


The best solution would be to buy another esc, the dual 6.6 is good, or a unity if you wanna stick with dual esc
```

---
## \#3 Posted by: Davewesh Posted at: 2019-06-07T19:03:47.268Z Reads: 50

```
~~FOCBox Unity (Pre-orders out till Late July or August most likely) or VESC 6.6 - Which would you Suggest?~~ Ill probably just go with the 6.6, On paper it runs better higher amperage than the FOCBOX, and I can get it sooner and significantly cheaper. 

Looking forward to getting home and lowering the motor settings to see what I can get out of it with regards to it cutting out. If anything ill have to find another use for it or just sell it /smh.
```

---
## \#4 Posted by: Balta_6 Posted at: 2019-06-07T20:00:29.400Z Reads: 41

```
The big problem with the unity is it's availability which is shit, and now there is a big problem that some people experienced a sudden cut, which obviously resulted in fall
```

---
## \#5 Posted by: Davewesh Posted at: 2019-06-07T20:03:58.280Z Reads: 40

```
Yeah, Id like to get this board running well so that I can justify upgrading in the next month or so. So we'll get the 6.6 on order now, and maybe ill look into the FOCBOX when im ready to upgrade the board and trucks to something a bit more 'highend' (probably trampa) . I have 5 months to spend my "wellness" fund at work and Mountain Boards are approved :smiley:.
```

---
## \#6 Posted by: Davewesh Posted at: 2019-06-10T00:23:58.812Z Reads: 22

```
Edit: 

As far as the cutouts/Stalling goes this still occurs however, the issue with starting from a stop or grass/incline based movement has been resolved by moving from a 20 tooth drive to a 14tooth drive HTD gear. 

This effectively increases the gear ratio from 4.2 to 6 which made an insane difference. Everything else appears to be a limitation with the 4.20 vesc from flipsky as mentioned previously.
```

---
