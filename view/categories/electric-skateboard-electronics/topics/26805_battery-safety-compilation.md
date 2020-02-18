# Battery safety compilation

### Replies: 1 Views: 723

## \#1 Posted by: jotatsu Posted at: 2017-07-05T02:58:26.511Z Reads: 119

```
Hello 

I'm new in the esk8 scene, but i have a little more in endless sphere, power walls and that kind of stuff. For esk8 community i've not seen some discussion on the battery safety topic, so i've made here a little recopilation of the tips i've seen to add safety to the diy packs that we have to produce.

**DISCLAIMER**: INABE I'm Not A Battery Expert, some people work this stuff as a profession in the industry or academia, if there is a disagrement between them and me, or between you and me, i will pick me last. 
**DISCLAIMER 2**: I speak one total language , 1/2 bad spanish and 1/2 bad english...
**DISCLAIMER 3:** Read battery university, endless-sphere, this forum. There are guys that have been doing this for years and have shared the experience

---- **Motivation**

* Economical. The more safety feature you have, the less chance  part or your whole pack goes wrong, given that people put between 50-200 usd in only cells , its as way of protecting your investment (not counting that the battery can damage other components in the process of kicking the bucket). 
*  Liability. This is DIY, you carry the consequences of a fire in your house, residential building, your job or on the street. You have to think that you are working with dangerous materials, and by that token, you should do your best try to make them safe

* -S*** happens: Think that laptop manufactures, Boeing, Samsung, Boosted and many others have had problems with batteries, and we are talking about established companies and mega companies. You and i are not better than those guys at manufacturing and QC.

-- **General recommendations.**

* Have a fire extinguisher handy

* If you are gonna store batties on bulk choose a dry place that is not under sunlight, not near stuff that can catch fire if the batteries do. If you can buy fire proof bag better. 


-- **Design considerations**

* Cell chemistry: I'm not gonna cover the different variations, there is a ton. But you need to have a general idea of what chemistry you are going to use. All of them have different characteristicas in capacity, safety, C rating, voltage. etc. 
*  Cell format: Here you have 2 choices pouch or cilindrical. Both have different safety considerations as both implement slightly different passive and active mechanism. Pouch for example bulge when something is wrong , cilindrical vent . 
* Cell source: If you can buy new, form a reputable source. The market is full of fake batteries, recycled batteries, etc etc. Dead laptop batteries were a source for tesla walls, but given the way a skateboard treat batteries i dont think is a good idea to use "almost new" cells.
* Putting it together; You can either solder, spot weld, use preconnected packs, ez assembly packs or ultrasonic weld. I've seen no1 use the latter, most people solder or spot weld. Take into consideration that a spot welder is another thing you have to borrrow/build/buy and that soldering may damage your battery. 

--**Passive measures**

* Spacing : I cringe at the sight of the e-bike community packs (sorry guys) . Those are humongous packs that normally are compacted in a large brick. The thing is batteries produce heat, and in compact arrangements, heats goes to the adjacent cells. If one cell goes into thermal runuway, it will drag the other cells even if its aislated electrically from the pack. In skateboard the things are better as you normally do a a flat pack. If you can, think about a little more spacing between the paralell packs, or maybe every certain number of cells.
*  Venting: Imagine that the  pack goes wrong, while it burns it will release a lot of hot smoke and flames. If you put something like a safety pressure valve you can direct where that pressure goes. If not the pressure can build inside whatever box you put the batteries making the fire worse or even making a nice skateboard grenade.
* Intumescent coating: This is directly from the tesla patents, is a coating that absorbs heat and expands helping to aislate the fire. I've not seen this one implemented much, i don't know why give that the coatings are very cheap. 
* Crapping the bad cell. This one is hard to implement but offers a nice protection agains individual cells going thermal runaway. Basically if a cell gets too hot it will melt the adjacent support and will fall outisde of the pack. 

--**Electrical measures**

* Cell fuses: Fuses rated for the max discharge of the cell and a little more, connected between each cell and the positive side of the battery . Protect against the cell short circuit and receiving the whole current of the pack. I've seen resistor legs, thin wire,. thin nickel strip and proper fast glass fuses in this one. So far, the glass fuses seem the most reliable. 
* Battery fuse: Goes at the end of the battery, rated for the maximun short burst of the battery and a little more. Protect the battery in case the esc and beyond go haywire.
* Wiring and connectors: If you dont pick the right wires for your application, they will get really hot , they could melt the insulation and short circuit each other. The general recommendation i've seen is going 8awg silicone wire and xt90 connectors just to be on the safe side. On the same token, the intercell connector can be done either with pure nickel strips or a thick copper wire 'bus bar'
* Loop keys or manual ways to disconnect or turn down the electrical circuit in your skateboard. Its not fun when something is shorting and you have now way to turn off the damn thing. I dont know much about this ones. 

--**Electronic measures**

* BMS: Main job is to keep the voltage of the individual cells very close. Some of the features are overcharge, overdischarge, shor circuit, etc. The really smart ones have cycle counters, coulombic efficiency measure, capacity calcultar, CAN , I2C, blueooth  communication, soft switch, among others. (for a $$$ of course). I like the ones that beep when they are dying.
* BVM: Voltage monitor, sometimes integrated into the BMS, other times you can use a simple hand held device that tell you the voltage of each cell so you can decide if the pack is good or going to hell. 
* Hobby chargers. This is like an external BMS, you connect the balancing leads to this thing and it will charge the batteries mantaining the voltages of them close. 

--**Other considerations**

* Unlike vapers, tesla walls or other applications, you are going to beat the s*** out of the pack. Is the pack ready to take vibrating, smacks, deck flex, etc, without shorting, disconecting or damaging the cells?
*  Water, the sworn enemy of all electrical stuff. Is your battery water-proof? water-resistant? or a sponge that will take any moisture and put in between the cells. 
* Heat and cold. Your batteries dont like the two extremes, so in those places you have to think of the battery temperature during operation. 

Thats all i can think of, i hope some is true and valuable.
```

---
