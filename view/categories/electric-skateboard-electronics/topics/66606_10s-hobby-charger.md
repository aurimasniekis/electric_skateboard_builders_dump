# 10S Hobby Charger?

### Replies: 7 Views: 509

## \#1 Posted by: michaelcpg Posted at: 2018-08-31T01:33:25.914Z Reads: 92

```
Anyone know of any good 10S hobby chargers out there?

I have a 10S9P pack with no BMS that I currently charge with a 4A dumb charger. Ideally I want something that will allow me to adjust the voltage so I can cutoff the charge at 41V and potentially allow me to balance charge in the future if need be.

I've got another 12A dumb charger which had the voltage cutoff set to 41V but it's recently started having issues that sound similar what a few others on the forum have apparently had after adjusting the voltage.

Obviously one option would be to get another high current dumb charger and then install a BMS with a programmable voltage cutoff but I would prefer just to have an all in one, fully external charging solution, particularly seeing as a hobby charger is likely to be more useful for other potential future projects...
```

---
## \#2 Posted by: deucesdown Posted at: 2018-08-31T02:32:07.051Z Reads: 79

```
I think evpeak a9 is the only one right now. Oh and maybe the Chargery one.

There are multipin waterproof connectors, so you can bring the balance leads out.
```

---
## \#3 Posted by: Narnash Posted at: 2018-08-31T10:00:05.064Z Reads: 63

```
Junsi iCharger 1010B+ (max. 10A)  or 3010B (max. 30A)

I have the 3010B it works very nicely with my 24V Server psu (2x Dell AA23300) but mind you that combo isn't the quietest (use 2x HP DPS-600PB these are quieter as a high amp DC source).

I charge my 10S 24Ah pack easily in around 90 minutes, balanced to 41,5V. The hobby charger itself is neither super silent but basicly any hobby charger has a audible fan from my experience (it's quieter than my Turnigy Reakto 300W I had before though).


EDIT: The accesories included with the Junsi are kinda limited, you need an extra adapter pcb if you want to charge anything different than 10S (or direct adapter cables that can plug into the 11 pin) a longer balance cable (or parallel balance cable) might also be quiet handy.
```

---
## \#4 Posted by: michaelcpg Posted at: 2018-08-31T10:30:00.855Z Reads: 51

```
This is what I was initially looking at until I realised that you need a separate AC to DC PSU to power it... :(
```

---
## \#5 Posted by: briman05 Posted at: 2018-08-31T11:05:00.024Z Reads: 48

```
I have the Luna cycle advance charger you can set to 100% 90% or 80% charge.
```

---
## \#6 Posted by: xilw3r Posted at: 2018-08-31T11:06:26.667Z Reads: 49

```
I am using this, powered by an old atx psu. (might not be the same listing)
https://www.aliexpress.com/item/900W-Digital-Control-DC-DC-Boost-Module-great-Step-up-Converter-Power-Supply-Module-CC-CV/32712692639.html?spm=2114.search0104.3.1.26845db0NBvxkX&ws_ab_test=searchweb0_0,searchweb201602_2_5910017_10065_10068_5723115_5890017_5723715_5723815_10696_5723215_5723415_10084_10083_5722215_5724017_5724317_10618_10307_10820_10821_10303_10302_5970017_5723315_5723615_5724117_5724217_5722315_10059_5723015_5722115_100031_5723915_5725017_5725117_5980017_5724917_10103_5990017_5722415,searchweb201603_16,ppcSwitch_5&algo_expid=0ed34348-c495-4c8d-a940-c9d80fc5a83b-0&algo_pvid=0ed34348-c495-4c8d-a940-c9d80fc5a83b&priceBeautifyAB=0

pros: cheap, configurable voltage and current for basically any pack
cons: loud and annoying high pitched whine, not a hobby charger, so no balance leads and all that
```

---
## \#7 Posted by: Narnash Posted at: 2018-08-31T12:54:21.680Z Reads: 38

```
Most -if not all- big hobby/LiPo/LiIon Charger need a DC power source, in the RC scene it's very common to use modificated used server PSUs because they are cheap, reliable and power efficient. 
It is also very common to "stack" 2 or even 3 12V server PSU to achieve higher voltages (most hobby chargers need a higher voltage than 12V to charge faster than 5A)

On Ebay you can find dozens of used server PSUs for very cheap (arround 15-25€ each/ ~30$). They are used but get cycled out every few years by companies when they upgrade . I personally recommend the HP DPS-600PB it's a quiet, kinda compact unit and has a decent 575W output. My Dell AA23300 is also a an option but kinda long (around 33 cm) they were very cheap I got both with shipping for 18€.

To use 2 switching power supplies in siries you need to have on one of the PSUs the **DC output** ungrounded and not connected to the case! The AC side remains grounded and untoched (safe). 
After that you can connect them in series, to get your 24V, 36V ... . The overcurrent and shortcircuit protection is still intact and in the end you have a cheap high wattage 24V power supply.
```

---
