# Power adaptor for BMS - help needed

### Replies: 9 Views: 1040

## \#1 Posted by: MontPierre Posted at: 2017-07-11T17:01:40.920Z Reads: 80

```
Hi!

I have gone through the forum to find answer on which power adapter I will need for my BMS - unfortunately no clear answer to my questions.

My setup is 3x 3S 8000mah in series making it 9S. I know it isn't a typical set up but it made more sense in terms of less individual batteries to mount, 5S would be to thick... 2S would have to be 4x - more space neded.

Anyway, my bms is 10s and I'm planing to connect only 9 cells. Here is BMS I've got 

http://www.ebay.co.uk/itm/Battery-Protection-BMS-PCB-Board-F-10-Packs-36V-Li-ion-Cell-Max-40A-w-Balance-/262605636328


Would I need 33. 3 v power supply - 9x3.7V? 

I saw 36 V on eBay with max 2A - would it be painfully slow charge ? I charge my iPhone with 2A and it takes an hour max. How long would it take on my batteries?  Would it fry BMS ? On my BMS it says that charging ampers are up to 10A.


Here is example of a charger I found:

https://www.ebay.co.uk/itm/391377849281 


I'm only using bms for charging. Any advice would be amazing !
```

---
## \#2 Posted by: Okami Posted at: 2017-07-11T21:21:37.318Z Reads: 66

```
If u charge at 2A, it.means about 2ah can be put in the pack in an hour (at least in 3/4 of charging time)

So it might take almost 3-4hours.to fully charge depending.on how empty battery is and how.much time balancing.takes at the end of charging.

And yes, u might.need 33.3v unless bms can somehow burn off extra volts.

Im not.so good with bms charging.in such.situations but one option would.be to.get "lab power supply" where u can.adjust.voltage as needed, though it probably wont.be.portable.in end and would.loose.the.benefit.of.charging.through bms
```

---
## \#3 Posted by: MontPierre Posted at: 2017-07-11T21:29:15.376Z Reads: 58

```
Thanks! 

Well I might go 10s to make things easier in terms of finding off the shelf charger 37V 2A or higher Amps. Do you think I could install in series 2x 3S and one 4S to make 10S? 

I just got 3x 3S batteries and would want to make most of them rather than selling off all of them and getting let's say 5x 2S.
```

---
## \#4 Posted by: SilentException Posted at: 2017-07-11T21:35:57.563Z Reads: 49

```
You will need a charger with **output** of 4.2V x number of cells, so in your case 4.2V x 9 = 37.8V

BUT, problem is that eBay listings sometimes give you nominal voltages and sometimes output voltages. And on top of that, some use Li-Ion nominal (3.6V) and others Li-Po (3.7V). Ouch. I always look for the output voltage of the charger.

The one you listed is listed as Li-Ion 36V, which probably means it is actually 10S or 42V output. You don't want that.
```

---
## \#5 Posted by: MontPierre Posted at: 2017-07-11T23:03:33.367Z Reads: 45

```
This clears up a lot for me. I think I will go with 10s setup to find 42V charge - plenty on ebay. 

I found this which nicely shows charging voltage vs nominal voltage :slight_smile:
 
<img src="/uploads/db1493/original/3X/e/5/e5261da6b7e7fa6175666c12ccc3ce11ca60813f.png" width="690" height="336">

I hope this helps someone! 

Any thoughts on ?
> Do you think I could install in series 2x 3S and one 4S to make 10S?
```

---
## \#6 Posted by: jmasta Posted at: 2017-07-11T23:32:30.930Z Reads: 41

```
Can you use a 10S BMS with only 9 cells? Wouldn't the BMS see one cell voltage as 0V and cut the line?
```

---
## \#7 Posted by: SilentException Posted at: 2017-07-11T23:34:45.242Z Reads: 39

```
[quote="MontPierre, post:5, topic:27367"]
Do you think I could install in series 2x 3S and one 4S to make 10S?
[/quote]

Theoretically, yes but I would make sure they are the same cells (mAh, manufacturer, C-rating, even size). Wrapped Li-Po packs are usually ohm-matched (cell internal resistance) and if you mix and match different cells you will end up with very uneven "pack".

[quote="jmasta, post:6, topic:27367, full:true"]
Can you use a 10S BMS with only 9 cells? Wouldn't the BMS see one cell voltage as 0V and cut the line?
[/quote]

Both BesTech and SuPower (batterysupports) told me it is a no-issue. Guess 0V means "no cell" and not "empty cell" :slight_smile: Well, if I think about it, not connected line would perhaps not even read 0V but some weird value so they have a way of knowing if a cell is connected.
```

---
## \#8 Posted by: MontPierre Posted at: 2017-07-12T08:23:05.458Z Reads: 37

```
Indeed, I'm thinking of getting 2s Zippy 8000mah and their 3S model 8000mah looks like it has exactly same C rating, even size, its just one cell less. Well I'll give it a try, it will save me space of one battery, I'll have 4 instead of 5.
```

---
## \#9 Posted by: Slak Posted at: 2018-06-01T11:11:55.003Z Reads: 12

```
Pretty sure IR will be different between 2S and 3S Lipo, even if it is the same brand, series, etc...
Don't know if it will be a problem but others should be able to confirm that
```

---
