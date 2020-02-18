# LED Display - Help needed

### Replies: 17 Views: 466

## \#1 Posted by: barajabali Posted at: 2018-06-30T14:28:10.193Z Reads: 148

```
I’m looking to make a “boosted style” LED display for my board. I want 5-6 LEDs on the display and it needs to run 12s. Happy to pay you for your service! Shoot me a pm
```

---
## \#2 Posted by: trancejunkiexxl Posted at: 2018-06-30T14:35:35.113Z Reads: 149

```
i really like the one @ervinelin has on his build. is only 3 lights tho :grin:
```

---
## \#3 Posted by: Pedrodemio Posted at: 2018-06-30T14:53:19.962Z Reads: 141

```
I made one for my board, but it’s not universal since it gets the voltage reading from the VESC via UART using an arduino, but can be easily changed to read the voltage from a resistor divider

I don’t know if it wold be to bulk to integrate inside a battery

I can send you the code it you want ![image|666x500](upload://k0a92RaCw68jiDRU69cYlntNnFw.jpeg)
```

---
## \#4 Posted by: barajabali Posted at: 2018-06-30T14:57:50.522Z Reads: 132

```
That is very interesting. I don’t know very much about coding so I don’t know how much I’d benefit from it. Thanks for the offer though :) I’m ideally looking for a plug and play solution.
```

---
## \#5 Posted by: barajabali Posted at: 2018-06-30T14:58:48.654Z Reads: 122

```
@ervinelin. Did you make that yourself?
```

---
## \#6 Posted by: Pedrodemio Posted at: 2018-06-30T15:06:39.029Z Reads: 123

```
Plug and play I haven’t seen one, you could have a module made for you, just the 5 leds, a voltage regulator and a small micro controller and have some one assemble for you, I’m a bit far away and shipping would kill the price

I just don’t know if it would be cost effective. How much do you pay for the modules you currently use on your battery’s?
```

---
## \#7 Posted by: barajabali Posted at: 2018-06-30T15:13:43.322Z Reads: 121

```
Well now I pay only a couple dollars but I’d happily buy a higher quantity from you to make the shipping more worth it. 

Could you make it work for both 12 and 13s?
```

---
## \#8 Posted by: Pedrodemio Posted at: 2018-06-30T15:17:33.405Z Reads: 121

```
With the assembly it will really be hard for due to lack of time, but if no one comes up with a batter idea I can see if I can come up with something in a week or two since I’m right in the middle of finals

I’m thinking in even using a arduino and make a shield for it, I think it would be simpler and drop the cost a bit
```

---
## \#9 Posted by: barajabali Posted at: 2018-06-30T15:28:33.252Z Reads: 113

```
I could handle assembly if it’s not too difficult. Let me know! Good luck
```

---
## \#10 Posted by: barajabali Posted at: 2018-06-30T15:42:00.176Z Reads: 108

```
If someone could design this and test it. I’d be happy to pay for the Service and BOM.
```

---
## \#11 Posted by: BoostedBuilder Posted at: 2018-06-30T16:34:20.241Z Reads: 93

```
[This could potentially be interesting for you!](http://bestechpower.com/fuelgasgauge/PCB-D142.html)
```

---
## \#12 Posted by: barajabali Posted at: 2018-06-30T16:35:13.432Z Reads: 88

```
Thanks for that, I have seen it and it is just a bit too ugly. :/ maybe I’ll buy and try to gut it
```

---
## \#13 Posted by: Mich21050 Posted at: 2018-06-30T17:14:24.200Z Reads: 89

```
What about the led indicator @Martinsp sells in his shop? :smile:
```

---
## \#14 Posted by: BoostedBuilder Posted at: 2018-06-30T17:18:08.836Z Reads: 88

```
It has 10 LED's, not 5. Won't work properly.

You might also get this Meepo one, and gut it. I think the internals are very small and simple.

![image|180x250](upload://zKyM3Gzq71h70OxZNM2F3IJ2Eoa.jpg)
```

---
## \#15 Posted by: barajabali Posted at: 2018-06-30T17:18:32.726Z Reads: 88

```
I didn’t know about that one. Seems promising, too many lights for my liking but a good option. Thanks
```

---
## \#16 Posted by: ervinelin Posted at: 2018-07-01T00:51:05.263Z Reads: 69

```
Nope I bought them off the shelf
```

---
## \#17 Posted by: Exigent Posted at: 2018-07-02T01:40:20.047Z Reads: 45

```
If you want one that reads the voltage directly from the battery pack, there are kits out there that offer up to 7 LEDs (You don't have to use them all). You can select one LED at a time or LEDs successively light up (or turn off) as the voltage changes. You control the set points for voltages. A kit costs abour $8 if I remember correctly but you'd want brighter LEDs.

No Aduino or other microcomputer required. Based on two LM324 chips.
You can also "roll your own" from scratch if desired. Assuming the batteries are kept more or less balanced, you also don't have to measure the full voltage of the pack to get an idea of the overall percentage used. You could for example, just monitor the voltage over half the cells in a pack. You'd tap the cells at a voltage point so that the input never exceeds the rated maximum for the respective circuit used.

Example circuit:
http://www.circuitdiagram.org/8-led-battery-monitor-using-lm324.html

Here's another one using just a single LM3914. 
https://www.electronicshub.org/battery-level-indicator/
```

---
