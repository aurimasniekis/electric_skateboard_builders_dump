# Adding WS2812B LED strip to a 10s4p battery pack

### Replies: 3 Views: 255

## \#1 Posted by: chickengun Posted at: 2019-03-28T19:49:19.141Z Reads: 65

```
I would like to add 60 WS2812B LEDS to a new build and I am wondering how to do that. The LED strip runs at 5 V and one LED can draw up to 60 mA (but it's more like 20 mA on avarage). My initial thought: Get a step down converter that can handle the max current drawn which is 60 mA * 60 = 3.6 A at 5 V.
So the first question is: Which one? And is it safe to solder it directly to the 10s4p battery pack? I want to use the firefly remote and I was thinking of modifying the code to put a LED on/off option to the settings menu which will set a GPIO pin (e.g. No 5) on the arduino of the firefly receiver either to HIGH or LOW which than turns on a mosfet, which powers on the LED Strip. Another Arduino is needed to control the LED strip. I draw this picture:
![image|615x500](upload://z2J6irC11wNcw716kiZ9sJFslkD.png) 

What do you think about this idea? Is it ok to do or will I burn my vesc? :smile:
```

---
## \#2 Posted by: 702vegas Posted at: 2019-03-29T00:19:29.513Z Reads: 49

```
Theres a post something like this but different addressable rgb
```

---
## \#3 Posted by: chickengun Posted at: 2019-03-29T01:13:47.410Z Reads: 44

```
After thinking about this a bit the step down converter might not be a good idea. Even if it's 85% efficient there will be still a problem of heat dissipation (1-3 Watts). Maybe I should just use four 18650 batteries in parallel for the LED strip without any voltage regulator as the ws2812b leds work between 3.6 and 5.2 V. I could charge them together with the 10s4p pack (over a tp4056 board). This way there will only be heat during charging and not when e-skating
```

---
