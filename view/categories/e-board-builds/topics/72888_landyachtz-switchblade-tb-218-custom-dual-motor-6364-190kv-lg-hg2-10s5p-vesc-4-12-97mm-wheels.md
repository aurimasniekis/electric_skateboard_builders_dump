# Landyachtz Switchblade &#124; TB 218 &#124; Custom &#124; Dual Motor 6364 190kv &#124; LG HG2 10s5p &#124; VESC 4.12 &#124; 97mm wheels

### Replies: 5 Views: 675

## \#1 Posted by: Electrotechnics Posted at: 2018-10-31T06:05:50.233Z Reads: 166

```
I decided to begin this build after my original DIY single motor esk8 was run over by a University bus (the driver didn't even stop after cutting a corner, nearly running me over, and totaling my longboard!)

This build has cost me around $1000 total. I started with a Landyatchz Switchblade 38" deck, paired with the TB 218mm trucks and 97mm wheels, after that, everything else is custom on this board. I top mounted the deck with spacers I designed and 3d printed to prevent wheel bite and to provide clearance for the battery. Next I designed up a dual motor mount to be cut out of a 3mm carbon fiber plate, and with a quick run on the CNC, I had the parts for my motor mount. This mount design can be rotated to be underneath, or rotated backwards in a reverse mount configuration as I used. 

Long board after meeting the underside of a bus.   
![wrecked%20board|666x500](upload://v5NVX0HsXvROMywlA8LgnyVIRIf.jpeg) 

Mount design:
![motor%20mount%20cad|666x500](upload://ylkkJRfqSsj5vY72pnGYMDqYk6V.jpeg) 

Carbon parts:
![motor%20mount%20pieces|666x500](upload://6CO8jXIIrUbpNnKYvOwDs91HSCn.jpeg) 

Dual mount assembly: 
![motor%20unit|666x500](upload://ngCjwylDO7CoYrIaFuWrDd5UrTj.jpeg)
```

---
## \#2 Posted by: Electrotechnics Posted at: 2018-10-31T06:13:12.448Z Reads: 149

```
For motors I used two KEDA 6364 190kv motors, rated for 2000W each. The shafts do not have a key-way or a flat; so the first thing I did was disassemble the motors, and mill a flat onto the motor shaft. Overall the KEDA motors are well built, and look and feel great despite only costing $37 each! 


Keda 6364 190kv motors:
![motors%20apart|666x500](upload://xv77sw8Woe6OYRvgtqz5Zeop19R.jpeg) 

Flat milled onto motor shafts: 
![milled%20flat|666x500](upload://iWCebNcz8jzGrRmpadYXLz9e6Hv.jpeg) 

Assembly of drive train: 
![motor%20mount%20adapter%20bench|666x500](upload://bqDPuESlBcNeHuXQDHn2KoyF2Rb.jpeg) 


Mounted on the deck:
![motors%20back|666x500](upload://nKqScbiwbpRywbiqAZcFQ4VXsah.jpeg)
```

---
## \#3 Posted by: dareno Posted at: 2018-10-31T06:28:43.498Z Reads: 138

```
Check that rear bearing.  Hk stuff is coming with badly seated bearings lately.  That one looks deformed.
cool build btw  love the carbonny bits
```

---
## \#4 Posted by: Electrotechnics Posted at: 2018-10-31T06:32:26.608Z Reads: 147

```
I custom built my own 10s5p battery pack out of LG HG2 cells. This battery is 36 volts, 15,000 mah, 540wh and has a 100a max discharge. I bought a lot of 50 cells for $167 so they were about $3.35 per cell...not bad at all. 
I chose to solder the battery pack together, as the solder joints have far less resistance than battery tabs, which is crucial when expecting to draw 20a per cell max. Soldering 18650's is a perfectly valid way of assembling a pack, it just requires a 65w+ soldering iron and very good soldering skills, the soldering iron stays on each cell for no more than a second, causing no damage. 

Mock up of how the cells will be arranged on the deck before assembly:
![battery%20mock%20up|666x500](upload://ywq2wtvW0LhYZwwRKlidxg26AO4.jpeg) 

Next I grouped the cells into sets of 5 using 16 awg high stand wire with silicon insulation. 
![solder%20top|666x500](upload://nTJiNZ7I2BsYUe92qpSfos3G1T.jpeg) 

Then I arranged the parallel packs into series to make two 5s 5p packs, I attached the 3 sets of 5 cells side by side together using double sided foam tape, allowing the pack to flex with the deck without any damage: 
![finished%20battery|666x500](upload://gFJ4bOh5ZUlBb91GhyIl69IcwVH.jpeg) 
![series%20cells|666x500](upload://gtyFfA1U7pu7Hlc4m5ZOjtuXSEb.jpeg) 

Battery packs finished with balance wires attached: 
![finished%20battery|666x500](upload://gFJ4bOh5ZUlBb91GhyIl69IcwVH.jpeg) 

I have some battery pack heat shrink coming in so that packs will be wrapped when fully complete.
```

---
## \#5 Posted by: Electrotechnics Posted at: 2018-10-31T07:05:12.820Z Reads: 128

```
I used two different branded VESC 4.12's one of them was the Torque Boards 4.12 ESC and the other is a Flip Sky VESC 4.12. I think the Flip Sky VESC is built better than the TB VESC, and its cheaper. I got the infamous DRV error on the Torque ESC, so I ordered up a few new DRV chips, and after 10 minutes of soldering, I had a new DRV chip installed. I also removed the power wires, and replaced them in the style that FlipSky uses, with a low profile inline connection to the capacitors. 
 ![drv%20replace|666x500](upload://eeA996F21UaS4jGXksNd54o8YXq.jpeg)
 ![vesc%20wiring|666x500](upload://tkgVPsDgq55aXp9ASq6AA32hKsI.jpeg) 



I am currently waiting on my second pulley to arrive in the mail, so I only have one wheel driven until it comes in. 
I could not wait to get it going so I strapped all the parts on the bottom using Velcro tape and Velcro straps. 

![deck%20layout|666x500](upload://iFsoL0zpuldLmFHnoSXAdunzr0F.jpeg)
![working|666x500](upload://4DhFqNq5yVVn1PWiRbHpQAjLzyQ.jpeg) 

This thing is super fast with just a single motor. I can't wait to get the second drive pulley installed to see what kind of power both motors together have. 
The next stage of this build is going to be designing and building a carbon fiber enclosure. 

I have the needed materials and vacuum bagging equipment to do a full epoxy resin and carbon fiber layup for the enclosure. So I need to design the enclosure shape, 3d print a mold plug for it, make a mold, then do the actual layup to make the case. I'm hoping to get some very nice looking carbon fiber enclosures out of the mold. I will post the results, and if anyone is interested in a carbon enclosure big enough for 50 - 18650 cells and two VESC's I might make some more and sell them. 

Other future mods might include upgrading to the FocBox Unity later this year when it is finally released. 

![temp%20config|666x500](upload://zYHulwIDvKjKivFQAHCD2d6DYGz.jpeg)
```

---
