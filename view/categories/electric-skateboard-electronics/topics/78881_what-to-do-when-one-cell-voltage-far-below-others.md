# What to do when one cell voltage far below others

### Replies: 43 Views: 645

## \#1 Posted by: Songsta Posted at: 2018-12-24T19:37:02.859Z Reads: 172

```
Hi all

I'm a noob to Esk8ing and have come across my first battery issue.

One of my cells on one of my 2 6s batteries is about 1V lower than the others. My charger has given me the warning “balancer voltage too low”. When I checked, the voltage was 2.538V while the others where ranging from 3.19V to 3.60V (See the attached images)

Is the situation irreversible? I’ve read the anything below 3V is pretty bad for lipos so getting this low is probably going to mean I throw away the pack. Also, the fact that there are such major differences between the voltages doesn’t seem good either. 

To give some context which might help - I rode my board today (Trampa Urban Carver, 136kVa motor) with the batteries at around 55%. They are connected as 12s. I had charged the batteries about 4 days ago and then rode until about 60% on that day. My ride today was really short - 3,3kms on relatively flat road, but the battery went to 7% at the end, which took me about 25 minutes. It was when I tried to charge the batteries again to storage levels that I got the warning. 

I’ve checked the other battery and everything there looks good and all values are within a hairs breadth of each other. 

Any help here would be greatly appreciated. 

![image|666x500](upload://piCiB6uKHmr8kLn734HWvn7laXq.jpeg) 


![IMG_1062|666x500](upload://msZV6ojjTthOrCxzZ68k7dBddws.jpeg)

![image|666x500](upload://vy9wtVCauLURqbOy3EEtDkoeKDY.jpeg)
```

---
## \#2 Posted by: Sn4pz Posted at: 2018-12-24T20:23:02.577Z Reads: 154

```
Does it show and external signs of stress? Puffing? Leaking?

If not, you might be able to charge it up and balance just fine

Just keep an eye on it and a bag of sand near by
```

---
## \#3 Posted by: Songsta Posted at: 2018-12-25T04:46:31.417Z Reads: 140

```
Thanks for the advice, Sn4pz. I can’t see any visible issues at all. 

I have a Lipo bag that I’ll use when trying to charge it. 

The charger won’t allow me to even charge it using the balancing cables when sees a voltage below 2.75V but the manual recommends charging it without the balancer cables for a few minutes to get it above the threshold and then continuing with the balancer cables after that.
```

---
## \#4 Posted by: Andy87 Posted at: 2018-12-25T04:51:14.582Z Reads: 135

```
All your cells are pretty much out of balance.
That doesn’t look good at all.
Usually the cells should be around +-0.1V from each other.
Did you already tried something in the meanwhile?
```

---
## \#5 Posted by: Songsta Posted at: 2018-12-25T04:56:15.439Z Reads: 128

```
Something else that may have impacted this is that I didn’t prep the batteries before I used them for the first time about a month ago. I just connected them to the board and used them. They ran to 0% (as indicated on the led indicator on my board) and when I then connected them to the charger all the cells were at around 2,98 - 3.02ish. They charged and balanced fine immediately after that, but perhaps that wasn’t the wisest thing to do with new batteries?

I must admit that it’s exciting to learn about how all of this works (the electronic side of Esk8ing) but it’s also a little scary, because it’s not a cheap endeavour (at least not here in a South Africa) and not ruining my equipment is definitely high on my priority list!
```

---
## \#6 Posted by: Songsta Posted at: 2018-12-25T04:57:15.945Z Reads: 124

```
No, I haven’t tried anything yet. I’ve been waiting for advice from this forum.
```

---
## \#7 Posted by: PXSS Posted at: 2018-12-25T04:58:06.031Z Reads: 120

```
The battery is in general over discharged. Probably no permanent damage if its the first time but deff dont make it a habit. 

You can charge without balance wires until the last cell reaches 3.2v then charge normally. 

The reason all the cells look so out of balance is that you over discharged them. Once batteries reach 3.3v they can drop down to 2v in matter of minutes. 

Charge your battery and balance them. After ride until you see about 3.5v/cell under load or 3.7v/cell with no load. This should be your new 0% charge. Keep it above that and your battery will last a long time.
```

---
## \#8 Posted by: PXSS Posted at: 2018-12-25T05:01:00.833Z Reads: 114

```
What capacity is your battery?
Charge it at 0.2x the capacity in current as soon as possible. The longer you leave it over discharged the more damage there is. 

Also try to keep the battery compressed and cool when charging initially to 3.2v min. That way it wont delaminate.


If you make this a habit then your batteries will die very quickly.
```

---
## \#9 Posted by: Songsta Posted at: 2018-12-25T05:05:32.568Z Reads: 106

```
Its 2x 6s 6000mAh in series, so 12s.

So I connect the one battery to the charger _without_ the balancing cable and charge for a few minutes. I then put the balancer cable back in and check the voltage of the lowest cell to see if it’s above the threshold of the charger’s minimum allowed voltage. Once it’s above that I leave the balancer cable in and continue to fully charge it?

I guess I should also change my LED indicator to show Volts, not percentage?
```

---
## \#10 Posted by: Songsta Posted at: 2018-12-25T05:06:32.820Z Reads: 95

```
This happened yesterday afternoon (about 12 hours ago) and I was too scared to do anything about it until I’d asked here.
```

---
## \#11 Posted by: PXSS Posted at: 2018-12-25T05:19:28.062Z Reads: 91

```
Correct. You should charge at 1A initially.
Also yes. Change to display voltage.

If you keep over discharging the battery like this. It won't last very long at all.
```

---
## \#12 Posted by: Songsta Posted at: 2018-12-25T05:35:26.494Z Reads: 88

```
Thanks. I’m definitely going to try monitor things better from now on.
```

---
## \#13 Posted by: Andy87 Posted at: 2018-12-25T05:40:00.609Z Reads: 91

```
I can recommend you to add a lipo alarm to your packs
https://hobbyking.com/en_us/hobbykingtm-lipo-voltage-checker-2s-8s.html?___store=en_us

it´s cheap and you can set your indication voltage how you want.
so if any of your cells in your pack will drop down the set voltage you will get an alarm.
```

---
## \#14 Posted by: Songsta Posted at: 2018-12-25T05:45:10.105Z Reads: 89

```
Thanks Andy. What concerns me is that I’ve got the Vesc 6 and it’s supposed to have the battery protection checking in it. I’ve set all the thresholds correctly but it doesn’t seem to be accurate. I don’t know if it tracks individual cells though.
```

---
## \#15 Posted by: Andy87 Posted at: 2018-12-25T05:53:24.507Z Reads: 85

```
The vesc6 like any other vescs only monitor the over all voltage.
if you want to monitor the single cell voltage, you need a BMS for discharge, or the cell checker I linked you.
What was your battery cut off start and cut off end setting in the VESC?

For lipos it should be something around 3.5V per cell, 
so for 12s for example cut off start at 44.4V and (3,7V per cell) and end at 42V (3.5V per cell)
```

---
## \#16 Posted by: Songsta Posted at: 2018-12-25T06:27:57.703Z Reads: 80

```
I've got the cut off start at 44.4 and the end at 38.4, which is 3.2 per cell.

I'll definitely take your advice and get a cell checker.
```

---
## \#17 Posted by: NickTheDude Posted at: 2018-12-25T06:38:42.933Z Reads: 77

```
3.2 is very low for lipos, that's probably why they got overdischarged in the first place. You should set the cutoff end to 3.7 like @PXSS said.
```

---
## \#18 Posted by: Andy87 Posted at: 2018-12-25T06:49:45.834Z Reads: 75

```
rise the cut off end to 3.5V per cell.
after that you anyhow don´t get something out of the packs
and the risk is too high to overdischarge them, like you did.
better save than sorry ;)


EDIT: I noticed that the cell checker not super accurat, means they meassure the volatage +-0.2V depending on the one you get.
I would recomment to check the cell voltage first time with your charger, thant with the cell checker and than adjust the alarm limit to the tolerance the checker has. Or just set the alarm a bit higher and you will get the peeping more early ;)
```

---
## \#19 Posted by: pat.speed Posted at: 2018-12-25T07:57:05.595Z Reads: 73

```
I think he is using lipos, I would definitely not recommend recharging after a cell has gone as low as 2.5v. This happened to me the other day and I have ruined my pack
```

---
## \#20 Posted by: J0ker3366 Posted at: 2018-12-25T08:03:59.750Z Reads: 70

```
Your lipos is trash. Replace it. Set your hard cutoff to 42v. Set you soft cutoff 44v. Try not to run it to hard cutoff. You'll harm the lipos.
```

---
## \#21 Posted by: Songsta Posted at: 2018-12-25T09:53:58.991Z Reads: 66

```
I've been charging up the pack today and it seems to be working. The balancing is working and the cell's resistance seems to be reducing so I think I may be able to save this battery after all.
```

---
## \#22 Posted by: pat.speed Posted at: 2018-12-25T10:02:50.896Z Reads: 63

```
I’d be scared to use it again. What would you rather fork out for a new pack or a new board? I’m going to try and fix my pack and just use it for low power applications, maybe a portable charger
```

---
## \#23 Posted by: J0ker3366 Posted at: 2018-12-25T10:10:23.333Z Reads: 63

```
[quote="Songsta, post:21, topic:78881"]
so I think I may be able to save this battery after all.
[/quote]
You haven't saved it. Its going to gradually shit on you completely no matter what you do. I did the same thing with some 2s lipos. Had one of them drop and it started taking out the others. Originally bought 6 2s for the build and ended up having to buy 4 more to replace the dying ones. Don't compromise your other lipos! Replace it.
```

---
## \#24 Posted by: PXSS Posted at: 2018-12-25T13:53:14.466Z Reads: 64

```
I know he's using a lipo. His cells are basically brand new, yours probably are not. The battery is not trash. 

I do this for a living plus I also fly a lot of RC and have over discharged plenty of batteries when I forget to set my timer. If its an older battery it'll get puffy and capacity will be greatly diminished and you can essentially call it trash. On a newer battery you'll probably lose 20-30 cycles of life plus some capacity which isn't insignificant but the batteries are definitely not trash.

If he takes better care of them, he'll be okay. The battery isn't 100% anymore but its also not super damaged. 

@J0ker3366
Not two scenarios are the same. You had 6 different batteries to keep in check. He only has 2. Yes, eventually the lipo is going to crap out, all of them do. His battery being brand new and only over discharged twice now, (I hope) wont ride as good as it would had he never over discharged them but again, they are not trash. 

He's also got a balance charger, so he can learn how to use one properly and how to diagnose a dying lipo. With his charger he might even be able to do a capacity check, IR check, and temp check on a charge cycle, all of which can determine the state of his battery far more accurately than any of our guesses. 

Doing a periodic capacity check on your cells is recommended so you don't get caught off guard when a battery starts dying. 

---

Yes, one bad lipo can take out other good ones but with the proper care, it won't happen. If he follows my advice and raises his threshold so that none of his cells get over discharged any more he'll be okay.
```

---
## \#25 Posted by: deucesdown Posted at: 2018-12-25T15:55:10.048Z Reads: 60

```
Some general advice to help you get caught up quicker.

If you're running without discharge bms, especially lipo. Don't even get near the neighborhood of empty. Things get unpredictable near empty, especially with old or damaged lipos.

Check cell voltages of old or suspicious packs often.

Lipos have different "empty" voltage than 18650. About 3.7v is essentially empty. 3.85v is about 50%. Sounds like your battery meter, and your vesc settings, were for lithium ion not lipo.

Don't leave lipos at full charge for long periods.

With lipo, you can plan your rides so you charge to full right before the ride, and finsh the ride at storage voltage, you can save from over discharge problems and a lot of fussing with storage charge.
```

---
## \#26 Posted by: Songsta Posted at: 2018-12-25T21:11:11.314Z Reads: 57

```
Thanks @PXSS. I’ve taken the batteries to storage levels which seemed to have balanced everything nicely again. 

I cant do a capacity check with my charger, unfortunately. Can you suggest how I would do this? I’m also not sure what and IR check is? 

Cheers and thanks for all the great help!
```

---
## \#27 Posted by: PXSS Posted at: 2018-12-25T22:24:58.246Z Reads: 49

```
What charger do you have?
```

---
## \#28 Posted by: Songsta Posted at: 2018-12-26T03:29:16.792Z Reads: 42

```
I've got the Graupner Ultramat 18 from Trampa. It can charge up to 12s, which allows me to keep the batteries in the battery box and just plug the charger into the xt90 sticking out the box.
```

---
## \#29 Posted by: Songsta Posted at: 2018-12-26T03:46:02.445Z Reads: 46

```
**Update**:

 when I woke up this morning and went to charge the batteries for a morning skate, I saw that the one battery hadn't retained the storage charge very well compared to the other. I didn't jot down the voltages before I started charging, but I took pics just after charging had started, which should still show what I mean.

![20181226_053927|690x215](upload://29UXanbqqAVBt8Nx5DwRjcfw9zV.jpeg) 
![20181226_053905|690x203](upload://rNNdrUjRCfw8OrADYIat7cyNBmO.jpeg) 
![20181226_053835|690x249](upload://veWKJiZrvHGyDzj5xzJLxTQ9drV.jpeg) 
![20181226_053815|690x221](upload://jImu36P3eQsH4fS5jF068Qz8Rxm.jpeg) 
![20181226_053746|690x206](upload://br33J0x3ynRXfc772PrBmh3YzcV.jpeg) 
![20181226_053408|690x202](upload://qEEE6h64ruNzO9QdVoLFHLoHera.jpeg) 

I'm going to ride it a bit after its charged and then check the levels afterwards to see how unevenly the draw is. I'll post the results after that.
```

---
## \#30 Posted by: Songsta Posted at: 2018-12-26T04:04:46.037Z Reads: 45

```
[quote="deucesdown, post:25, topic:78881"]
Sounds like your battery meter, and your vesc settings, were for lithium ion not lipo.
[/quote]
Everything was configured for LiPo. I got the board from Trampa, pre-built, and they advise the VESC configuration for LiPo, which I set accordingly. 

Here are the settings that were sent to me when I first bought the VESC. These are for a single motor configuration.

**Motor Current Max:**

118Kv: up to 45Amps

**_136Kv: up to 50Amps (my motor size)_**

154Kv: up to 55Amps

**Motor Current Max Brake**: up to -35Amps (will give you efficient braking not too sharp)

**Battery Current Max**: 60Amps 

**Battery Current Max Regen:** -30A
```

---
## \#31 Posted by: deucesdown Posted at: 2018-12-26T04:28:20.566Z Reads: 44

```
[quote="Songsta, post:16, topic:78881"]
I’ve got the cut off start at 44.4 and the end at 38.4, which is 3.2 per cell.
[/quote]

This is what I was talking about with respect to vesc. 3.2v cut off per cell is low for lipo, especially with no bms on discharge.

sidenote: Even with BMS you don't want to bump into low cell voltage cutoff and have the bms cut power.
```

---
## \#32 Posted by: pat.speed Posted at: 2018-12-26T04:31:45.199Z Reads: 43

```
Do you use the balance lead when charging? Or do you use a bms in the box, if you don’t use balance leads the cells can’t be balance correctly
```

---
## \#33 Posted by: Songsta Posted at: 2018-12-26T04:59:40.016Z Reads: 43

```
[quote="pat.speed, post:32, topic:78881"]
Do you use the balance lead when charging?
[/quote]

Definitely! The first thing you read about LiPos is how you need to ensure they’re balanced.
```

---
## \#34 Posted by: pat.speed Posted at: 2018-12-26T06:28:00.738Z Reads: 42

```
[quote="Songsta, post:28, topic:78881"]
plug the charger into the xt90 sticking out the box.
[/quote]


All g, I thought you weren’t by the way you said this
```

---
## \#35 Posted by: Songsta Posted at: 2018-12-27T04:25:39.105Z Reads: 36

```
I thought I’d share my individual cell volt readings from yesterday to get some thoughts from the forum.

(I started tracking my voltages in a spreadsheet instead of just as pictures, to make it easier to share here.)

Below is a table of what the readings looked like:

|Description|Cell 1|Cell 2|Cell 3|Cell 4|Cell 5|Cell 6|Cell 7|Cell 8|Cell 9|Cell 10|Cell 11|Cell 12|Total Volts|
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
|Fully Charged for the day|4,190|4,194|4,191|4,196|4,195|4,194|4,195|4,195|4,194|4,194|4,195|4,193|50,326|
|After first skate|4,077|4,067|4,100|4,033|4,127|4,081|4,094|4,094|4,094|4,089|4,095|4,094|49,045|
|After second skate|3,919|3,909|3,943|3,891|3,962|3,926|3,939|3,939|3,937|3,932|3,938|3,937|47,172|
|After final skate|3,729|3,719|3,741|3,706|3,752|3,731|3,742|3,742|3,737|3,739|3,735|3,737|44,810|
 

You can see that cells 1-6 don’t discharge as evenly as cells 7-12. I’m not sure exactly how bad it is, as I’m not sure what the tolerance should be.

I’ve had _no_ heating up or puffiness of the batteries and the batteries seem to be performing well.
```

---
## \#36 Posted by: Andy87 Posted at: 2018-12-27T05:38:39.953Z Reads: 36

```
The difference is less than 0.1V. 
I wouldn´t worry in this case. Just keep tracking the values in future.
All your cells will have probably a slightly different internal resistance, so over the discharge they also slightly discharge different from each other.
```

---
## \#37 Posted by: Songsta Posted at: 2018-12-27T10:21:09.988Z Reads: 35

```
Thanks Andy. I'm glad my batteries don't seem to be ruined.
```

---
## \#38 Posted by: PXSS Posted at: 2018-12-27T13:48:44.599Z Reads: 33

```
Sorry I havent replied. The thread wasnt pinging me. I'll give you a more detailed reply tonight but your cells look good on a quick glance. Yes they are not as even on 1-6 but that's expected after the over discharge. 

I'm glad its not damaged too bad. Keep checking it regularly and it'll last a long time :)

Do change your vesc settings as @deucesdown recommended!
```

---
## \#39 Posted by: pat.speed Posted at: 2018-12-27T14:25:11.101Z Reads: 33

```
A little off topic, but the cells I over discharged came back up to 3.98v after letting them rest for a day or two. I then charged them at 1 amp to 3.4v then 3.5amps up to 3.75. The cells seem almost unscathed as they perfectly balanced themselves without even using the bms or anything, just connected straight to the output of a hobby charger with two battery cell checkers connected.

I still plan to put a new pack into my board as I am paranoid about an esk8 fire, but I guess you were right about the cells being salvageable. They will now be a power bank for my phone and esk8 range extender
```

---
## \#40 Posted by: PXSS Posted at: 2018-12-27T14:40:50.719Z Reads: 33

```
I would never recommend using a battery that was not balance charged immediately after an over discharge event. They might look ok but they need to get balanced at 4.2v. So unless you have a way to balance charge them, yes, you should replace them. :)

Also. Dont let your lipos rest too long after an over discharge, it's not good for them. The sooner you get it to its storage voltage, the better. You do have to keep the battery cool though.
```

---
## \#41 Posted by: Songsta Posted at: 2018-12-27T17:30:48.313Z Reads: 25

```
Thanks all for the great help and advice! This was my first post on this forum and the response I got was encouraging, especially for a n00b.
```

---
## \#42 Posted by: Songsta Posted at: 2018-12-27T18:12:56.684Z Reads: 24

```
[quote="PXSS, post:38, topic:78881"]
Do change your vesc settings as @deucesdown recommended!
[/quote]

I did so before I started riding yesterday. Too nervous to mess up my batteries further!
```

---
## \#43 Posted by: PXSS Posted at: 2018-12-27T18:30:12.798Z Reads: 23

```
For lipos you should be using roughly 80% of their rated capacity for max cycle life. Next time you empty your pack, do an unbalanced charge cycle with balance leads plugged into your charger so it doesn't over charge any one cell. This will give you the most accurate estimate on how much capacity you're actually getting out of the battery. In reality it's still a little lower since there are some inefficiencies in charging that the charger doesn't take into account.
```

---
