# Unbalanced cells? A thread about nothing

### Replies: 8 Views: 406

## \#1 Posted by: Sebike Posted at: 2018-07-10T20:16:07.667Z Reads: 143

```
So After todays ride I opened up the enclosure to monitor my cells before charging them up to full charge again. All cells read 3,47 volts measured on the BMS balance wire connector. To be able to measure the first group of cells without stripping the battery I put the negative probe on the charge port -.

I charged the battery up to 42 and re-measured the cells. 

HORROR! 

First group of cells read 3,89 v. All the others were at 4,20-4,22

Faulty cells? Time to buy new cells? Disassemble battery? Lots of work? Fire?

So, I started searching the forum and read everything I could. To no good,, cells were still at 3,89. 
Time to strip the battery. Shrink wrap, foam, fish paper, kapton.... 

Inspected nickel welds. Rock solid. Checked soldered balance wires. No problem.

So, then I measured that first group of cells again. Probe directly on nickel this time. duh

4.20! 

Phew!! Funny thing is that all parallel groups showed the same exact voltage pre-charging while measuring at the same spots - charge port and balancing connector, but post charging (while BMS was in balancing mode I guess) measuring through charge port gave a lower voltage reading on that first group of cells.
```

---
## \#2 Posted by: Sebike Posted at: 2018-07-10T20:32:20.501Z Reads: 131

```
I learned another thing today.

My cheap 42v 2A charger only provides a 1,13 A @CC to the battery. 

A bit on the slow side. :smile:
```

---
## \#3 Posted by: i2oadsweepei2 Posted at: 2018-07-10T22:18:09.018Z Reads: 102

```
That is good news. It’s good if you are a bit concerned about your batterys health whether you built it or not. I tore apart my battery after the [PSA: Be careful assembling Li-ion Battery packs](https://www.electric-skateboard.builders/t/psa-be-careful-assembling-li-ion-battery-packs/59296) thread. Thankfully all was good. The charge would be a bit slow at 1.13a. Now I want to go test my power supply 😂 👍
```

---
## \#4 Posted by: Sebike Posted at: 2018-07-10T22:25:37.886Z Reads: 93

```
Yeah. Those threads are scary. Since reading about one of those fires, I always charge my board either outside or next to me. Never overnight or unattended. 

Charger was one of those $7 off ebay. At least it doesn't put any stress the battery.. :smile:
```

---
## \#5 Posted by: pat.speed Posted at: 2018-07-10T22:42:12.785Z Reads: 84

```
May I recommend a boost converter cc/cv charger? I was looking for an adjustable charger for my 10s and 12s packs and was reading the thread about using a 60v psu and step down power supply, but 60v psu are a tad expensive. I then googled cc/cv boost converters first one that popped up was a 600w 12-80v converter for leds. I got that and a watt meter to see current and voltage and connected it up to a 12v 15amp psu I had laying around, it worked but only charged at about 1.5a, so I got out an old adjustable psu cranked it up to 24v and I now have 5a at 50v for my 12s pack. Hurray. 

Total cost ~ $30 AUD
```

---
## \#6 Posted by: Sebike Posted at: 2018-07-10T22:59:54.948Z Reads: 72

```
Nice one! GJ!

Do you have links to the parts you used?
```

---
## \#7 Posted by: pat.speed Posted at: 2018-07-10T23:06:26.721Z Reads: 72

```
These are from the Australian store but shouldn't be to hard to find on other stores



https://www.ebay.com.au/itm/Digital-LCD-Watt-Meter-Battery-Balance-Ammeter-Amp-Analyzer-60V-100A-DC-RC-Volt/221399347636?ssPageName=STRK%3AMEBIDX%3AIT&_trksid=p2057872.m2749.l2649





https://www.ebay.com.au/itm/DC-DC-600W-10-60V-to-12-80V-Boost-Converter-Step-up-Module-car-Power-Supply-AU/162286536954?epid=931031217&hash=item25c90808fa:g:1FgAAOSw9hdaMORb




This isn't from the same seller but it is the same item.
```

---
## \#8 Posted by: Okami Posted at: 2018-07-11T11:32:48.881Z Reads: 47

```
Im using this little meter to know charge power and charger is chinese one but they can seemingly adjust end voltage for your needs.

![IMG_20180618_114455|690x403](upload://gai80pHScRIK9tjPbF9FaV75Ohf.jpg)

https://m.aliexpress.com/item/32815463801.html?pid=808_0000_0131&spm=a2g0n.search-amp.list.32815463801&aff_trace_key=5dfab3dca0b14e0198b69b2b6f6eec16-1530255367831-08943-UneMJZVf&aff_short_key=UneMJZVf&aff_platform=msite

U can choose what plugs they include. Not as fancy as adjustable charger but works nicely if u need to carry it and use it as "travel" charger..

I have it set at around 41.5v, so each cell have some room for imbalance but i usually dont charge higher than 4.15v anyways
```

---
