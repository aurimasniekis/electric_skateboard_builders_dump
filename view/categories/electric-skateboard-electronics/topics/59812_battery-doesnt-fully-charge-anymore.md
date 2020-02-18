# Battery doesn&rsquo;t fully charge anymore

### Replies: 49 Views: 1090

## \#1 Posted by: rey8801 Posted at: 2018-06-23T08:18:23.748Z Reads: 191

```
Hi guys! Basically until one week ago I was charging my battery 10s3p 30Q up to 41.2V to increase the life span, since I had a bms for charging and discharging. Now I change the BMS for charging only and the last week I notice that I reached home with the battery being 10-15% lower than usual. Therefore I decide to open the charger and set it back to 42.1V instead of 41.1V. Then charged the battery but it only reaches 40.2V instead of 42.1V. I checked the charger and it outputs 42.1V but stops charging at 40.1V. In the past with my charger set at 41.1V the battery reached 41.1V. Do you know what could it be? Thx
```

---
## \#2 Posted by: rey8801 Posted at: 2018-06-23T08:49:51.066Z Reads: 185

```
I then turn on the board and spin it. Then connect the charger and this time stopped charging at 40.7V instead of 40.1V. I hope it's the charger that is not able to read the V from the battery anymore.
```

---
## \#3 Posted by: Ackmaniac Posted at: 2018-06-23T11:05:23.269Z Reads: 184

```
Guess it's the bms that shuts down too early. Just check each cell with a multimeter via the balance leads if they are balanced. Maybe one cell is too high so that the bms shuts down too early.
```

---
## \#4 Posted by: rey8801 Posted at: 2018-06-23T11:35:24.040Z Reads: 176

```
Yeh that was my fear. It would mean open the battery pack again :tired_face: then I do not understand the purpose of bms if the cell are not balanced anymore.
```

---
## \#5 Posted by: rey8801 Posted at: 2018-06-23T11:50:13.095Z Reads: 166

```
Yeh is the bms. I open the enclosure and basically my bms has leds to show when the single cells reached 42V...
![IMG_20180623_134135_HHT|281x500](upload://mgYqA8MMnPgqtrNF6N5V5MUYePK.jpg)

As you can see one of the led is on. Basic Aly it has led to show when the single cells reach 42V.

Here the bsm I use 10S 40A/60A bms Li-ion large high current BMS PCM with SAME discharge port for electric bike electric car 60a bms
 http://s.aliexpress.com/ZzUZRVvE?fromSns=Copy to Clipboard
![aliexpresshd|281x500](upload://m2kBm7x4l2Ul9iswQr1LhfgDHc2.jpg)

Then I do not really understand the purpose of it. It's gonna to be worse over time. How can I solve it?
```

---
## \#6 Posted by: onepunchboard Posted at: 2018-06-23T12:08:57.284Z Reads: 156

```
my suggestion is ride the board until u reach soft cut off and slow discharge at home till safe limit. 
then try charge again. (check the cell group with meter)
18650 tensency to discharge and match the voltage. 
Fast charging can cause unbalance like you. 

I think we all have to face this issue sometimes as we use regen brake. which kinda aid this problem, unless you use discharge bms.

hope this helps

btw I haven't tried BT module bought from you. is it just plug and play or do I have to set something? give me a short note
```

---
## \#7 Posted by: rey8801 Posted at: 2018-06-23T12:14:26.402Z Reads: 152

```
Thx for answer. My was discharge also, I just moved to charging only one week ago and that was enough to unbalance it. I do not really like this behaviour, since I do not fast charge the battery. 

It's plug and play you only have to set it in vesc. If master PPM and UART with 9600 baud. If slave UART 9600 baud.
```

---
## \#8 Posted by: onepunchboard Posted at: 2018-06-23T12:20:27.471Z Reads: 150

```
I'm sorry to hear that.

I think you have to open the pack and discharge problem pack to match the others.
```

---
## \#9 Posted by: rey8801 Posted at: 2018-06-23T12:24:36.839Z Reads: 150

```
Yeh but how to discharge the problem cells without remove the nickel strips? Moreover it will be back again in one week
```

---
## \#10 Posted by: onepunchboard Posted at: 2018-06-23T12:30:21.694Z Reads: 144

```
hm, just a guessing but bms could be defective.

oh got an idea, if you charge it at lower voltage like 38v or 39 and try continue charge till 42v this might do trick.

and for discharging take the problem balance wire (+lead) and clip or use magnet to connect with - lead. like magnet press coper wire on top of battery.
and connect those wire to hobby discharger or small light bulb. I fixed many labtop batt like this.
```

---
## \#11 Posted by: rey8801 Posted at: 2018-06-23T12:36:06.522Z Reads: 133

```
Thanks for the idea for discharging. 
On the other hand I don't understand what you meant with charging at lower voltage and then try to keep charging to 42V. In my mind the bms charging only does the job when you reach 42V and only there it will adjust the cells between each other. Moreover It can only balance small difference not huge gap. Do you think bms balance along the all charging process? Because otherwise I do not understand how can be that the cells are unbalanced now.
```

---
## \#12 Posted by: onepunchboard Posted at: 2018-06-23T12:43:12.569Z Reads: 127

```
I meant 
charge the pack to 38v and 39v 40v and so on
so you give the pack constant 38 voltage.
if the pack reach 38v it will no longer charge higher than 38 because you only give 38.
than you go to 39v the pack will stop at 39v
and so on.
it might work or not. I havent tried this myself.
but Idea is giving other cells enought time to catch up problem cell group. that way they may match at lower voltage and start charging together to the 42v.

I have no idea how bms works but looks like yours only thinker at the end of voltage.
```

---
## \#13 Posted by: rey8801 Posted at: 2018-06-23T13:44:30.097Z Reads: 122

```
Ok got it. I am now discharging the battery on the bench. It will take a while and then I will try to charge at lower V. The thing is that I only have a 10s charger so I can not decrease and increase the V too much. It only allows few V adjustments.
I think that most of the bms for charging works like that. Only the discharging function is constantly working. I will maybe switch to a Bestech or similar if they are more reliable.
```

---
## \#14 Posted by: Ackmaniac Posted at: 2018-06-23T13:57:20.378Z Reads: 123

```
Forget all that have been said.
First check the cells voltages if they really differ from each other. Maybe the BMS is defective so that it thinks one cell is already fully charged but isn't in reality.
If one cell is really fully charged already then leave the pack connected at the charger for a couple of hours because now the BMS needs to balance the cells which can take a long time when the balance bleed current is only 50ma or somewhere near.
The BMS shouldn't balance during discharge and it also can't do that when the bleed current is so tiny and we only brake for a couple of seconds.

When you charged the pack to less voltage then stupid BMS can't balance the cells because they only start to balance when the cells are fully charged.

If the cells voltages really differ that much from another then there also must be a reason which you should try to find out. Maybe one cell in a parallel pack lost a nickel strip.
```

---
## \#15 Posted by: rey8801 Posted at: 2018-06-23T14:01:48.947Z Reads: 120

```
Ok so now the I discharged the battery to 36V, I will plug it and leave it for hours after the charger will stop charging. Do you know a BMS that either I can use it charge and discharge, without the problem of cutting the brakes as I had when my bms was discharge too (but at least the cells were balance at that time I belive), or one that is for charging only but does balance also during the  Haring and not only when battery is fully charge. Thx for the help
```

---
## \#16 Posted by: Ackmaniac Posted at: 2018-06-23T14:11:46.628Z Reads: 111

```
You don't need to discharge, doesn't change anything.

Problem is that it would be wrong for the BMS to start balancing when the battery has a low voltage and get's charged.

Let's say fully charged all cells are exactly at 4.2V.
When you discharge a 10S pack to 30V then one cell might be at 2.9V another one at 3.1V, another one at 2.95V, another one at 3.05 and a couple at 3.0V. Because the cells are not perfectly evenly discharged. One might have a capacity of 2900ma and another one has 3000ma. So during discharge they can differ from each other.
So if the BMS would kick in immediately when you charge it it would lower all cells that are above the lowest cells from the beginning. And when it is then close to fully charged it needs to lower the the cells which were at 2.9V at the beginning because they would have a higher voltage as they have less capacity.
So it makes sense to only balance when the cells are close to beeing fully charged.
A stupid BMS which is only driven by hardware can only kick in at a fixed voltage which is adjusted by resistors. And most BMS are like that.
A smart BMS could be adjusted adjusted to balance the cells to a desired voltage of 4.1V.

So in your case. Charge the pack until the charger tells charging is done and then check the cells voltages. If they differ a lot check the battery for faults. Otherwise leave it long connected to the charger so that the BMS can balance the pack.
But maybe your charger and BMS don't fit together because if the BMS reduces the charge voltage the charger might think charging is done and shuts down.
```

---
## \#17 Posted by: rey8801 Posted at: 2018-06-23T14:37:10.734Z Reads: 101

```
Thx, got it. I actually do not know if my bms adn charger will work togheter. To me my charget stops charging once the Voltage is reached and that's it. I ma now charging to 41 V, then I will charge to 42V. On the other hand I was thinking whether could be a good idea set the charger a bit higer, like 42.7V so that the bms has more time to balance and the charger will maybe keep trying to charge the cells. What do you think? too risky?
Do you know a good BMS that does is fuxxxing job? I do not want to facing it every week. I do not know who doesn't use any bms how can not have unbalanced cells then.
```

---
## \#18 Posted by: wafflejock Posted at: 2018-06-23T14:41:08.373Z Reads: 100

```
I use lipos so different situation to some degree but just use a balance chargers (AR1 from keenstone is what I'm using, imax b6 is popular as well).  BMS is mostly just taking this kind of balance chargers with you plus some extra features possibly for monitoring or balancing cells on the fly.
```

---
## \#19 Posted by: rey8801 Posted at: 2018-06-23T14:49:02.665Z Reads: 104

```
yes but than I need the balance connector available to plug it to the balance charger. Meaning there is no reason of having a BMS charge only. That's why we use a BMS to be able to charge the board with a normal charger.
```

---
## \#20 Posted by: wafflejock Posted at: 2018-06-23T14:59:44.686Z Reads: 119

```
Right I wasn't saying to have both a BMS and balance charger was just saying what people without a BMS do.. should have quoted but was on mobile.

[quote="rey8801, post:17, topic:59812"]
I do not want to facing it every week. I do not know who doesn’t use any bms how can not have unbalanced cells then.
[/quote]

This was one of the things that pushed me away from doing 18650 based packs (either buying a spot welder or buying a premade one).  Seems everyone insists on hooking up a BMS instead of coming up with a way to charge with more reliable charger that gives you feedback about what's going on and the health of your cells.  I've heard good things about the bestech BMS but they come at a cost.

No reason one couldn't hook up a balance connector (it's just a JST-XH connector, just need a crimp tool and some connectors and time).  Only issue then is getting a charger that can deal with 10S (they exist but more expensive than 6S ones).  Another plus with dropping the BMS is there's less components to get rattled apart on your board (getting rid of parts makes the engineering part of me happy).

Sorry I know this doesn't help with the immediate issue but might be worth considering.
```

---
## \#21 Posted by: rey8801 Posted at: 2018-06-23T18:03:07.264Z Reads: 103

```
Thanks for your input. I appreciate the help that I always receive from this community.
```

---
## \#22 Posted by: bartroosen12 Posted at: 2018-06-23T18:24:48.418Z Reads: 105

```
Just charge your board for a longer time, let the charger plugged into your board also when the charger says that the battery is full.
It just means the that your cells are not balanced perfectly, one cell hitted 4,2V and the charger stops, than the bms will slowly discharge that cell and the charger will start again for a couple minutes. It just takes a long time but once you did that it won't give problems in the future.

One cell is 4,2V and the others will be around 4,05V. That's really not a problem at all, believe me. I've had a 16S pack and 1 cell was at 4,2V while the others were only 4V and plugged my charger in for around 20h and the cells were all perfectly balanced.
```

---
## \#23 Posted by: rey8801 Posted at: 2018-06-23T18:27:24.811Z Reads: 101

```
Now I charged all the cells up to 41V. I already see the same led on(few post above to see the picture) which is wierd. I will now charge them to 42V and leave it. I hope I will see more led turn on over time. I will keep you all post it.
```

---
## \#24 Posted by: bartroosen12 Posted at: 2018-06-23T18:38:28.055Z Reads: 102

```
![IMG_20180623_203455|375x500](upload://rBCdS4TgoDXT7iJDNZVwEImxpip.jpg)
This was my pack with lifepo4 cells so 3,6V means fully charged. You can see one cell was 3,7V so the bms stopped and slowly discharged only that cell. Than start charging again when the cell is below 3,55v. At the left you can see the result after 20h charging, perfectly balanced.
I got a bluetooth bms so I could check everything on my phone and computer.
Just set your charger between 42V - 42,5V and you will be fine.
```

---
## \#25 Posted by: Holyman92 Posted at: 2018-06-23T19:13:53.344Z Reads: 93

```
My 1st bms arrived damaged, would only charge cells to 80% upon further inspection (separating the metal sandwich heat sinks) I found the last 2, either resistors or diodes, burned up on this bank of 10... logic says 2 out of 10 burnt means only 80% charge... they said it wouldn't harm the cells to run so I did u til my new bms arrived
```

---
## \#26 Posted by: rey8801 Posted at: 2018-06-23T19:17:48.243Z Reads: 91

```
I think that part it's fine form me since I reach 41v and in the past I charged up to 42V. Anyhow this BMS does what they want:smile:
```

---
## \#27 Posted by: rey8801 Posted at: 2018-06-23T19:19:04.806Z Reads: 88

```
YEh I got know abot the bluethooth one too late. It would have been fantastic! Anyhow now charger at 42V and let's see
```

---
## \#28 Posted by: rey8801 Posted at: 2018-06-24T07:45:49.261Z Reads: 88

```
HI! I left the battery charging the whole evening and night and I see that the only led that was on is now off menaing the bms balanced that one, but the overall voltage is exactly 41V when the charger should go up to 42V> I think the bms doens't resume the charging and stops everything at 42V. Althought I remember the first time I charged them all the led were on becasue the all battery pack reached 42V. Which BMS did you use? would you reccomemended? I think it's useful being able to read the single pack Volt. Thx
```

---
## \#29 Posted by: bartroosen12 Posted at: 2018-06-24T07:48:45.673Z Reads: 88

```
I have this bms now:
http://s.aliexpress.com/fmQRjeYJ?fromSns=
41V isn't bad at all that 1V more maybe like 3% range of your whole battery. When you drive a full 42V pack, the voltage in the begin drops so fast so that 1V won't make any difference.
![0L|690x388](upload://5wQ4tp9FfjxAdlpbDDyHEAo8Idr.png)
This is 10A discharge on 30Q cells.
```

---
## \#30 Posted by: rey8801 Posted at: 2018-06-24T07:52:05.847Z Reads: 88

```
Funny it is the same vendor I bought mine :sweat_smile: https://www.aliexpress.com/item/32829800932/32829800932.html?shortkey=ZzUZRVvE&addresstype=600
I do not understand then why mine seems not work as it should do.
Did you choose the one with bluetooth only? or also PC?
```

---
## \#31 Posted by: bartroosen12 Posted at: 2018-06-24T07:53:18.933Z Reads: 86

```
Both, bluetooth and pc.
If you really want them at 4.2V charge them seperate with a lithium charge module, like the one in a powerbank. ![1529826940372202724487|375x500](upload://bus0YRDFzNpDEOsrB3hm1b4yvQn.jpg)
You can plug them in the balance connector, very easy
```

---
## \#32 Posted by: rey8801 Posted at: 2018-06-24T07:57:51.013Z Reads: 86

```
I agree that 41V it's ok, It's just wierd that the charger doesn't try to reach 42V and moreover that if I spin the moto one sec so that the bms will allow the charger to start the cycle I see onyl the same led show up, suggesting that the packs are still unbalanced. I do not know what to think, I just don't want to open the battery pack for nothing. That's it.
Do you use it for charging only? I see that it is also programmable
```

---
## \#33 Posted by: bartroosen12 Posted at: 2018-06-24T08:45:27.491Z Reads: 87

```
I also use it for discharging. Yeah you can adjust a lot of settings, actually everything.
![IMG-20180616-WA0013|690x420](upload://hECPkJRCkLd5cddYpr2U4gP5vSl.jpg)
And you can also change the setting via bluetooth in the app so I'm really happy with it. I just like to be able to see every cell voltage, makes everything so much easier :sweat_smile:
These are the settings for my Lifepo4 16S pack
![IMG-20180616-WA0016|690x419](upload://fXkO2rn0GgUWt8JQPVJh5oakFjH.jpg)
I has also 4 temp sensors so you can put one in your battery pack, bms, esc and maybe one close to your motor. But you don't need to connect them, it's just for information or you can set a max temp. value for these.
```

---
## \#34 Posted by: rey8801 Posted at: 2018-06-24T09:17:49.023Z Reads: 83

```
Then I will go for it. If I can program it is the way to go. Thx!
```

---
## \#35 Posted by: rey8801 Posted at: 2018-07-15T15:57:41.349Z Reads: 77

```
Hi! I finally found the bravery of open partially the battery so that I can access to the BMS. I then charged the battery al lteh way up and I am waiting the BMS finish to balance two cells (I can see it becasue it has a led light for each cell lead + that turn one when fully charged). Aftercharging I just checked the cells and these one the results 10s battery:
|1|4.1|
|2|4.1|
|3|4.1|
**|4|4.17|**
|5|4.1|
|6|4.1|
|7|4.1|
**|8|4.13|**
**|9|4.21|**
|10|4.1|


The cells group are out of balance and indeed the leds are on so seems the BMS is working, but why it allowed to get so unbalanced? I will report back in a while but I was wondering to manually discharge the single cells can I connect a small led to the single led pin (the pin that usually connect to the BMS). If it is possible the + wire goes to the unbalanced cell, but the + one should be connected to the B- pin or the pin form the previous cell group? The reason why I am asking it, is because if I measure with a multimeter placing the - probe to the B- lead and the + probe to let's say Cell 9 + lead I get the total Voltage (around 37.8V when fully charged). On the other hand if the - probe to the pin of group 8 I get only the voltage of the single 9 cell group. So I am not sure where to place the - of the light bulb, I do not want to give it to much Voltage.
Thx!
I made this simple circuit for discharge the cell. 
![IMG_20180715_203336|690x388](upload://tAAz4lR41ttIcDJj1J72z0RLBy2.jpg)
```

---
## \#36 Posted by: itsmikeholland Posted at: 2018-07-15T16:19:36.400Z Reads: 73

```
you should seriously consider getting a higher-end BMS and use it to balance discharge. I commute up and down some big hills in LA daily and have never had issues with balance discharging after a year. Best advice to move in this direction would be to see if @barajabali will sell you one of the BMS's he uses. they're fantastic and I can't be sure he doesnt do something special to make them balance discharge at higher amperages.
```

---
## \#37 Posted by: rey8801 Posted at: 2018-07-15T16:25:15.157Z Reads: 73

```
Yeh, I am in EU so if I can find something locally would be better. I do not know why my BMS allowed the cell to get so unbalanced. @bartroosen12 talked about a BMS with Bluetooth that you can set it for higher overcharge protection, plus monitoring the single cell voltage. I like the idea to be able to check it without open the battery. I check all the connections, nickel strips ecc... everything looks good. really solid. I really think is the BMS  :expressionless:
```

---
## \#38 Posted by: kuphjr Posted at: 2018-07-15T16:28:41.488Z Reads: 71

```
Even if you buy a BMS, I am a firm believer that everyone should also buy a hobby charger. BMSs work pretty well, but never seem to work quite as well as a hobby charger. 1-2 times a year it’s a good idea to balance charge your pack with a hobby charger to make sure everything is well balanced. That is why I build 2s li ion packs and connect them with bullet connectors to make a 12s pack. Much easier to troubleshoot and charge with a hobby charger.
```

---
## \#39 Posted by: rey8801 Posted at: 2018-07-15T16:32:03.409Z Reads: 70

```
@kuphjr @onepunchboard @itsmikeholland New results after 1.30h of balancing

|1|4.1||4.12|
|---|---|---|---|
|2|4.1||4.12|
|3|4.1||4.12|
|4|4.17||4.18|
|5|4.1||4.12|
|6|4.1||4.12|
|7|4.1||4.12|
|8|4.13||4.1|
|9|4.21||4.18|
|10|4.1||4.12|
|||||
||Ore 17||Ore 18.26|

Now group 8 it's better the other still not
```

---
## \#40 Posted by: rey8801 Posted at: 2018-07-15T19:21:39.520Z Reads: 67

```
I started to discharge some cells. I am doing like that to be able to monitor it
![IMG_20180715_211944|281x500](upload://1naJGGT1Cob0rEkg482AtbK9O4Y.jpg)
```

---
## \#41 Posted by: onepunchboard Posted at: 2018-07-15T19:41:14.002Z Reads: 61

```
Huh, I thought problem went away.
Good choice manual mode for the win
```

---
## \#42 Posted by: DeathCookies Posted at: 2018-07-15T19:44:17.418Z Reads: 63

```
[quote="rey8801, post:15, topic:59812"]
Do you know a BMS that either I can use it charge and discharge, without the problem of cutting the brakes as I had when my bms was discharge too
[/quote]

Maybe the bms had only 5a charging current and the Regen braking provided more which results in cutting out the brakes?
```

---
## \#43 Posted by: rey8801 Posted at: 2018-07-15T19:55:16.282Z Reads: 64

```
Yeh I will try but since it happens once I am afraid it will happen again after few charges. One of the cell ( cell 8) is lower tha the other may I charge it with this as you said?
![IMG_20180715_215530|281x500](upload://4QHTZ5KxSYC6qsVGlfaK48i3cqB.jpg)

I just need to connect the cell to B+ and B- right?
```

---
## \#44 Posted by: rey8801 Posted at: 2018-07-15T19:58:18.335Z Reads: 59

```
The problem was that when battery nearly fully charged in the first 2 km hard brakes result in BMS cut out to prevent overcharge. So I am now using it for charge only
```

---
## \#45 Posted by: DeathCookies Posted at: 2018-07-15T20:07:46.384Z Reads: 61

```
[quote="rey8801, post:44, topic:59812"]
The problem was that when battery nearly fully charged in the first 2 km hard brakes result in BMS cut out to prevent overcharge
[/quote]

That is only a problem with a >12s battery (50,4v + regen Spikes)
With a 10s you should not have the Problem. I still think the bms had too less charging current ability
```

---
## \#46 Posted by: rey8801 Posted at: 2018-07-15T20:10:05.557Z Reads: 60

```
When I remove the discharge branch than the problem went away. I also have the telemetry data and you see that just before the voltage reached 48V because the BMS cut out and current doesn't know where to go and it's read at the VESC level by the HM-10 module. That what I thought
```

---
## \#47 Posted by: DeathCookies Posted at: 2018-07-15T20:14:44.857Z Reads: 60

```
[quote="rey8801, post:46, topic:59812"]
When I remove the discharge branch than the problem went away.
[/quote]

That means if you do not discharge through the bms it works. That means the bms cannot handle the Regen current? It seems like that
```

---
## \#48 Posted by: rey8801 Posted at: 2018-07-15T20:18:24.645Z Reads: 64

```
ah ok that's for sure. The overcharged protection starts to low. I am now balancing manually the cell and I will give it another try. Otherwise I will change it. I am sick of opening the battery

Some is discharging and some charhing :laughing: it's a mess! 

![IMG_20180715_221854|690x388](upload://6tUAUzin9Wz42Ll5otFfjgmk8eX.jpg)
```

---
## \#49 Posted by: rey8801 Posted at: 2018-07-15T22:53:56.092Z Reads: 54

```
@onepunchboard
Finally! Now we'll see for along they will be stable. Thanks for the help :grin:

![IMG_20180716_005210|690x388](upload://vlFtH1fNfwPGICH6DbnziIm8ADi.jpg)

After one night of final balancing from the BMS

|1|4.16|
|---|---|
|2|4.16|
|3|4.16|
|4|4.18|
|5|4.17|
|6|4.17|
|7|4.17|
|8|4.17|
|9|4.17|
|10|4.17|

Let's see for how long it will last this time...
Thank you everyone for the help!
```

---
