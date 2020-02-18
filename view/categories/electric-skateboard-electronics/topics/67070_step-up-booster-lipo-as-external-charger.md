# Step up Booster + Lipo as external charger

### Replies: 11 Views: 614

## \#1 Posted by: Schulerbible Posted at: 2018-09-05T05:30:22.005Z Reads: 101

```
Hi guys,

We are currently fiddle with a step-up boost converter trying to use a 6s lipo to charge any 10s board at about 4A. My electronics skillz are a bit rusty and I haven't found much about the converter online. It has three potentiometers, one at the input, one in the middle to somewhat limit the current, and one at the output to set the output voltage.

https://www.ebay.com.au/i/183141137924?chn=ps

![image|500x500](upload://1A6FXbHRrGShuv5O3rjlzmoVOeW.jpg)

Anyone here knows how to measure and set the current limit? I did think about using a power resistor at the output to simulate a load and adjust the current accordingly? Would that work or :fire::fire::fire:? 

Cheers

![image|663x500](upload://xLhzserq3vLLFEPJ16zcxFXLoT3.jpg)
```

---
## \#2 Posted by: pat.speed Posted at: 2018-09-05T06:03:08.708Z Reads: 85

```
The way I set mine was to have a watt meter connected to the output, then I plugged in my board and adjusted it to 4a
```

---
## \#3 Posted by: Schulerbible Posted at: 2018-09-05T06:09:52.789Z Reads: 80

```
Well that's what I wanted to avoid. Since the Lipo can output a lot of amps and the step up supplies up to 1200W  it could happen that I charge the cells at way more than 4A until I got the right value dialed in. Sure it's just a matter of seconds until I've adjusted the right value on the trimmer but I am not sure if this is good for the cells ...
```

---
## \#4 Posted by: pat.speed Posted at: 2018-09-05T06:14:39.909Z Reads: 81

```
Mine could do 600w but when I first started it, it was set to 1a. Another option might be to first set it up with power supply, that way you can limit the input amps. 

Your calculations above look to be correct although you need to assume an efficiency of about 70-80%
```

---
## \#5 Posted by: Schulerbible Posted at: 2018-09-05T06:15:35.464Z Reads: 77

```
Thanks, yeah true.
```

---
## \#6 Posted by: dareno Posted at: 2018-09-07T00:34:06.854Z Reads: 59

```
@TinnieSinker isn't this what you are working on?
```

---
## \#7 Posted by: TinnieSinker Posted at: 2018-09-07T02:01:19.617Z Reads: 56

```
Thanks @dareno i was wondering if there was a thread about it yet. i've had success charging with a boost converter.

used a watt meter to set the amps and volts (although i found the volts were out by .5 with the multimeter). To start with i turned the amps all the way down, then adjusted up to where i wanted, about 5-6a. but it went all the way up to 10a!

old mate who commissioned a power box from me bought a 4s by mistake and i've concluded that 4s is not enough. it could only charge at 2a, no where near fast enough and only 40% efficiency

I've done bench tests with a small 6s pack, a 2200mah. at 5-6a i got 2000mah into my board, which is fine by me

the parts I have used:

https://www.ebay.com.au/itm/DC-DC-600W-10-60V-to-12-80V-Boost-Converter-Step-up-Module-car-Power-Supply-AU/162286536954?ssPageName=STRK%3AMEBIDX%3AIT&_trksid=p2060353.m2749.l2649

https://www.ebay.com.au/itm/XH-M609-12-36V-Battery-Low-Voltage-Disconnect-Protection-Module-DC-Output/142707891539?ssPageName=STRK%3AMEBIDX%3AIT&_trksid=p2060353.m2749.l2649

https://www.ebay.com.au/itm/150A-DC-Combo-Digital-LCD-Volt-Amp-Watt-Meter-Power-Analyzer-Pro-Battery-Tester/302698855211?ssPageName=STRK%3AMEBIDX%3AIT&_trksid=p2060353.m2749.l2649
```

---
## \#8 Posted by: SkaterBoy58 Posted at: 2018-09-07T04:10:32.907Z Reads: 46

```
@Schulerbible  I currently run one of these boost converters as a portable step-up booster for charging 10S board. Your basic power and current calculations are correct . 

Best way to set the booster module up is

* With a voltmeter only connected to output - adjust output voltage adjust pot to give 42V output

* Turn the A -ADJ pot ( Output current ) all the way counter-clockwise ( up to 30 turns) . This is setting to minimum current (0A)

* Connect an in-line wattmeter or ammeter to booster module output

* Connect board charging socket to wattmeter output and then adjust A-ADJ pot to desired current setting

Attached is some basic technical data from Sellers

![20180907121118414_0001|690x487](upload://g0afvNcvgrfCrdeGgpFD46UWBQv.jpg)![20180907121118414_0004|690x487](upload://38qb0v7b7W6OQWDRAXGQsq1Oz3X.jpg)![20180907121118414_0003|690x487](upload://6m0ZiokVHOt1pGbLWoQHma9EIya.jpg)![20180907121118414_0002|690x487](upload://rfDYBa38I75QPlf43VQKdKhCq0g.jpg)
```

---
## \#9 Posted by: Schulerbible Posted at: 2018-09-07T04:30:18.694Z Reads: 42

```
Thanks, I did step one already, tuning the output voltage. However, I do not have a wattmeter. I have just a couple of amp/voltage meters around, hence using the power resistor load. Thanks for the tip with the poti!
```

---
## \#10 Posted by: SkaterBoy58 Posted at: 2018-09-07T04:48:56.177Z Reads: 41

```
For your load resistor - I have used a 100W 8 ohm wirewound resistor and mounted it over a fan before and it works fine continuously for several hours( for battery discharge testing) Draws about 4-5A

 ![62B88702-3768-48F3-95C5-77292EF8AE96|666x500](upload://bAlCuNYn1bVAz0nux8ae4ilrYrV.jpeg)
```

---
## \#11 Posted by: Schulerbible Posted at: 2018-09-07T05:16:48.173Z Reads: 36

```
Ha, I am using this. a 10 Ohm variable resistor, does up to 8A.

![image|690x388](upload://hiXPuLfONU6dZhv0bsPR6KgxBFC.png)
```

---
