# Question about BMS and power supply

### Replies: 13 Views: 4997

## \#1 Posted by: Hillso Posted at: 2016-07-02T00:11:41.946Z Reads: 287

```
What power supply do I need to use voltage wise?
For example if want to use 8s bms with lipo, so it's 29.6V nominal and 33.6V max , can I use 30V or 35V power supply? or I can use only 33.6 power supply? Thanks.
```

---
## \#2 Posted by: lox897 Posted at: 2016-07-02T02:52:14.311Z Reads: 287

```
You would use the power supply with the same voltage as you batteries fully charged. Example: 10S = 42v fully charged so you use a 42v power supply.
```

---
## \#3 Posted by: Hillso Posted at: 2016-07-02T12:33:20.402Z Reads: 271

```
Thanks.
Do you I can trust this BMS 10A charge current, or will it burn my house?
http://www.aliexpress.com/item/High-Quality-Brand-New-Battery-Protection-BMS-PCB-Board-For-10-Packs-36V-Li-ion-Cell/32597003264.html?spm=2114.01020208.3.56.AOh3xo&ws_ab_test=searchweb201556_7,searchweb201602_4_10037_10017_405_507_10033_406_10032,searchweb201603_3&btsid=297a21a0-f748-4586-8bbe-3a42e95615a3

I'm buying 33.6V 10A power supply from this seller: http://www.aliexpress.com/item/High-Quality-Brand-New-Battery-Protection-BMS-PCB-Board-For-10-Packs-36V-Li-ion-Cell/32597003264.html?spm=2114.01020208.3.56.AOh3xo&ws_ab_test=searchweb201556_7,searchweb201602_4_10037_10017_405_507_10033_406_10032,searchweb201603_3&btsid=297a21a0-f748-4586-8bbe-3a42e95615a3
```

---
## \#4 Posted by: lox897 Posted at: 2016-07-02T12:50:40.884Z Reads: 248

```
You can't charge with 10 amps unless your batteries can handle it. What batteries and configuration do you have? You could use that BMS just for charging and then bypass it for discharging.
```

---
## \#5 Posted by: Hillso Posted at: 2016-07-02T13:00:47.762Z Reads: 247

```
I plan to charge 8s2p 5.5A Lipo (11A) so it will be roughly 1C at 10A.  And I plan to bypass for discharging, but I'm scared this is too much for the little bms (altough it's rated for 10A charging).
```

---
## \#6 Posted by: lox897 Posted at: 2016-07-02T13:05:31.744Z Reads: 243

```
If you want a really reliable BMS get it from BatterySupports or Bestech Power.
```

---
## \#7 Posted by: Hillso Posted at: 2016-07-04T19:33:09.121Z Reads: 227

```
I don't need a reliable, high amp BMS because I use it only for balance charging (correct me if i'm wrong).
Do I need a switch between the BMS and the battery, or can the battery and the bms be connected when not charging?
I think I heard that I need only  one 8s BMS if i have 8s2p lipo, is that true?
Thanks a lot for the help.
```

---
## \#8 Posted by: lox897 Posted at: 2016-07-04T23:34:17.490Z Reads: 208

```
1. I don't need a reliable, high amp BMS because I use it only for balance charging (correct me if i'm wrong).

You can never be to careful when charging lipos. Be careful when charging. You do not need a high amp BMS.

2 Do I need a switch between the BMS and the battery, or can the battery and the bms be connected when not charging?

You don't need a switch.

3. I think I heard that I need only one 8s BMS if i have 8s2p lipo, is that true?

Correct
```

---
## \#9 Posted by: AndyL Posted at: 2016-12-21T16:45:28.044Z Reads: 164

```
Hey there @lox897 ! Stumbled upon this thread while researching  on BMS. Mind educating me on what amp I should be looking for when buying a BMS? Does a BMS enable me to have a laptop-style charging? I would be using 2 x Zippy 3S 5000mAh LiPo batteries connected in series to give a 6S.
```

---
## \#10 Posted by: Alextech Posted at: 2016-12-21T16:56:02.610Z Reads: 164

```
@AndyL You will want your BMS to be overall to be under the max discharge current of your battery for example.  A 10s3p 25r will yield 60a continuously, but you should get a 50a continuous BMS if you'd like to have the protection of if a cell fails the BMS will take care of such same with lipo.  But lipos tend to have higher discharge rates compared to 18650, this means you can use a much higher bms, personally I think you'd probably never go above 80a. Also  Unfortunately the bms on Hobby King would overvolt the lipos which can be very dangerous lipos should never be overcharge to more then 4.225 volts each cell. A BMS can be used for lipo as so long it has overvoltage is under 4.225v with the tolerance (ex.  +-.025) the bms listed would overvolt to 4.3v

Yes most laptop style chargers are what is used for bms with the right connections,  you can find them at Radio shack if your in the US 😊
```

---
## \#11 Posted by: AndyL Posted at: 2016-12-22T18:12:32.718Z Reads: 149

```
Thanks alot for your swift response :slight_smile: Would these work ? BMS (http://www.batterysupports.com/22v-24v-6s-60a-6x-36v-lithium-ion-lipo-battery-bms-pcm-pcb-p-478.html)
Charger:(http://www.batterysupports.com/liion-lipo-252v-222v-2a-6s-wall-socket-battery-charger-ac-dc-p-135.html)
How does one calculate the continuous current? My batteries are 3s Zippy 20c 5000mAh LiPos if it helps.
Also, how would I go about enabling the charger to work? (Like installing the charging port and wires) A link would be great (can't seem to find the answer on this forum) Lastly, what do they mean by charge/discharge? Seen several ppl talking about just using BMS to charge or something like that. Sorry for the questions, really appreciate the help T.T
```

---
## \#12 Posted by: Bibzz Posted at: 2017-11-10T08:36:00.490Z Reads: 75

```
i have a similar question. I'm trying to built a 8s2pbattery pack with Samsung 18650 25r (http://www.18650batterystore.com/18650-Batteries-s/106.htm) but not sure what bms to use please help! The 30a..45a...60...? Not sure how the "a" works ?  i want to change, discharge and balance?
i would very much appreciate the help!!!
```

---
## \#13 Posted by: Lorenz1 Posted at: 2018-10-29T22:13:52.727Z Reads: 29

```
Cant I just use a Power supply that has the same or HIGHER Voltage than the fully charged voltage of the pack? Becouse most bms have a overcharge protection.
```

---
