# External BMS and Charging Box

### Replies: 7 Views: 1304

## \#1 Posted by: SkaterBoy58 Posted at: 2018-12-31T04:10:11.018Z Reads: 242

```
Following on from requests for a separate build thread from my current build thread -   [La-croix-long-range-cruiser-carving-machine](https://www.electric-skateboard.builders/t/la-croix-long-range-cruiser-carving-machine/76960)  - this is all about the external BMS and Charging box I am currently building. All of my boards and auxiliary battery packs are 10S with all balance wires bought out to a 12 pin socket for an external BMS.

For completeness - below is the blurb from the original thread

A bit of an update on external BMS concept.

The concept is to build an external BMS box for charging the battery pack via a DieBie BMS and individual cell voltage indication with an added function of being able to individually discharge any of the 10 cell packs via bleed resistors. 

This concept requires all 11 ( for 10S) battery pack balance wires to be connected to a socket on the board enclosure.

 I have used this 12 pin IP68 socket on all my boards ![12%20pin%20plug%20and%20socket%202|505x489](upload://kqzgNlomUr7wr2t5cyxt0MshXOZ.jpeg) 


 It is relatively cheap directly from China ([12 pin plug/socket](https://www.aliexpress.com/item/SP2110-12-pin-waterproof-connector-IP68-LED-power-cable-connector-pancl-cutout-21mm-12pins-Plugs-and/32767770117.html?spm=a2g0s.9042311.0.0.27424c4dmdrgR0))

The main charging CCCV function will be  via a Drok unit that I will take out of my existing charger box.  You can dial up charging voltage and current and it has 10 preset charging V and I settings .

![2%20dps%20unit|556x500](upload://7gBzUOaMr8eUeBcDI1gAH2ncVyL.jpeg) 

The idea is to build this new BMS Charging box that I can use on new La Croix board, my existing Landyatchz DIY and various other 10S battery packs/boards.

The cell voltage indicator is a Chargery BS12 lcd unit that has audible alarm for OV and UV .
![chargery%20unit|690x420](upload://psUsrGC2kIWEzu5XqzjzdjJfm2m.jpeg) 

The external bleed resistors are 8 ohm 25W metal enclosure  which will give approx. 0.5A discharge 

![bleed%20resistors|651x289](upload://EgschgENzlL3YF2JZUJIeyjYFA.jpeg)  
[25W bleed resistors](https://www.aliexpress.com/item/10pcs-lot-25W-Golden-Aluminium-Resistor-1R-2R-3R-4R-5R-6R-8R-1-5R-2/32604093340.html?spm=a2g0s.9042311.0.0.27424c4dEopPMl)

The leds are ultrabright red and these draw approx 0.15A to aid the discharge and to show which cell is being discharged . These require 2.0V max so require 27 ohm resistor to drop voltage .![led|483x487](upload://f1jH6OANzoeudakB7g7BYSTD866.jpeg) 


 [superbright led link](https://www.aliexpress.com/item/20pcs-LED-10mm-Red-Ultra-Bright-Super-bright-LED-DIODE-Lamp-Light-Bulb-10MM-Round-top/32879810203.html?spm=a2g0s.9042311.0.0.4bd84c4d7GRHsp)

and of course the BMS will be the DieBieMS unit 
![IMG_20170323_165245|666x500](upload://suplV3gG1WiTSNMRfhEQt6ft1CR.jpg) 

[DieBie MS](https://www.electric-skateboard.builders/t/diy-6s-to-12s-bms-with-can-diebiems/2639)

So progress to date is to make all holes and cut-outs , mount switches , cell  lcd display , input and output sockets , bleed resistors and leds- all wired up and functioning but no BMS fitted yet.
![no%201%20|666x500](upload://cL89oJ4dOO5oSYQ1tgmx8WJPN7q.jpeg) 


Still to do is to insulate external resistor connections and mount remaining bits .
```

---
## \#2 Posted by: Sascha_stevenson Posted at: 2018-12-31T15:03:42.939Z Reads: 203

```
@SkaterBoy58 
Tesla Charger for ESK8?? 
Haha, looks great keep it up :wink:
```

---
## \#3 Posted by: deucesdown Posted at: 2018-12-31T18:32:46.905Z Reads: 188

```
Thanks for posting. I wrote up a bunch of questions, but I think the process of writing questions gave me answers.

The DieBieMS will perform final balancing, but it's slow to bleed down at 100ma or whatever. The manually toggled 25w (5.9a at 4.2v) resistors speed things up.

The chargery monitor has an audible alarm for a cell group hitting 4.2v, to tell someone to come toggle the switches.

Did I get that mostly right?

Did you consider going with 10 single channel TP4056 with isolating power supplies, instead of bleeding down? I'm thinking, this would only give 1a charge rate, but perhaps combined with bulk charging, might be faster overall, as you're not flipping between 6a and 100ma bleed, watching things oscillate. Like this:

https://www.electric-skateboard.builders/t/first-build-mono-6374-vesc-10s3p-bms-90mm-flywheel/37257/14
```

---
## \#4 Posted by: SkaterBoy58 Posted at: 2019-01-01T00:29:24.851Z Reads: 149

```
> The DieBieMS will perform final balancing, but it’s slow to bleed down at 100ma or whatever. The manually toggled 25w (5.9a at 4.2v) resistors speed things up.

not quite - the DieBieMS  comes with 15 ohm discharge resistors which gives approx 270mA discharge on cell voltage of 4V. 

and resistors draw current entirely dependant on applied voltage (and nothing to do with power rating of resistor) so the 8 ohm resistors will draw 500mA with 4V applied with a power dissipation of 2W .

in addition - the ultra-bright red leds draw approx. 100mA  more 

so the intention is to connect the 8 ohm resistor and the led in parallel with the BMS discharge resistor to get approx. 870mA discharge current on BMS balancing .

This is required due to the large cell capacity (30Ah) which would take forever to balance just using the BMS bleed resistors at 270mA.

The DieBieMS cell discharge mosfet ( a TSM2323)  is rated at 4.7A drain current continuously and 20A current pulsed with a max power dissipation of 0.8W at 70 degrees C . 
The Rds-on is approx 40mohms so at 870mA total discharge current gives a power dissipation of 31mW . 

The other benefit on connecting leds and external bleed resistors is that you can see the DieBieMS balancing the cells by the leds - which is quite cool.

![bms|375x500](upload://coYjMdpYnjtDgUTu72DtTAJSB0P.jpeg) 

I will draw up full schematic of the bms/charger and post here

A few other features I wish to incorporate are

* 2 output sockets - 1 via BMS control and the other directly from CCCV charging module (need this to use CCCV module to charge other batteries ( 4S and 8S LiPo ) and for general use

* additional of cooling fans to keep airflow over BMS resistors - and enabling five cells at a time to discharge during cell balancing

* a system to switch over charging current from 5A to 300mA for final charging up to 41.8V
```

---
## \#5 Posted by: SkaterBoy58 Posted at: 2019-05-06T00:51:34.710Z Reads: 91

```
This post is to detail another version of an external BMS charging system built for a fellow La Croix DIYer here in Perth Australia.

The basic specs are

* Digital displays for individual cell voltages ( its for a 10S 6P battery pack)
* LCD Meter on box showing Charging voltage/current/power with cumulative Wh
* Utilising DieBieMS  https://www.electric-skateboard.builders/t/diy-6s-to-12s-bms-with-can-diebiems/2639 PCB – but with external resistors to increase balance discharge current
* LEDs to show DieBieMS balancing function
* 10 switches to discharge individual cells
* External power supply and charging module tom provide up to 5A charging

The reason for the external balance resistors is that the DieBieMS only has 15 ohm bleed resistors which is approx. 250mA.

The battery packs on our LA Croix super long range cruiser boards https://www.electric-skateboard.builders/t/la-croix-long-range-cruiser-carving-machine/76960 are approx. 30Ah ( 10S 6P using 51E 21700 cells) and 250mA would take a very long time ( days) to reduce a P pack voltage during balancing.

With the external 6 ohm resistors and the super bright LEDs – the balance discharge bleed current is approx. 1A.

This build requires direct soldering to the DieBieMS – so it not for beginners learning to solder.

So first the schematic for balancing discharging- the blue on this schematic id DieBieMS pcb and the red is the additional wiring for this build. All balance/discharge wiring inside the box is 22awg silicon and all charge wiring is 16 awg silicon .

![photo%201%20cell%20discharge%20schematic|690x487](upload://ujC7DfxCGI1Gs8KgLwrwsi4YBBt.jpeg) 

The DieBieMS balance discharge Mosfet (Q5 TSM2323) is rated at approx. 4.7A continuous or 20A pulsed so there should be no problems switching the 1A balance discharge current.

![photo%202%20Q5%20Data%20Sheet|690x393](upload://gYptTVmDNNIvFlYUUHoMlXLRHt7.jpeg) 

Basic shopping list for the bits and pieces is as below

**Box**

https://s.click.aliexpress.com/e/bFzgp2Lq

**36V 11A Power Supply**

https://s.click.aliexpress.com/e/pznujNA

**CCCV Module**

https://s.click.aliexpress.com/e/zbwKGRA

**6 Ohm 5W Resistors**

https://www.aliexpress.com/item/5W-6-8-10-12-15-18-20-ohm-6R-8R-10R-12R-15R-18R-20R/32874540014.html?spm=a2g0s.13010208.99999999.284.30453c005BmJjY

 
**Switches**

https://www.aliexpress.com/item/10pcs-MTS-101-2-Pin-SPST-Switch-ON-OFF-2-Position-6A-250V-AC-Mini-Toggle/32901167568.html?spm=a2g0s.9042311.0.0.561f4c4da5TnmO

**Ultrabright LEDs**

https://www.aliexpress.com/item/20pcs-LED-10mm-Red-Ultra-Bright-Super-bright-LED-DIODE-Lamp-Light-Bulb-10MM-Round-top/32879810203.html?spm=a2g0s.9042311.0.0.2fad4c4dU7gBon

**Digital voltmeters**

https://www.aliexpress.com/item/0-28-Inch-2-5V-30V-Mini-Digital-Voltmeter-Voltage-Tester-Meter-LED-Screen-Electronic-Parts/32737103272.html?spm=a2g0s.9042311.0.0.27424c4dFqeJ8Y

**LCD Meter**

https://www.aliexpress.com/item/DC-6-5-100v-20A-LCD-Combo-Meter-Voltage-current-KWh-Watt-Panel-Meter-12v-24v/32546896962.html?spm=a2g0s.9042311.0.0.27424c4dBAPOp9

**Construction photos**

Basic box with cut-outs 

![photo%203%20holes%20cut%20out|280x373](upload://v1811xgfmI06EkGqGa7RgwJeQRc.jpeg) 

![Photo%205|375x500](upload://sWxkKFvm7hMQ88p50ieBEOen800.jpeg) 

![Photo%206|666x500](upload://i8NGZ7h6CBhHtpGTqt0OIDVWNNy.jpeg) 

![photo%207%20|375x500](upload://bBDtGMVzQoMl45kbrsrnCW80o1D.jpeg) 

![photo%208|666x500](upload://762YKaRq6tsxEOgKiYCYhF2uQY4.jpeg) 

![photo%209|666x500](upload://h7FiDBnHKLHa8HcpoLIl2TMCJ1M.jpeg) 

![photo%2010|666x500](upload://zX07av00jd01BI4UP2sgme8cBKc.jpeg) 

![photo%2011|666x500](upload://dd3ayKYfbj8C2ZW83mNdvEkI0CZ.jpeg) 

![photo%2012|666x500](upload://y4RlFd5ojD6A5nvmKMs6UhRcNda.jpeg) 

On earlier builds using DieBieMS bms , I have had a few problems with the molex balance plug pins. They are bit flimsy with no mechanical strength ( even using the correct crimping tool) so for this build I have soldered balance leads directly to bms pcb using the available tabs on the 15 ohm discharge resistors.  This needs to be completed very carefully !  . Tin the ends of the resistor first using a very hot small soldering iron tip.

![photo%2013%20direct%20to%20pcb|666x500](upload://3WY7qVGkNA9yfTxEq0p29Q8YrWp.jpeg) 

![photo%2014%20direct%20to%20pcb|666x500](upload://j9W1WavOU5t74zPeQhSfqhciy6S.jpeg) 

The charger is external and consist of a fixed 36V 11A LED strip power supply driving a CCCV module mounted on top of the power supply. The output of the CCCV module was set to 45V 5A.

![Charger%201|375x500](upload://m3d2QHY3elVMyvJHov538wCjoOr.jpeg) 

![charger%202|666x500](upload://ztmMuvjDgaGC4JmCK4iXjCKti3m.jpeg) 

The DieBieMS pcb finally arrived – it was supplied with FW 0.27 and is compatible with latest DieBieMS tool version 0.27 which has a few enhanced features from earlier versions.

The pcb was configured using the DieBieMS tool with key config settings being:

**Key settings**
![diebiems%20key%20config%20settings|690x377](upload://eDZZjwoUdQT5r9f2dGbfRwNQi9N.jpeg) 

After all wiring was complete - triple checked all wiring and did as much continuity testing as possible without power .

First power on – no magic smoke so all good.!

Connected up the 12-pin balance lead plug and 2-pin charging plug to my board ( The board pack voltage was approx. 38V) and the cell voltage displays , DieBieMS pcb sprung to life.

Connected up charger and charging current started and LCD meter showed charging current and pack voltage .
![working%20photo%201%20|375x500](upload://mwmLlA7zLxPCN9Aav537rWAQjFb.jpeg) 


With the charging current set to 4A and the BMS “Soft Overvoltage” set to 4.18V – the BMS charged and balanced the P packs to about 4.13V .  Setting the charging current down to 0.5A enables the final top-up to 4.18V . This feature is kind of handy in that a “normal” charge only charges to 4.13V which should prolong the cell life – but you can top up to 4.18V ( should you want to for a long ride) by reducing the charging current to 0.5A.

After a long charge and pack balance – the pcb discharge mosfets had no detectable temperature rise – probably due to the cell discharge sequencing function and the pulse discharge function of the bms. The external 6 ohms resistors were only very slightly warm.

Tested P pack discharge switches with BMS off and all works OK.( the switch basically shorts out the DieBieMS discharge mosfet)

So overall the external BMS build was successful and achieved objectives using the worlds best bms pcb DieBieMS.

Happy to answer any queries
```

---
## \#6 Posted by: banjaxxed Posted at: 2019-05-07T13:40:05.838Z Reads: 63

```
Thanks for this detailed guide. I really think this is future-forward

More and more we see builds being made with discharge only BMSs and given the other components it's not the $80-$110 that is the problem

Not only for the physical space reason but also because a discharge BMS gives another point of failure which ends the ride at best but at worst of course can injure if it blows when taking breaking current.

This and a rhoestatic break seems like a really good route. Plus you only need one BMS really even for multiple boards if you schedule charging time (may not work for a group).

And question: do you fellas share the single charger? How does that work?

Oh and @JTAG JIC you didn't see it
```

---
## \#7 Posted by: SkaterBoy58 Posted at: 2019-05-07T23:14:00.250Z Reads: 58

```
Yeah - I use the one BMS for both of my DIY boards - both have same 12 pin socket and charging socket.( and a few locals also use same ) 
There is no room for BMS in my DIY boards - stuffed full of cells ! - and even if these was , I would never put a BMS in the enclosure - as per your reasons above   Cheers
```

---
