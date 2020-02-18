# Building a 16s5p battery from 80 samsung 30A laptop cells

### Replies: 27 Views: 1749

## \#1 Posted by: WARMAN Posted at: 2017-02-10T02:36:55.610Z Reads: 177

```
So I'm building a battery from laptop cells,I made it 10s4p first but soon found out through trial and error that it wasn't enough power for the motors to reach there full potential "dual r spec" 
So luckly I had already bought enough laptop batterys "80 cells" in total off a seller on ebay i got a really good deal and all the cells are the same samsung 30a 3000mah.
So I'm going to now build a 16s5p battery I have my bms and charger my question is can I use the 16s "48v" bms and the "48v" charger as the voltage of the intire pack will be more than this,is this enough to charge the batterys fully? will it just take longer or do I need a higher v bms and charger?
```

---
## \#2 Posted by: Tuomalar Posted at: 2017-02-10T03:19:18.372Z Reads: 172

```
You can't use 16s battery with vesc or any other common esc.  And you need 57.6V charger.
```

---
## \#3 Posted by: TheImmortalJew Posted at: 2017-02-10T03:19:22.313Z Reads: 172

```
A 16s5p configuration will not work. There is no ESC out there that can handle that high of voltage, yet! :wink: 12S is the max. Also, I'm not sure what you refer to when you say samsung 30A 3000mah cells. There is no way they can handle 30A continuous, or even peak for that matter. Some specific model number of what cell you have will help to determine what their specs are. 

Either way, this can and has been done before even if the cells can only do 5A continuous. Search laptop battery build and you'll find a few bold pioneers, I know @Ackmaniac did a nice build with some. I would suggest putting as many cells in parallel as you can to get a decent discharge rating. Aim for at least 40A continuous and it should work ok. You could try a 6S13P, 8S10P, 10S8P, etc. Just keep it under 12S.
```

---
## \#4 Posted by: benwong Posted at: 2017-02-10T03:32:48.470Z Reads: 157

```
how to determine li-ion discharge rate? there is not same like lipo C rate. 
if one he2 continue discharge is 20amp, need use how many cell to reach 80amp ? 4p?
```

---
## \#5 Posted by: TheImmortalJew Posted at: 2017-02-10T03:35:33.545Z Reads: 153

```
C ratings are generally used in the world of lipos, but you can rate li-ions by C rating too. Just divide the continuous discharge by the capacity. An LG HE2 would therefore be 20,000/2500 = 8 C continuous discharge. So yes, 4P for 80A.
```

---
## \#6 Posted by: treenutter Posted at: 2017-02-10T03:42:52.501Z Reads: 142

```
@warman is the problem that the cells you used had very low discharge rates? Is that why you feel that you can't optimize your motors?

10s4p built with 18650s or an equivilent provides plenty of power for dual outrunners. A lot of forum members have that setup. 

As others have mentioned, you won't find a common ESC that can handle a pack like that.
```

---
## \#7 Posted by: WARMAN Posted at: 2017-02-10T04:13:31.588Z Reads: 132

```
Thanks for the feedback lads the 30a refers to the battery model like samsung 20f etc it in no way refers to the amps.
The problem is just underpowered @treenutter I'm not actually sure what the a rating is just the capacity.
When made in a 10s4p configuration just wasn't enough speed "only bench tested" but I'm sure it wouldn't have been faster than 18mph on the road.
I do recall seeing another build with 94 cells I think on here and came across "kris's workshop" a channel on YouTube he did the same.
Glad I reached out for advice first before I started spot welding I'm learning all this as I go "first build"
Think I'll go the 10s8p route would the 48v charger be sufficient or should I go with slightly higher as mentioned above?
```

---
## \#8 Posted by: smurf Posted at: 2017-02-10T04:23:58.890Z Reads: 122

```
With a 10sXp you'll need a 42v liion charger
```

---
## \#9 Posted by: WARMAN Posted at: 2017-02-10T04:26:51.061Z Reads: 122

```
10sXp lol you been playing too much ps4! 
Is there a configuration with 80 cells that would make it 48v?
```

---
## \#10 Posted by: smurf Posted at: 2017-02-10T04:30:53.649Z Reads: 116

```
10s 42v
11s 46.2v
12s 50.4v
```

---
## \#11 Posted by: TheImmortalJew Posted at: 2017-02-10T04:35:09.414Z Reads: 116

```
My misunderstanding! This is the datasheet for your cells.
http://www.meircell.co.il/files/Samsung%20ICR18650-30A.pdf
At a 6A continuous discharge you would have 48A with a 10S8P pack, which is decent as long as you don't have crazy hills to climb. You could do 48V (12S) with 72 cells in a 12S6P configuration, but I would stick with the 10S if you have exactly 80 cells to work with.
```

---
## \#12 Posted by: WARMAN Posted at: 2017-02-10T04:50:12.928Z Reads: 114

```
Great info thanks for that top man! 3 hours charge time no shit! It's been 4 days with a 4 bay charger lol 
I do have quite a few steep hills here in bournemouth I would like to bolt up thats why i forked out the extra for dual.
people with samsung 25r high drain in a 10s4p seem to have no problem how would mine compare to that with 80 cells same kind of torque and speed? that's all I'm after and good range obviously.
```

---
## \#13 Posted by: WARMAN Posted at: 2017-02-10T05:45:16.687Z Reads: 116

```
Seems it will still be 32 amps lower than using 25r in a 10s4p anyway I'll keep building and test it if not I'll upgrade later be fine for beach cruising! 
Apriciate the help lads cheers
```

---
## \#14 Posted by: Tuomalar Posted at: 2017-02-10T05:49:00.432Z Reads: 112

```
10s4p with 25r -> 36V, 10k mah and 80A discharge
10s8p with 30a -> 37V, 24k mah and 48A discharge
```

---
## \#16 Posted by: WARMAN Posted at: 2017-02-10T14:42:46.614Z Reads: 96

```
Ended up going with a 10s8p as my charger is actually 42v I'm halfway through the pack should have it done soon @barajabali I'm sure you could answer this would be apriciated...can I use my 16s bms on this battery is there a way to wire it up or should I just buy a 12s bms
```

---
## \#17 Posted by: PXSS Posted at: 2017-02-10T14:50:32.095Z Reads: 93

```
Why are you using those cells? Were they dirt cheap???
```

---
## \#18 Posted by: faithfulpuppy Posted at: 2017-02-10T15:26:22.779Z Reads: 84

```
yeah i wanna see some links
```

---
## \#19 Posted by: WARMAN Posted at: 2017-02-10T15:26:59.030Z Reads: 84

```
Got them all for less than £100 they were a steal and all fairly new cells hardly used!
```

---
## \#20 Posted by: PXSS Posted at: 2017-02-10T15:58:56.322Z Reads: 80

```
Yep. That would be in the dirt cheap category. Lol
```

---
## \#21 Posted by: barajabali Posted at: 2017-02-10T16:26:32.604Z Reads: 74

```
are you gonna make a 10s, 12s, or 16s? 

I've never seen someone use a 12s bms on a 10s battery for example but I think its possible. I dont think it would be a problem if you wired it correctly. 

Just pretend that the last 6 or 4 cells are there and dont hook them up to the BMS
```

---
## \#22 Posted by: faithfulpuppy Posted at: 2017-02-10T16:44:24.385Z Reads: 68

```
are you gonna link us to the seller's page?
```

---
## \#23 Posted by: WARMAN Posted at: 2017-02-10T16:44:28.523Z Reads: 69

```
Yeah sorry meant should I buy a 10s bms I'm nearly done building my 10s8p and will just need to wire in my 16s bms that I have so basically just dont wire in the last 6
```

---
## \#24 Posted by: WARMAN Posted at: 2017-02-10T16:47:43.847Z Reads: 72

```
Was a one off deal Bro ebay seller bought them for a convention then after didn't need them and just wanted rid of them
```

---
## \#25 Posted by: faithfulpuppy Posted at: 2017-02-10T16:48:28.029Z Reads: 74

```
damn that's lucky. Nicely done dude.
```

---
## \#26 Posted by: barajabali Posted at: 2017-02-10T16:51:38.514Z Reads: 73

```
Yea although I've never done it it should work. Are you farmiliar with how to wire a bms? If not hit me up
```

---
## \#27 Posted by: WARMAN Posted at: 2017-02-10T16:52:11.596Z Reads: 72

```
Was lucky as you can never tell which cells are actualy inside samsung laptop batterys I just happened to get 80 of the best maybe search ebay for the highest capacity samsung laptop batterys you can find for a good price
```

---
## \#28 Posted by: WARMAN Posted at: 2017-02-10T16:54:15.695Z Reads: 71

```
Yeah I'm quite competent when it comes to this sort of stuff and iv done alot of research just like to be 100% sure thanks for your input
```

---
