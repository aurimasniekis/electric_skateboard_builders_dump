# What is the Best Voltage Meter

### Replies: 24 Views: 2921

## \#1 Posted by: SyrusB Posted at: 2017-05-25T02:04:41.251Z Reads: 383

```
Ok so I was going to get a meter and I wanted advice on what the best one is I want one with a precent instead of the Voltage. I am using Lipo batteries if that is important.
```

---
## \#2 Posted by: Jinra Posted at: 2017-05-25T02:06:31.715Z Reads: 384

```
I'd suggest you get used to reading voltage as it's much more accurate and easier to read for cell safety, but if you want a % meter this is the one I use

https://www.amazon.com/DROK-Black-light-Capacity-Automotive-Indicator/dp/B01LQ7MT4K/ref=sr_1_4?ie=UTF8&qid=1495677935&sr=8-4&keywords=battery+meter

The reason I'd recommend voltage is because these meters are programmed to display a certain % at a given voltage, but different cells have difference tolerances for how low they'll go. Typically, 18650's can go a bit lower in voltage than Lipo's before being considered "empty".
```

---
## \#3 Posted by: SyrusB Posted at: 2017-05-25T02:29:12.538Z Reads: 372

```
Ok what would you recommend for regular Voltage then
```

---
## \#4 Posted by: Okami Posted at: 2017-05-25T19:37:22.979Z Reads: 336

```
I think the one @Jinra gave you is a good one. It already has case/enclosure as not all of these have it.

You can select which voltage you need (6s / 8s / 10s etc)..

Just put it in voltage mode the first few times, to know how low can you go with your lipos.. then put it back to percentage mode to see how much % it is..

I think it should show still about 30% when u will get close to lipo pack limit.. but this is how I calculate easily the range for mine - I know how many miles/km I can do with 10% for example.. then see Ive got 50% left.. it will be this much miles etc.
```

---
## \#5 Posted by: Jinra Posted at: 2017-05-25T19:39:05.518Z Reads: 320

```
I don't think mine has a voltage mode actually.
```

---
## \#6 Posted by: Okami Posted at: 2017-05-25T19:53:03.644Z Reads: 323

```
mh maybe someone else has to reply to this then.

I know the ones similar were sold under Baiway name.

If you hold the button etc nothing else comes up @Jinra  ? So u can only choose battery system and nothing else?

Maybe u got to do it with a solder bridge or something.. really not sure..

--

anyways, he can always hook up a lipo alarm, if possible and monitor the lipo back that way or just connect the percentage display when lipo is empty so he knows what percentage is empty..
```

---
## \#7 Posted by: jess.t.moody Posted at: 2017-05-25T19:53:23.260Z Reads: 309

```
With these meters, voltage under load is ±%5 give or take a few. I used [this](http://www.ebay.com/itm/LCD-Battery-Capacity-Tester-Indicator-for-12V-Lead-acid-Lithium-LiPo-Battery-Hot-/401197295673?hash=item5d6938e839:g:ziEAAOSwopRYbRUm) one from eBay on my [Rouge Rogue](https://www.electric-skateboard.builders/t/rouge-rogue-custom-baltic-birch-deck-paris-trucks-turnigy-sk3-6s1p-ebay-motor-mount-hobbyking-x-car-beast-120a-esc-pepakura-case/23864) and it works great (would've prefered a panel mount one, though).
```

---
## \#8 Posted by: jess.t.moody Posted at: 2017-05-25T19:55:37.612Z Reads: 317

```
To set the cell count on mine, I held a button down on the back **while powering on**. I could then press the button multiple times to cycle through 1S, 2S, 3S, etc. Once you're happy with the settings, cut the power and when you turn it on again it should be good to go.
```

---
## \#9 Posted by: mmaner Posted at: 2017-05-25T20:03:34.891Z Reads: 311

```
I've tried most of the common volt meters, my favorite is the DROK DC8-63V.  Its solid as a rock, is very configurable and keeps its settings no matter what.

https://www.amazon.com/DROK-Lead-acid-Capacity-Indicator-Electric/dp/B01I30RAC4/ref=sr_1_2?ie=UTF8&qid=1495742462&sr=8-2&keywords=drok+dc8

You will also need to solder a button on to enable some of the settings.

https://www.amazon.com/gp/product/B01L95LP8K/ref=oh_aui_detailpage_o03_s00?ie=UTF8&psc=1

Its a bit larger than the others, but you wont have to open your board and put it back in V or % mode.
```

---
## \#10 Posted by: mmaner Posted at: 2017-05-25T20:51:50.774Z Reads: 297

```
...also, in case you have a difficult time finding the operating instructions for the DROK DC8-63V (like I did), here ya go.

    Instruction: 
    1) Power off the indicator 
    2) Press and hold Kdn key 
    3) Power on the indicator  
    4) Release Kdn key,then the screen will display "Pbx" or "Lix" (Pb is lead-acid; Li is lithium battery; X is the number of cells), then use ? Kup and ? Kdn to select battery types. 

    Pb1: Pb12V lead-acid battery 
    Pb2: Pb24V lead-acid battery 
    Pb3: Pb36V lead-acid battery 
    Pb4: Pb48V lead-acid battery 
    Li2: 2 pcs lithium batteries 
    Li3: 3 pcs lithium batteries 

    Li9: 9 pcs lithium batteries 
    LiA: 10 pcs lithium batteries 
    Lib: 11 pcs lithium batteries 
    LiC: 12 pcs lithium batteries 
    Lid: 13 pcs lithium batteries 
    LiE: 14 pcs lithium batteries 
    LiF: 15 pcs lithium batteries  

    FUNCTION INDICATORS

    F1: the backlight delay turn-off function; enter the low-power state (100uA) after displaying 10 seconds, the LCD displays but the backlight turns off. Press the OK key and the backlight turns off again after 10 seconds’ lighting. This mode needs the OK key.

    F2: the backlight voltage trigger function; enter the low-power state (100uA) after displaying 10 seconds, the LCD displays but the backlight turns off. When the voltage changes, the backlight automatically lights on for 10 seconds, or press the OK key and the backlight turns off again after 10 seconds’ lighting.  This mode needs the OK key.

    F3: sleep function; enter the ultra low-power state (<20uA) after displaying 10 seconds , the LCD and the backlight turns off. Press the OK key and the backlight turns off again after 10 seconds’ lighting. This mode needs the OK key.

    F4: power-on self-inspection; every time the electricity module is powered on, the LCD displays strokes for 2 seconds, and then displays the selected battery type for 1 second, finally displays the electricity capacity.

    F5: voltage display; the current battery voltage is displayed only on the right, the battery symbol on the left is still in accordance with the selected type.

    F6: the LCD shows the Logo on the lower left.

    * The F1-F3 functions need the front key, the default is without this key.
```

---
## \#11 Posted by: Randyc1 Posted at: 2017-05-26T14:47:39.665Z Reads: 276

```
<img src="/uploads/db1493/original/3X/3/c/3c4f811ca28a696467bf4187765e4a7dc98fb9ef.jpg" width="690" height="388"> small drok voltmeter.
```

---
## \#12 Posted by: MontPierre Posted at: 2017-08-09T13:01:46.000Z Reads: 235

```
Here is mine, got Drok one and attached small button as per post above to get "hidden" function of displaying voltage and percentage of the charge. 

<img src="/uploads/db1493/original/3X/8/0/808c47a0c625dad7cae0895974dc9e118988c39d.JPG" width="666" height="500">
```

---
## \#13 Posted by: SORRENTINO Posted at: 2017-08-09T13:53:12.825Z Reads: 226

```
Buy a 3 dollar bluetooth module and just run an app to see what your voltage is at :slight_smile:
```

---
## \#14 Posted by: Okami Posted at: 2017-09-01T06:28:58.874Z Reads: 210

```
To these who use these meters **with lipo batteries - Do you use lead acid  or li-ion mode?**

I believe these meters are not that good in percentage mode, when used along with lipo batteries..

Even if some people say you can get lipo till 3.0-3.3v (when it is basically completely empty),.. the recommended end of discharge is around 3.6-3.8v so Ive heard.. this would leave over 50% in percentange mode, since the meter is calibrated for li-ion batteries, which can easily reach 3.0v and still have some capacity left.
```

---
## \#15 Posted by: Jinra Posted at: 2017-09-01T06:31:02.970Z Reads: 205

```
mine reads 30% at 3.6 volts. Good enough for me as it helps me maintain a good cycle life while also knowing i can probably discharge past 0% if i really need to.
```

---
## \#16 Posted by: Okami Posted at: 2017-09-01T06:33:35.203Z Reads: 209

```
Good to know, Ive been using the meter only with li-ion so far and now when I ordered another one for a friend.. I got to conclusion he wont have it as precise as I have it for li-ion pack..

Though im not sure I get 30% at 3.6v.. which meter exactly are you using? (the one with button and with many bars, or no buttons and about 5 'bars' for the visual indicator?

Anyways.. good to hear it is 30%.. not 60% or something, was scared it wont be very useful, if it only drops 40% in whole discharge cycle.
```

---
## \#17 Posted by: Jinra Posted at: 2017-09-01T06:45:27.130Z Reads: 208

```
i use li-ion as well

https://www.amazon.com/gp/product/B01LQ7MT4K/ref=oh_aui_search_detailpage?ie=UTF8&psc=1
```

---
## \#18 Posted by: Okami Posted at: 2017-09-01T11:15:17.675Z Reads: 196

```
Thanks for info, yeh that is the one without buttons and 5 bars.. I wonder do the limits differ between them, I should check at what voltage my meter reads 30%.. I think it was about 60% at 3.7v or so.. 

If you take 3.0 as lowest and 4.2 as highest, that is 1.2 'steps'

3.6v would make it in the middle, but for lipo pack which shouldnt go much lower than 3.5v, it would need to show 50% at 3.85v per cell..

Though, I remember I have got it to about 10%.. but i dont remember anymore whenever that was 3.1-3.2v per cell or a different value, so im not sure whenever 0% is 3.0v or not.
```

---
## \#19 Posted by: MontPierre Posted at: 2017-09-01T12:47:17.477Z Reads: 189

```
Get a meter that can display percentage and Voltage - then you don't have to worry too much, you'll be able to judge capacity by voltage.
```

---
## \#20 Posted by: Mikaelj Posted at: 2017-09-04T21:02:17.977Z Reads: 177

```
Are you able to lock it in voltage mode? Mine always jumps back to percentage for some reason. And how do you set it up for lipo? I can choose 36v or 48v as 100%, but not set it to be 42v (10s) at 100%
```

---
## \#21 Posted by: Jinra Posted at: 2017-09-05T00:13:53.972Z Reads: 170

```
My setting for 10s is "10C". It doesn't display voltage though, only percent
```

---
## \#22 Posted by: mkeboard Posted at: 2017-09-07T01:21:49.935Z Reads: 154

```
Where on the circuit board did you solder the button?
```

---
## \#23 Posted by: mmaner Posted at: 2017-09-07T01:23:12.753Z Reads: 158

```
You cant miss it when you take the cover off, its just below the display where the small hole is in the cover, just make sure you've got the correct volt meter.  The half height meters only have a button on the back.

https://www.amazon.com/DROK-Lead-acid-Capacity-Indicator-Electric/dp/B01I30RAC4/ref=sr_1_2?ie=UTF8&amp;qid=1495742462&amp;sr=8-2&amp;keywords=drok+dc8
```

---
## \#24 Posted by: mkeboard Posted at: 2017-09-07T01:33:29.997Z Reads: 155

```
Cool, I didnt want to make contact between the wrong parts and blow it
```

---
