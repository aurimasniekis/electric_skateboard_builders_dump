# What&rsquo;s the best on/off button and battery indicator for 10s?

### Replies: 29 Views: 3269

## \#1 Posted by: shunpo Posted at: 2016-09-22T09:11:58.334Z Reads: 357

```
As I've mentioned before, I'm building a 10s4p pack. I wan't to have a on/off button that's nice and simple, preferably a button you push down on, instead of a flip switch sort of thing. And a battery indicator too, just simple as well, either a battery icon or just the % number would be great. 

Thanks.
```

---
## \#2 Posted by: DeathCookies Posted at: 2016-09-22T09:14:10.965Z Reads: 359

```
[quote="shunpo, post:1, topic:9974"]
I'm building a 10s4p pack.
[/quote]

Because you are building the pack yourself i want to mention that i am selling vedder anti spark switch kits otherwise i would not bother you with it;)
```

---
## \#3 Posted by: Airmacx Posted at: 2016-09-22T09:16:28.615Z Reads: 352

```
Oh cool, I was looking for one of the power buttons too, do you have a site? Do you ship to Australia?
```

---
## \#4 Posted by: lox897 Posted at: 2016-09-22T09:39:04.343Z Reads: 348

```
I would go with the Vedder Anti-spark switch as well as these two:

http://www.ebay.com/itm/2016-Battery-Capacity-Tester-Indicator-for-12V-24v-36v-48v-CAR-Lead-acid-lithium-/172143986261?hash=item281494c655:g:BiAAAOSwJQdW8m~D

http://www.ebay.com.au/itm/16mm-12V-Blue-Ring-LED-Light-Stainless-Locking-Pushbutton-Switch-NO-NC-/172311068456?hash=item281e8a3f28:g:16oAAOSwV0RXtemW
```

---
## \#5 Posted by: DeathCookies Posted at: 2016-09-22T09:39:18.807Z Reads: 340

```
@shunpo I am really sorry for hijacking your thread :frowning:
[This is my sale thread](http://www.electric-skateboard.builders/t/vedder-anti-spark-switch-v1-3-kit/9949)
```

---
## \#6 Posted by: shunpo Posted at: 2016-09-22T12:51:23.913Z Reads: 325

```
No worries :)
```

---
## \#7 Posted by: shunpo Posted at: 2016-09-22T12:52:24.281Z Reads: 317

```
Which button do I select? There's a bunch of options you can choose, which ones the right one? Have you had any experience with it as well?
```

---
## \#8 Posted by: Airmacx Posted at: 2016-09-22T13:01:38.546Z Reads: 307

```
Do you know of any good eBay power buttons? I've seen a lot of them when searching, but not sure if any of them are good or compatible.
```

---
## \#9 Posted by: DeathCookies Posted at: 2016-09-22T13:02:55.589Z Reads: 293

```
For the Vedder Switch you will need a STDP switch!
```

---
## \#10 Posted by: elkick Posted at: 2016-09-22T13:12:52.507Z Reads: 284

```
It's SPDT (Single Pole Dual Throw). :wink:
```

---
## \#11 Posted by: shunpo Posted at: 2016-09-22T13:15:48.035Z Reads: 285

```
Alright. What about the one @lox897 mentioned? I really like the button, rather than the switch, will I need the Vedder thing then? Or is the one he linked plug and play sorta?
```

---
## \#12 Posted by: laikiux Posted at: 2016-09-22T13:24:50.767Z Reads: 279

```
Hello, I have one question about battery indicators. I'm running 10s. Does this batt indicator set automaticaly, or it need to be programmed? I want 0% on 30V and 100% on 42v
```

---
## \#13 Posted by: kampfhahn Posted at: 2016-09-22T13:35:56.396Z Reads: 275

```
You only can set the number of cells you are using and the indicator will use the standard lithium values to calculate 100%-0%. You can´t set different values like 30V = 0% (which is too low by the way).
```

---
## \#14 Posted by: laikiux Posted at: 2016-09-22T13:43:31.676Z Reads: 267

```
No, it's not too low. It's pretty standart. Theoretically I can discharge my cells till 26V
```

---
## \#15 Posted by: DeathCookies Posted at: 2016-09-22T13:48:35.391Z Reads: 262

```
Edit: you are right. There is not even a STDP switch :smiley:
```

---
## \#16 Posted by: stealth71 Posted at: 2016-09-22T14:42:17.760Z Reads: 249

```
What is the voltage at the switch?  Is it battery voltage or is there a drop down in the circuit somewhere?  I was also looking for a waterproof switch to use on the anti spark.
```

---
## \#17 Posted by: DeathCookies Posted at: 2016-09-22T14:53:11.050Z Reads: 254

```
I got told that the voltage does not really matter as long as it is a SPDT ;)
```

---
## \#18 Posted by: stealth71 Posted at: 2016-09-22T15:24:54.524Z Reads: 253

```
So if you run 50V through a 12V rated DC switch might not be the best idea.  A lot of people say things not knowing what they are talking about.  Have you read anything about derating AC switches when running DC current through them?  When you have AC power it crosses 0V many times a second so the arc will break easily when opening the switch.  DC is a different subject cause there is no alternating current there is never 0V and thus DC switches are rated based on the arc gap needed at a certain voltage to break the circuit.

I think it does matter.  Will something else work possibly, but I am not an electrical engineer and only see a 1M ohm resistor on the circuit to the switch.

<img src="/uploads/db1493/original/3X/5/c/5caf3aad4cfb0f20cecc538920acef64bc97fd6d.png" width="690" height="216">
```

---
## \#19 Posted by: DeathCookies Posted at: 2016-09-22T16:26:33.928Z Reads: 242

```
The Main current does Not Flow through the soft switch, only 12v i assume! 
Thats why i got told that the soft switch voltage Rating does Not matter at all
```

---
## \#20 Posted by: michaeld33 Posted at: 2016-09-22T16:38:20.715Z Reads: 238

```
All my on off buttons have broken due to it "jamming" when it sparks and welds the inside of the switch together. I just use a XT90 loop key. I agree with @lox897 the LCD is very good, I use it on my boards.
```

---
## \#21 Posted by: stealth71 Posted at: 2016-09-22T17:03:02.126Z Reads: 222

```
Again I am not an EE, but when I look at the diagram I see battery voltage coming through the fuse, then through the 1M resistor @ R1.  So in my case 50V fully charged, V = IR so V/R = I or 50/1M = 50/1000000 = 0.00005A @ 50V  When you flip the switch it changes the gate of the mosfet from ground to battery voltage.

Now this is my understanding.  I would love for someone with more electrical design knowledge to tell me I am correct or not and explain why so we can all learn.
```

---
## \#22 Posted by: DeathCookies Posted at: 2016-09-22T18:05:58.872Z Reads: 207

```
I dont know if this is the correct diagram? I know for sure that D2 is outputting only 12V. I have also measured it on my vedder anti spark switch and it shows 11,7V :)
```

---
## \#23 Posted by: elkick Posted at: 2016-09-22T20:21:33.062Z Reads: 200

```
@DeathCookies is right, it's 12V only. It's not switching the main power with the rocker switch.
```

---
## \#24 Posted by: stealth71 Posted at: 2016-09-22T20:32:00.081Z Reads: 202

```
Ok so does anyone know what in the circuit limits the voltage?  Guess I need to hook mine up to the batteries and get the multimeter out.
```

---
## \#25 Posted by: lox897 Posted at: 2016-09-22T22:10:26.996Z Reads: 203

```
@michaeld33 I was assuming with my switch that we had to account for a high voltage and low amps but now that I know that you can go with a low voltage for the switch, the ebay ones should work fine.
```

---
## \#26 Posted by: lox897 Posted at: 2016-09-22T22:14:14.342Z Reads: 204

```
Now that I know that the switch doesn't need to handle a high voltage, only 12v, I have changed the link to a cheaper, exact one.

The criteria for a switch is:
- SPDT
- Non-momentary aka latching
- 12v or higher
```

---
## \#27 Posted by: DeathCookies Posted at: 2016-09-23T07:32:51.397Z Reads: 192

```
[quote="stealth71, post:24, topic:9974"]
Ok so does anyone know what in the circuit limits the voltage?
[/quote]

Like i have said before:

 [quote="DeathCookies, post:22, topic:9974"]
I know for sure that D2 is outputting only 12V.
[/quote]

If you look in the github repo in the BOM it says the following information about D2:
<img src="/uploads/db1493/original/3X/d/6/d62bf562dc992fb4ac3806014f1d9b385e81c672.png" width="690" height="27">
```

---
## \#28 Posted by: shunpo Posted at: 2016-09-24T08:31:48.998Z Reads: 184

```
Hello all. Thanks for the suggestions. I think I've come to the conclusion that buying one from DIY's site is the easiest, as it's already got everything included. My question is, will it work well with 10s? I think it should...

I found this on the esk8 market: https://electric-skateboard.market/product/high-voltage-onoff-switch/

It looks almost the same, if not exactly as the one on DIY's, and it's a little bit cheaper to get it from the esk8 market than it is from DIY's,and being on a budget, and conversions from USD to AUD, I'd like to save as much as I could, every dollar  counts here. 

So, thoughts?
```

---
## \#29 Posted by: mtgawesome Posted at: 2017-08-06T00:45:30.324Z Reads: 87

```
How would I connect this to my zippy 5000mah battery?
```

---
