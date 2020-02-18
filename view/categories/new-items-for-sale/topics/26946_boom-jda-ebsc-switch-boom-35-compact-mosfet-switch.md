# :boom: JDA EbSC Switch :boom: $35 Compact MOSFET Switch

### Replies: 24 Views: 2789

## \#1 Posted by: JdogAwesome Posted at: 2017-07-06T23:11:46.207Z Reads: 422

```
Hello Esk8ers! If your familiar with these forums you've probably seen me on here for a while now mainly on my  [EBoard MOSFET Switch](https://www.electric-skateboard.builders/t/eboard-mosfet-switch) thread and thats where this all kinda started. Anyways the main point of this thread is for me to advertise my new EBoard Switch or as I like to call it the EbSC or EBoard Switch Compact (I know bad name but it gets the job done). Everything about all my past designs and switches has been completely open source and I plan to keep it that way. Below you'll find all the schematics and board layouts to make your own switch or to design one for yourself. However for the people who dont want to build one themselves, im selling them as well. The current V1 board utilizes two IRFS7530 MOSFET's the same ones used on the VESC and has a current capability of 40A continuous with far higher burst currents which is plenty for most boards. The switch works with 6S-12S battery Setups with an absolute max of 60V or technically 14S though I wouldn't risk getting that close to the limits. My switches also included blue LED push buttons with sockets for super easy installation. They feature dual 12V Zener gate drivers to make sure the FET's are running at optimal efficiency as well as extra redundancy in case one of the gate drivers were to fail. If you happened to take a look at the PCB diagrams or layouts you would notice how theres no solder mask over the main current carrying traces. This is because there will be a layer of solder applied to the top of the traces to increase the current carrying capabilities. I also plan to add a conformal coating to the entire switch for added durability and to help protect the exposed traces. I also include with anything I sell a lifetime satisfaction guarantee to make sure that your happy with your purchase. Anyways thats enough rambling ill get onto the pricing.

Update: New V2 EbSC's Will utilize the IRFS7730 MOSFET instead as it is a 75V MOSFET that can handle voltage spikes better than the IRFS7530.

**Pricing:**

Price for a **single** EbSC is $35 + $3 domestic shipping (US only) 
2+ Switches shipping is free

**PLEASE DM ME IF YOUR INTERESTED IN ORDERING**




**----------------------------------------------------------------------------------------------------------------------------------**

**Eagle Schematic and Board layouts** can be downloaded [HERE](https://github.com/JdogAwesome/EbSC) from the GitHub repository.

Thank you for showing interest in my design, the Esk8 community is awesome and I love to help everyone out. Please leave any questions or comments down below and ill try to answer them all. If you did purchase one thank you so much! The profit I make off these goes towards funding my other projects like a new EBoard as well as some more exotic ones like my DRSSTC.

<a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/">Creative Commons Attribution-NonCommercial 4.0 International License</a>.
```

---
## \#2 Posted by: longhairedboy Posted at: 2017-07-07T19:39:46.695Z Reads: 342

```
What's the voltage on those mosfets?
```

---
## \#3 Posted by: JdogAwesome Posted at: 2017-07-07T19:45:38.555Z Reads: 334

```
Same as the VESC, 60V IRFS7530's
```

---
## \#4 Posted by: karma Posted at: 2017-08-07T18:49:08.407Z Reads: 292

```
Have you recieved them now? Could you post an update and maybe some pics? :)
```

---
## \#5 Posted by: longhairedboy Posted at: 2017-08-07T18:50:02.342Z Reads: 285

```
bump those up to 75v and you'll have me.    I routinely fried 60V rated fets at 12S.
```

---
## \#6 Posted by: JdogAwesome Posted at: 2017-08-07T19:09:43.127Z Reads: 275

```
@karma yeah I do have a bunch of pics, ill post then down below.

@longhairedboy hey LHB, what exactly do you mean you've friend 60V rated FET's? Like other MOSFET switches that have died, or VESC MOSFET's? If there other vendor switches then I think its definitely a drive voltage problem like I've seen on some other ones and not a mosfet voltage rating problem. Though yeah I would love to use higher voltage FETs to have extra headroom, but there arent many options that have such a low RDSon like the 7530s, Ill take a look into it though.


<img src="/uploads/db1493/original/3X/0/1/019e0ef3a407062aa1939567d59a9e6a0f257340.JPG" width="690" height="460"><img src="/uploads/db1493/original/3X/3/6/361fe409428bdcead3795279515bf939f872e41b.JPG" width="690" height="460"><img src="/uploads/db1493/original/3X/f/d/fd8c944e05d0eb784415ade4deeb79fb358df834.JPG" width="690" height="460">
<img src="/uploads/db1493/original/3X/0/8/087c0472f82ccef7a37e0df9a52ff7b6baa786f0.JPG" width="690" height="460">
```

---
## \#7 Posted by: longhairedboy Posted at: 2017-08-07T19:18:09.938Z Reads: 245

```
These are what i'm using. The IRFS7734. It was reccommended by a freind as a drop in replacement for the Vedder switches which is what i'm using.

https://www.instagram.com/p/BLl6ZZtAihf/?taken-by=longhairedboy

but what i mean by frying is that after a short while of seeming to be ok on 12S the original mosfets in the Vedder switch would fail closed leaving the board permanently in the on position. And so would the Flyer type 8-12S eswitches. I burned up i don't know  how many switches. But now i have zero issues. 

I don't know if that relates at all to your particular product, i just thought it might be helpful to know about. 

I'm not an EE or circuit designer. Electrons are still a source of witchcraft to me, but i know what works.
```

---
## \#8 Posted by: fedestanco Posted at: 2017-08-07T19:49:37.310Z Reads: 220

```
Is this for real? Maybe we have to revise @JTAG  bms'BOM

Actually 60v should be plenty even at 12s. Probably some downhill braking has killed them in your case.
```

---
## \#9 Posted by: longhairedboy Posted at: 2017-08-07T19:52:56.726Z Reads: 223

```
I assure you its more than real. I burned up TWO Ollin vedder switches (no fault of ollin's, at the time bugs were still everywhere) and probably a dozen of the flyers. This was at a point where i was in transition from using the flyers to using the ollins, which were original Vedder spec eswitches. 

@oriol360 and @torqueboards remember my ridiculous orders for half dozens of flyer switches and I think something i said to somebody about @chaka's switches at the time made him mad at me, but we're all good now.

Now i'm getting them directly from Macrofab with this slight modification and i have had ZERO issues. 

All ofthis happened about a year ago, and i still have the first of these type i'm holding in that pic in my daily rider working flawlessly under the worst conditions. They can handle the regen currents of hard braking easily and they can handle the currents associated with racing up hill with no trouble at all. 

one race on the old type and my shit wouldn't turn off anymore.
```

---
## \#10 Posted by: fedestanco Posted at: 2017-08-07T19:55:42.701Z Reads: 214

```
Good to know. Fortunately fets are among the components I havent ordered yet.
Are the 7734s holding strong?
```

---
## \#11 Posted by: longhairedboy Posted at: 2017-08-07T19:56:13.868Z Reads: 205

```
i sort of ninjaed your answer but yes, they are still going very strong.
```

---
## \#12 Posted by: JdogAwesome Posted at: 2017-08-07T20:23:32.317Z Reads: 198

```
Yeah those IRFS7734 are nice and have that 75V headroom, however there RDSon is 3mOhm's compared to the 1.4mOhms of the 7530 which means that the 7734 will get twice as hot as the 7530 at the same current draw. However if they've been working well for you and haven't been getting to hot then yeah thats a great choice. Ill look into it some more to see if theres any better choices, thanks for the info though! What im guessing is the main reason the FETs are dying other than improper drive voltage is like @fedestanco said, the braking can create some very high voltage bursts which can kill the MOSFET's. Whats weird is that the huge cap banks on the VESC's are supposed to suppress those types of voltage spikes. I think im going to through my VESC onto my oscilloscope and see if I can catch any high voltage spikes.

Also @longhairedboy I would love to get some of those broken switches and try to dissect and figure out what killed them and maybe fix them, DM me if your interested.
```

---
## \#13 Posted by: JdogAwesome Posted at: 2017-08-07T20:35:30.879Z Reads: 185

```
Well did a bit of digging and I found a great choice actually. Instead of the IRFS7734 the [IRFS7730](https://www.infineon.com/dgdl/irfs7730-7ppbf.pdf?fileId=5546d462533600a40153563ab68221e0) has RDSon of 2mOhms compared to the 3 of the 7734. I think the 7730 is actually a great choice, its also only $2.18 a piece on [Arrow](https://www.arrow.com/en/products/irfs7730trl7pp/infineon-technologies-ag). I think im actually going to start using these FET's in all my switches cause there RDSon is only slightly higher but the voltage increase will be great. Thanks @longhairedboy
```

---
## \#14 Posted by: chaka Posted at: 2017-08-07T21:15:28.953Z Reads: 185

```
Those look a lot like my revision on OSh Park ;)
```

---
## \#15 Posted by: trancejunkiexxl Posted at: 2017-08-07T21:20:20.718Z Reads: 182

```
good to know i was going to buy a bunch of the flier switches, its nice to have options =)
```

---
## \#16 Posted by: banjaxxed Posted at: 2017-08-07T21:20:52.987Z Reads: 186

```


Can you tell me what it's called @chaka ? 🙏  [quote="chaka, post:14, topic:26946"]
Those look a lot like my revision on OSh Park :wink:
[/quote]
```

---
## \#17 Posted by: chaka Posted at: 2017-08-07T21:22:56.906Z Reads: 187

```
https://oshpark.com/shared_projects/XuqJkZzU

Have at it!
```

---
## \#18 Posted by: banjaxxed Posted at: 2017-08-07T22:21:52.974Z Reads: 180

```
Looking for assembled in Europe
```

---
## \#19 Posted by: longhairedboy Posted at: 2017-08-08T00:00:18.236Z Reads: 176

```
is the 7730 a drop in replacement? because i would like to use those on my eswitches if they're better for this application. Even though i';ve not had any issues, reducing heat is always a priority so if these run cooler at the same performance level than i want them. 

wow this thread has been a really good one. This is what its all about.
```

---
## \#20 Posted by: JdogAwesome Posted at: 2017-08-08T00:14:54.759Z Reads: 172

```
Yep the 7730 us the exact same package, D2PAK7P, as the 7734 and 7530 MOSFET's. And yeah the reducing heat is always a good thing!
```

---
## \#21 Posted by: deucesdown Posted at: 2017-08-09T16:25:42.601Z Reads: 164

```
Sorry if this has been discussed elsewhere. What's the failure mode on these guys? open? closed? short? all of above?

And is the standby consumption negligible?

I'm using antispark loop key because above issues always skeeve me out.
```

---
## \#22 Posted by: JdogAwesome Posted at: 2017-08-09T16:39:51.426Z Reads: 171

```
Well in the case that these failed, what usually happens is the MOSFET's fail in a drain to source short which would mean the mosfets would stay in the on position, which would mean you cant turn off your board. It's never happened with my new switch designs though if it did I would be happy to fix them for you. MOSFET's when pulled low, or off, have a extremely high resistance which means the standby current is practically non existent. Loop keys are a great and cheap choice, though they never look quite as nice as a push button lol.
```

---
## \#23 Posted by: JdogAwesome Posted at: 2018-12-27T23:49:30.977Z Reads: 84

```
Just uploading latest Eagle files for anyone who would like to build their own switch. FYI this design is meant for 2oz copper, do not use it on 1oz substrate. [Dropbox Link](https://www.dropbox.com/s/aslw9s91jlty5rx/EbSC%20Switch%20V4.zip?dl=0)
```

---
## \#24 Posted by: Jonisonvespa Posted at: 2019-08-12T14:08:30.787Z Reads: 37

```
Hello
Wonder if any body has any pcbs for sale ?
In in the uk.
Thanks
```

---
