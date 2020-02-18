# DIY BMS with USB-C PD

### Replies: 14 Views: 699

## \#1 Posted by: meissnerl Posted at: 2019-05-22T12:08:10.193Z Reads: 118

```
Hi Guys.
Im currently making my electronic technician degree in Germany and I was looking for a project that I can do as my technician-project.
I was looking for a suitable BMS for my dual HUB motor setup but couldn’t find anything that fits.
So I figured, maybe I can design one by myself.

What the BMS should have:
-cell monitoring and balancing
-charge indicator 
-capability to charge with external charger
-10s LiPo (2 5S packs)
-charging via USB-C Power Delivery Prorokoll (maybe use as sink and source -> powerbank feature)
-overpower discharge resistor (if you go down hill and want to break but the batteries are fully charged you can Push a few amps trough a resistor to be able to at least break a bit longer)
-no smart connection (everything got Bluetooth but I personally didn’t want to connect everything to my phone)


I already did a test PCB with the Ti BQ7630 as Analog Frontend and the Ti TUSB422 as USB PD controller. As uC I planning to use some sort of PIC, because we use them in technician school.

Maybe you good some good ideas or suggestions to make this Projekt a success.
```

---
## \#2 Posted by: Andy87 Posted at: 2019-05-22T12:58:36.653Z Reads: 102

```
a small LED display which you can plug in via usb-c to get the actuall voltage reading of each cell easy displayed would be nice.
```

---
## \#3 Posted by: meissnerl Posted at: 2019-05-22T14:00:02.512Z Reads: 93

```
Mhhh 🤔 there are the normal USB Rx/Tx datelines besides the USB C bidirectional ones. Maybe it is possible to use them for data transmission, but I never worked with usb before... 

Or you just use these lines to transmit I2C data on it, this should work...
```

---
## \#4 Posted by: totalgeek9224 Posted at: 2019-05-22T15:10:55.846Z Reads: 73

```
If you want a good place to start in terms of BMS ideas, theres been a lot of demand for something similar to the DieBieMS but without the discharge capabilites, maybe some of the feature from that BMS could be ported here? Best of luck! Been waiting for a BMS with usb-c capabilities for a while now
```

---
## \#5 Posted by: bevilacqua Posted at: 2019-05-22T15:18:19.055Z Reads: 67

```
Can bus support
```

---
## \#6 Posted by: thisguyhere Posted at: 2019-05-22T15:25:04.715Z Reads: 63

```
i think the biggest problem with commonly found bms' is their balancing current is far too low for the types of batteries we're building.

balancing current is less than 100mA, so at this rate, balancing a large pack takes DAYS to complete.

for example, i just made a battery and greatest voltage variation between cells was 0.04.  despite this small amount of drift, it still took about 24 hours to bring everything to balance.

basically, if there's a bms that can balance at a much higher rate, let's just say 500mA, those with large batteries can expect to balance charge in a reasonable amount of time.
```

---
## \#7 Posted by: ducktaperules Posted at: 2019-05-22T15:34:19.499Z Reads: 58

```
i agree with this, small charge only bms like the DieBieMS would be great. VESC / metAR communication is great but its so big for some builds.
```

---
## \#8 Posted by: meissnerl Posted at: 2019-05-22T15:43:14.540Z Reads: 51

```
I’ve already took a look at this build but for me it is way to much for a normal esk8 build. As i said indent even want to do wireless because it schould be simple to use but quite powerful bms.
```

---
## \#9 Posted by: meissnerl Posted at: 2019-05-22T15:44:51.030Z Reads: 52

```
You have to think about transfering the Heat away from the discharge Resistors. But you are totally right, I take a look at the possibilities with the BQ7630!
```

---
## \#10 Posted by: ducktaperules Posted at: 2019-05-22T15:47:23.559Z Reads: 52

```
Whilst i think being able to charge off USB-C is useful (eg to top up at work) the reality is that its not that useful as a normal charging solution.

The USB-C PD spec supports a maximum of 100W at 20V. 

Firstly you will need to boost convert this up to a reasonable voltage to charge a 10s or 12s pack like most builders use. 

Secondly assuming this boost conversion is ~90% efficient you would get a maximum of around 1.8A charge current from a 100W charger. For a larger battery (eg. 12s4p) this would mean charge times would be somewhere around 6 hours for a full charge.

Thirdly its quite hard to find a USB-C charger that supports the 100W  power profiles. Most smaller chargers are only around 45W and most laptop chargers are only around 85W.
```

---
## \#11 Posted by: meissnerl Posted at: 2019-05-22T15:51:03.072Z Reads: 47

```
I know that only 100W is possible. And for the 100W you even need a special active cable that tells via the PD protocol that it is capable.
The USB charge is meant to be that you are still able to charge even if you have no charger with you. As I wrote, I want to still have cv/cc charging capabilities for fast charge (something around 5A). USB C should be possible up to 2A (for the stuff I read till now).
```

---
## \#12 Posted by: thisguyhere Posted at: 2019-05-22T16:00:12.627Z Reads: 49

```
[quote="meissnerl, post:9, topic:94617"]
You have to think about transfering the Heat away from the discharge Resistors
[/quote]

thought about this, but not sure how.  i can't find a heatsink small enough to fit across the row of resistors - and they do get really hot during balancing - 250f.

is there something else i can use?
```

---
## \#13 Posted by: meissnerl Posted at: 2019-05-22T16:04:02.181Z Reads: 47

```
Maybe use THT resistors they got a bigger area to do heat transfer. Or maybe it is possible to use something like a resistor array that you can mount to the case 🤔
```

---
## \#14 Posted by: meissnerl Posted at: 2019-05-23T13:14:39.388Z Reads: 38

```
What do you guys think: use a proper charging circuit like this I found on Ti’s website, or just use a simple boost converter circuit.

The problem to use the charging circuit i have to change the design to get more than .6A charging current.  http://www.ti.com/tool/PMP30157#1

In my opinion a simple circuit will do the trick, because we can easily take the voltage readings from the BQ76930 BMS front end.
```

---
