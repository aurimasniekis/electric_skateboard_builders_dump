# Modular 10S3P &#124; 9Ah flexible battery &#124; 6374 single motor &#124; VESC 4.12 build. Energus PS

### Replies: 19 Views: 1534

## \#1 Posted by: EnergusPS Posted at: 2018-09-25T09:40:14.105Z Reads: 251

```
Hello Builders, my name is Konstantin and I work at Energus PS. This is our introduction to the community and I will be representing Energus PS here so please adress all questions to me directly. Or by Email: sales2@energusps.com 
![2|478x499](upload://opVCubpYGfBcYDbVMBW4Ek73H8N.jpeg) 
We are a small European company(Lithuania) specializing in production of a modular  18650 cell type pack solution. The modules were initially designed for **Formula Student Electric** (www.formulastudent.de/teams/fse/)(The University of Melbourne, MUR Motorsports. Lancaster University, Lancaster formula students engineers. University of Canterbury, ucmotorsport. Swinburne University of Technology, team swinburne. E-AGLE Trento Racing Team ASD, unitn, DE MONTFORT UNIVERSITY. Wisconsin Racing Formula SAE. Bern Formula Student. Private Hochschule für Wirtschaft und Technik gGmbH. Technical University Ilmenau. University of Wollongong. Virginia Tech. Princeton Racing Electric. Institut Maschinenbau. University of Connecticut. Dartmouth Formula Racing. University of California- Irvine. University of California, Santa Cruz. INSTITUTO POLITÉCNICO DE LISBOA, ISEL Formula Student. Drexel university. University of Ontario Institute of Technology. University of Vermont. Milwaukee School of Engineering. Auburn University. University of British Columbia. Kait Racing Kanagawa Institute of Technology. University of Twente.)

With this **Demo Build** we want to introduce our Battery Modules to the eSk8 community.
![6|666x500](upload://ejOWkxggXx3mhjMRNbnN3iOsn4a.jpeg) 
**The Pack:**
![3|666x500](upload://ud2HJgElQrz35wbUMrdVxtuYMgT.jpeg) 
![5|666x500](upload://wcMmr9r9F8rHeN6bAH21tuwxrCA.jpeg) 
10S3P configuration was chosen as a perfect fit for 12S2P BATTERY ENCLOSURE V2 purchased online.
Samsung 30Q cells were chosen as most popular  eSk8 cells.
3mm rubber sheet was glued to the bottom of the enclosure for cell protection and vibration isolation.
4 side cuts on the enclosure allowed it to become flexible enough to match the Dec flex.
12AWG wire connections between the modules for flexibility

**The Module:**
![1|666x500](upload://bNd1m1oaD669WSHXQOIdjfpEntT.jpeg) 
    • Low weight: 267 Wh per kg
    • Individually fuse-protected cells, no parallel fusing is required
    • Ultra low self-discharge
    • No initial balancing required
    • Rapid prototyping of battery pack
    • Convenient thermal control
    • Built from genuine SAMSUNG 30Q cells
    • Low flammability: UL 94 V-0 rated
    • Analogue, 2-wire, 2-point temperature sensor
    • Nominal capacity: 12.4 Ah / 44.6 Wh
    • Nominal voltage: 3.60 V (2.50-4.20 V)
    • Volume: 0.122 liter
    • Weight: 174 g

**The BMS:**
![4|475x500](upload://s1EXXVDKOSCpx9WAe7YoXLONrGX.jpeg) 
In-house developed “Tiny BMS s516 – 150A/750A”

Features:
    • Android APP
    • Very small dimensions.
    • Flexibility: 4 to 16 cells of any kind, including Li-ion, LiPo, LiFePO4, Li-Titanate and Li-sulfur chemistries
    • Current measurement and SOC calculation.
    • Firmware updates, new feature releases and improvements for free.
    • Bluetooth connection (good for USB replacement).
    • Event logs and live data view: easy to debug the system, check what happened and when.
    • External contactor support for charger and load.
    • External current sensor support up to 750A.
    • Faster balancing due to "early balancing", which saves charging time.
    • Ignition/enable input. BMS will switch off the output and go to low power mode when no signal on certain pin (if enabled).
    • Temperature measurement in multiple points of the battery - for safety, to prevent overheating and charging in cold.

Specifications:
    • Series cells: 4 to 16
    • Cell voltage: 0.80 to 4.50 V
    • Cell balancing: 150 mA, dissipative
    • Discharge/Regen current peak: 150 A**
    • Discharge/Regen current sustained: 60 A**
    • Charge current peak: 100 A**
    • Charge current sustained: 30 A**
    • Discharge/Charge/Regen current: 750 A*
    • Interface: UART (USB / Bluetooth / CAN)
    • Up to 64 channel temperature sensors (available in Energus Cell Modules)

**The ESC:**

Generic VESC 4.12 

**The Motor:**

6374 sensored outrunner
![7|666x500](upload://quQIydqjiCFeLLtHXYODwYDOdn5.jpeg) 
The system is performing very well and is undergoing daily tests at our office :) Please ask what kind of stats would be of interest to you!

And please visit our website: www.energusps.com
```

---
## \#2 Posted by: Wraith Posted at: 2018-09-25T09:56:50.860Z Reads: 212

```
Is it limited to 3P only or can this be expanded further? Also would it be compatible with 21700 and larger cells later on in future releases?
```

---
## \#3 Posted by: EnergusPS Posted at: 2018-09-25T10:01:46.690Z Reads: 214

```
Hi Wraith, we produce different modules with any brand of cells as long as they are 18650. There are single and double row variants with up to 20 cells in one module. You can take a look yourself https://www.energusps.com/shop/category/li-ion-modules-3
```

---
## \#4 Posted by: Moros Posted at: 2018-09-25T10:32:02.060Z Reads: 208

```
Looks like an interesting design and I like how it offers fusing and has a good focus on safety.

Because everything is modular based I just want to make sure I am getting everything right.

So [this](https://www.energusps.com/shop/product/li1x4p25rt-li-ion-building-block-with-temp-sensor-3-6v-10ah-18c-139) is a single 4p pack for Samsung 25R and costs €51 each +VAT?
To make a 10S4P pack I would need 10 of the packs?

10 pack coming to a total of €550 + €116.50 VAT and €45 shipping.
That is **€674.55** for a 10s4p pack of 25R.
That is without even adding in a BMS, wiring, charging port and then I would still need to bolt it together and wire everything up.

Just as a pure example, I looked at [eskating.eu](https://eskating.eu/product/10s4p-eskating-electric-skateboard-battery-samsung-30q/) for a 10s4p pack to compare prices.

A complete pack, with the more popular 30Q, a well known and commonly recommended BMS, charge port, volt meter, power switch and 2amp charger for €450.

That is €180 cheaper with better cells, bms, connectors, charger and ready to go.  Once all that is added in to the price of your module the price gap will be even bigger.

So what exactly does your product offer over other options that are substantially cheaper and come complete and ready to go?
```

---
## \#5 Posted by: EnergusPS Posted at: 2018-09-25T10:54:26.852Z Reads: 182

```
Hello Moros,

Yes our modules are pricey, but that's because:

Individually fuse-protected cells, no parallel fusing is required.

Copper busbars (no nickel plates used).
.
3 temperature sensors integrated into each module.

To achieve this, a very different manufacturing process is required then spot-welding nickel  stripes. We never intend to compete with soft-packs.

Changing a cell to 30Q or any other cell will only change the module price to the delta of cell prices(witch are widely known)

We do understand that our modules are an overkill for most eSk8 builders as it was designed for electric racing to be stacked in hundreds of modules for huge packs. But I'm sure there will always be someone interested in "top of the line"
```

---
## \#6 Posted by: Moros Posted at: 2018-09-25T11:03:40.429Z Reads: 162

```
[quote="EnergusPS, post:5, topic:69153"]
Individually fuse-protected cells, no parallel fusing is required.
[/quote]


What happens if a fuse is to blow? Does the whole pack need to be replaced?
Also what happens if someone buys a pack and wants to change out the old cells to a new better cell that might become available at a later date.  Are they able to retain and reuse the modules with the new cell?
```

---
## \#7 Posted by: brenternet Posted at: 2018-09-25T11:22:25.770Z Reads: 154

```
You guys are making safety leaps, you'll get asked a lot of direct and mostly relevant questions here, as is the case with most passionate communities. Please don't be scared off by some of the more... outspoken... members.

Pricing and size aside the principle is excellent.
```

---
## \#8 Posted by: EnergusPS Posted at: 2018-09-25T11:38:47.914Z Reads: 149

```
If one fuse is to blow one cell will be disconnected from the circuit and remaining cells in the module will share the load of disconnected cell. So you can continue to use the pack but one module will have larger load per cell than other modules. It is recommended to replace that module.

The cells in the module are not interchangeable. So no you can not swap them for new ones. A new module will have to be manufactured.
```

---
## \#9 Posted by: brenternet Posted at: 2018-09-25T12:16:12.417Z Reads: 145

```
Both of these things give concern.

In an ideal world, personally, I'd like the pack to stop working if a cell dropped. I'd rather walk than take the risk of two or more going at once, no matter how rare.

Secondly in an ideal world these would be reusable. Battery technology is constantly moving.
```

---
## \#10 Posted by: EnergusPS Posted at: 2018-09-25T12:28:28.703Z Reads: 141

```
Actually there is little sense in disabling  the pack after one cell drops:
The module will remain damaged 
If remaining cells will start to overheat temp sensors in the module will signal the BMS to turn off the pack
The other modules are not affected at all
You can safely get home!
```

---
## \#11 Posted by: Andy87 Posted at: 2018-09-25T13:05:45.850Z Reads: 136

```
If you anyhow need to change the full pack if only one cell fuse out, I think it's not a big deal if it’s not totally shut down.
If it would be possible to change single cells than, yes please, no more stress for the other cells in the pack.
I would also more likely see an option where I can interchange the cells by my own.
Maybe one day I want to go from 25r to vtc6a.
In this case it would be great to just swap the cells
```

---
## \#12 Posted by: EnergusPS Posted at: 2018-09-25T13:14:06.071Z Reads: 131

```
This Pack consists of 10 modules each module of 3 cells. 
If one cell fuses out only 1 of 10 modules will be damaged but operational.
Remaining 9 modules will remain intact.
So you can disconnect 1 module and continue to use 9S(module) pack without any repairs!
```

---
## \#13 Posted by: EnergusPS Posted at: 2018-09-26T09:45:44.426Z Reads: 109

```
Ok so @Wraith asked about a double row modules:
2x3P(6P module) dimensions are  : 65mm x 38mm x 70mm
![20180926_115602|690x388](upload://s6Qc1dqURclGpkPkTkQSGRs4Ggx.jpeg) ![20180926_115616|690x388](upload://r3i55ULQfqXQszjw66EgL8ftphE.jpeg) ![20180926_115644|690x388](upload://98KZ9LcyKLs03rbrLb9P38zYJ6f.jpeg)
```

---
## \#14 Posted by: Andy87 Posted at: 2018-09-26T09:47:49.519Z Reads: 108

```
is there the negative side exposed? or just the plastic cover missing on the pictures?
```

---
## \#15 Posted by: EnergusPS Posted at: 2018-09-26T09:50:17.542Z Reads: 107

```
Just the plastic cover missing to show the copper bus bar...
```

---
## \#16 Posted by: wcoolnet Posted at: 2019-07-04T17:25:25.489Z Reads: 53

```
@EnergusPS When shipping to the USA do you have a minimum order quantity for battery modules when ordering with a TinyBMS?
```

---
## \#17 Posted by: EnergusPS Posted at: 2019-07-05T11:46:57.335Z Reads: 50

```
Sure, no problems.please contact sales.
```

---
## \#18 Posted by: wcoolnet Posted at: 2019-07-06T01:36:43.241Z Reads: 45

```
@EnergusPS Last year when I talked to sales I was told there is a minimum order quantity of 20 battery modules. So I was a bit surprised to see that you were trying to market to the electric skateboard community with your sample board only having 10 modules.
```

---
## \#19 Posted by: EnergusPS Posted at: 2019-07-06T05:33:05.236Z Reads: 43

```
Not sure what happened, the account was managed by another sales rep. We now have a samples program and can offer small quantities. Also there are some options to get a discount, so feel free to discuss it as well.
```

---
