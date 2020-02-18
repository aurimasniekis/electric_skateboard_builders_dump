# Vesc temperature?

### Replies: 15 Views: 1078

## \#1 Posted by: nikoli280 Posted at: 2018-04-20T15:07:09.458Z Reads: 168

```
Hi everyone. I was wondering. What kind of temperatures do you see on your vesc when using. I have a single vesc and a 192kv motor in a 10s setup and I got on a 5km ride uphill with a max power draw of 900w and speed around 30km/h a temp of 75C which I think is a bit high. Do you guys fix with heatsinks or?
```

---
## \#2 Posted by: onepunchboard Posted at: 2018-04-20T17:09:36.661Z Reads: 159

```
somethings wrong there 75 is not good. i pull 90amp, it should be warm not hot
```

---
## \#3 Posted by: nikoli280 Posted at: 2018-04-20T17:43:40.196Z Reads: 155

```
Yes it does not seem right. what can make them so hot.
```

---
## \#4 Posted by: onepunchboard Posted at: 2018-04-20T18:02:08.945Z Reads: 153

```
did you open vesc and pill off the sticker on mosfet? recent vesc has some qc problem with plastic btw fet and heat paste
```

---
## \#5 Posted by: rey8801 Posted at: 2018-04-20T18:08:32.122Z Reads: 146

```
I thought that only focbox has that sticker problem. To me the over temperature has to be Research in bad soldering and long wiring. Wrong setting. Defect product. If you are heavy then go dual and heat sink. I am de a really basic one and maybe it doesn't do that much but I run dual hub motors and with 15 minutes ride between 900w to 1400w the temperature went up to 40 °C at most. Dual really helps
```

---
## \#6 Posted by: nikoli280 Posted at: 2018-04-20T20:55:46.205Z Reads: 136

```
I now attached some heat sinks to the FEts. But i still dont get why get got so hot
```

---
## \#7 Posted by: bevilacqua Posted at: 2018-04-20T20:57:43.718Z Reads: 131

```
It should be normal on a high kv single setup without cooling (on a Uphill)
```

---
## \#8 Posted by: TeslaAlex Posted at: 2018-07-11T07:01:44.744Z Reads: 107

```
I’m a bit worried about my focbox recent temperatures. Riding up hills makes it heat up to about 80-90C. Is this a big problem? :grimacing:
```

---
## \#9 Posted by: telnoi Posted at: 2018-07-11T10:04:09.608Z Reads: 100

```
If you haven't messed with the cut-off temperature and are using the latest firmware, you should be fine. The firmware will slow down your board if the temp becomes too high.
```

---
## \#10 Posted by: TeslaAlex Posted at: 2018-07-11T10:45:24.440Z Reads: 87

```
Ok, I have experienced the board slowing down when riding up hills. I’m considering making an additional heat sink of 10mm aluminium to put under the focbox with thermal paste. What do you think? :thinking:
```

---
## \#11 Posted by: Benjamin899 Posted at: 2018-07-11T11:07:37.450Z Reads: 85

```
there are some thread about heatsinking.
```

---
## \#12 Posted by: TeslaAlex Posted at: 2018-07-11T11:43:03.198Z Reads: 78

```
Yea, I have read most of them but can’t find any heatsink to buy locally, so I wondered if simple massive aluminium would improve the cooling.
```

---
## \#13 Posted by: Benjamin899 Posted at: 2018-07-11T11:54:39.798Z Reads: 75

```
well that topic was talked about there but i can summerize it. 
Bigger heatsink acts like a reservoir for heat, so if you have no active cooling, like airflow on some cooling fins, it will have problems dissipating heat to the environment. 
You could implement the cooling mehtod of cpu/laptop cooler.
My idea was to connect these hollow copper pipes, filled with some gas, lead them out of the enclosure and connect them to some aluminum fins.
```

---
## \#14 Posted by: TeslaAlex Posted at: 2018-07-11T13:22:43.834Z Reads: 71

```
I just found an aluminium heatsink with fins on eBay. I’ll drill holes to be able to screw the focbox to it. I’ll then cut a hole in my enclosure and epoxy the heatsink in place. This way, the heatsink is constantly cooled down by the wind. Sound good? :wink:
```

---
## \#15 Posted by: Benjamin899 Posted at: 2018-07-11T14:04:56.008Z Reads: 63

```
sure just be sure that it is airtight
```

---
