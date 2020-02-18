# Xiaomi m365 changing bms

### Replies: 35 Views: 26121

## \#1 Posted by: chickengun Posted at: 2018-04-02T18:51:59.301Z Reads: 405

```
Hi,
this is more like a e-scooter question, I hope someone can help me out.

I have a Xiaomi m365 scooter which doesn't charge anymore. After a ride (I almost emptied the battery) I opened it and checked the voltages of the 10s3p battery. All looking good. I get 36 V over all 18650 batteries in series and 3.6 V on all 3p cells, however when this goes through the bms the output voltage is only 17V (this 17V goes to the controller board), so there is something wrong with the bms as this should be 36V (or 42V fully charged). In fact there are two LED's that are supposed to blink on the bms but I don't see anything blinking. I read in most cases there is a bad welding spot on the battery pack or a Z fuse has blowen, but it was not the case for me..

All the components on the bms are looking good. I checked both Z fuses and also the big components that are crucial for the power supply (some mosfets and Schottky diodes) but they seem to be ok. The only thing I found suspicious is the BMS chip (BQ7693003). I couldn't touch it as it was very hot! I believe it is over 100 °C or in that range. I think this is not normal... That's why I desoldered the red wire from the battery pack as I don't want it to be hot all the time...

Buying some of these components (bms chip?) will take some time to arrive (from china) and I wouldn't be sure if this will fix it. As I need a fast solution (I don't have another escooter nor esk8 ready yet...) why not buying a bms and replacing it with the stock one?

My question: Do you think this will work? Xiaomi has a Firmware for the bluetooth board, the bms board and the controller board. I am not sure, if I change the bms will the system still run? I don't care about using the app I just want to use the scooter for the next few weeks until I get a new one. What are your thoughts?
```

---
## \#2 Posted by: kelomen Posted at: 2018-04-04T13:57:41.633Z Reads: 346

```
Hi !
I' have the same issue described by you...where you able to find anything? tks!
```

---
## \#3 Posted by: chickengun Posted at: 2018-04-04T19:29:48.917Z Reads: 317

```
No I didn't find the time. But maybe we can try to fix it... Can you please describe precisely how you encountered this issue? Also, is the BMS chip (BQ7693003) hot in your case?

Please read [this](https://smarthomesguides.com/xiaomi-mi-jia-m365-electric-scooter-review-designperformanceproblems/), you will find there very good information.
```

---
## \#4 Posted by: chickengun Posted at: 2018-04-04T19:38:57.965Z Reads: 312

```
This here is the D9 schottky diode that I thought was causing the issue. With my multimeter (diode test mode) I tested if there is a shortage, and it was! The two red dots here are shorted:
![20180404_212835_resized|281x500](upload://9j2g1IuppwsnlvNhnZvsVMQIGTf.jpg)

After I desoldered this component I noticed that the pcb is designed that way... so xiaomi used a dual schottky diode to get 2*5A=10A... So this is probably not the component that is defective... I tested all three big mosfets and they seem to be OK too.
```

---
## \#5 Posted by: dzsonni Posted at: 2018-04-18T08:03:01.235Z Reads: 257

```
Hello,

I am facing a similar issue. The battery control board seems to be completely dead but I can't seem to find the faulty component. The cells are intact and they output 36V as they weren't fully charged before the fault. Did you manage to find a solution yourself or does anyone know if you can actually order just the pcb from xiaomi? I wrote to their global service but no response so far.
```

---
## \#6 Posted by: Silverline Posted at: 2018-04-18T09:38:42.919Z Reads: 241

```
Have you guys seen this https://youtu.be/9cdZOjROdBM
```

---
## \#7 Posted by: chickengun Posted at: 2018-04-18T19:47:21.600Z Reads: 226

```
yes I saw that video. This guy replaced his Z fuse, but in our case it's unfortunately something else.
```

---
## \#8 Posted by: chickengun Posted at: 2018-04-18T19:55:41.409Z Reads: 218

```
Sorry I didn't find the time to investigate yet :frowning:
You can't order a pcb from xiaomi, you can only buy the full battery pack (that comes together with the bms).
```

---
## \#9 Posted by: losip Posted at: 2018-05-23T18:12:30.809Z Reads: 214

```
Please remember that the Texas Instruments BQ76930 BMS chip is customized by Xiaomi. You can't just fit another one - even if you have a rework station that will handle these delicate SMD chips.

95% of the time that you have 36v from the battery but only residual voltage from the BMS is because the BMS has switched off the power due to a perceived fault. Many will be aware of problems caused by one of the 11 cell monitoring connections being broken under vibration. Just because there is 36v from the battery does NOT mean that all the connections are intact.  All of the monitoring and thermistor connections must be intact, too.

There are a few other common faults. I have one on the bench now where an amateur has tried to repair the BMS card and snapped the ribbon cable, breaking many of the monitoring connections. Not a lot I can do about this but the customer does have a working BMS board with nowhere to use it.
```

---
## \#10 Posted by: chickengun Posted at: 2018-05-24T17:18:06.381Z Reads: 186

```
This here seems to be interesting (use google translate):
http://wiki.myelectricscooter.org/fr/xiaomi_mijia/xiaomi_mijia_m365#remplacement_d_un_bms_xiaomi_par_un_bms_generique

I will order this bms: https://fr.aliexpress.com/item/Mayitr-1pc-10S-36V-37V-16A-Li-ion-Lithium-Battery-BMS-PCB-PCM-Suitable-For-Ebike/32825891301.html?spm=a2g0s.9042311.0.0.J8Sl6Q&aff_platform=link-c-tool&cpt=1527182218651&sk=rNJiaeI&aff_trace_key=47a1030d1525453ea49a538516f3db97-1527182218651-01665-rNJiaeI&terminal_id=a9dbdc5524fe4af9bce845a8df0d9086
and this motherboard: https://nerch.en.alibaba.com/product/60757014408-805536253/replacement_motherboard_for_xiaomi_mijia_m365_scooter_parts.html?spm=a2700.icbuShop.89.3.204e5876WcLOUR

Will try to fix it that way. You can't use the xiaomi app but if it's charging thats fine to me.
```

---
## \#11 Posted by: losip Posted at: 2018-05-24T18:15:01.850Z Reads: 170

```
There are so many errors of fact in that wiki article that I'm not sure I would trust the instructions on using a generic BMS board. As indicated, this would need a special controller board that can operate without a data connection from the BMS. It's not clear to me that the Nerch components have been re-engineered to cater for a generic BMS. The alibaba web site only claims that they are replacement parts and I would assume they are identical to the original Xiaomi parts

I hope it's not the case, but you could be wasting your money that could be put towards a new battery assembly.

Good luck!
```

---
## \#12 Posted by: BotoX Posted at: 2018-07-13T21:12:07.350Z Reads: 162

```
How about an open source BMS?
https://github.com/BotoX/xiaomi-m365-compatible-bms
Using this for the past few weeks with 12S battery on the original M365 controller.
Bought the BMS from here: https://www.lithiumbatterypcb.com/product/13s-48v-li-ion-battery-pcb-board-54-6v-lithium-bms-with-60a-discharge-current-for-electric-motorcycle-and-e-scooter-protection-2-2-3-2-2-2-2-2/
You don't need the bluetooth and PC interface that comes with it.
```

---
## \#13 Posted by: Sisqoboy Posted at: 2018-07-14T20:19:11.567Z Reads: 147

```
Hi there, 

I have the same symptoms like yours. How did you solve the problem?
```

---
## \#14 Posted by: Sisqoboy Posted at: 2018-07-14T20:29:46.622Z Reads: 141

```
Could you help me please? My bms or ribbon cables are broken. Bms has only 4 red flashes. On that website you ordered from can we order one for the original xiaomi m365 batteries? Will that work and doesn't have to activate it or do some firmware thingy?
```

---
## \#15 Posted by: chickengun Posted at: 2018-07-17T17:32:25.203Z Reads: 128

```
For me there is no LED flashing at all, I haven't find the solution. That's way I decided to replace the whole mainboard and bms. Still waiting for my mainboard to arrive,I bought it at alibaba and the tracking is saying its still on its way, no new news since mid June though...... I believe they lost it...
```

---
## \#16 Posted by: pitslz Posted at: 2018-11-24T16:56:28.798Z Reads: 113

```
@BotoX where do you upload this custom firmware?
```

---
## \#17 Posted by: inys Posted at: 2019-02-24T22:05:26.661Z Reads: 102

```
I had the same issue, only red LED blinking, 20v on BMS output. But everithing seems to be fine on BMS and battery. Finaly i found that it vas broken little black cable on secondary temperature sensor locatet on the battery. In my case no need to change BMS. Not yet :slight_smile:
```

---
## \#18 Posted by: chickengun Posted at: 2019-03-02T17:42:34.252Z Reads: 98

```
So I ended up replacing the BMS with one from aliexpress and when I changed it it worked for a minute but than the LEDs stopped flashing again... Then I notied the ribbon cable is causing the problem that is connected to the batteries, probably just a loose connection. When I applied some pressure on the ribbon cable it worked again...
```

---
## \#19 Posted by: ron Posted at: 2019-03-03T13:52:40.180Z Reads: 87

```
So the BMS from Ali is working now?
```

---
## \#20 Posted by: chickengun Posted at: 2019-03-03T13:54:22.358Z Reads: 85

```
This one is working: https://de.aliexpress.com/item/New-Outer-Inner-Tube-Pneumatic-Tyre-Accessories-for-Xiaomi-Mijia-M365-Electric-Scooter-Tires-Tyres-8/32815889093.html?spm=a2g0s.9042311.0.0.27424c4dQtJ6q8
```

---
## \#21 Posted by: chickengun Posted at: 2019-05-07T18:43:59.136Z Reads: 69

```
Update: After flashing BMS107.bin using the m365 downG app for experimenting reasons the scooter is now beeping 2 times long and 2 times short. This is the "bad bms password" error code. Strange. After flashing back BMS115.bin (the one I had before) same beep sounds... I checked the battery connections and bms board, seems to look good.

What I noticed when flashing is that at 97% the scooter turns off, than after 2 seconds the m365 downG app goes to 100% and says done. I suspected bad firmware flashing but for [this guy](https://www.youtube.com/watch?v=3MAXu0UVl3s&feature=youtu.be&t=60) it shows the same behavior in his video so I guess it's fine.
```

---
## \#22 Posted by: chickengun Posted at: 2019-05-08T13:51:45.392Z Reads: 68

```
For those who have a clone bms board from aliexpress that are dealing with my described error code you can use [this](http://www.mediafire.com/file/rsi037zbgg9ijc0/BMS115fix.zip/file) app together with the modified BMS115 firmware to force write the correct uid. CAUTION: Don't use the app you find on google play, otherwise you will brick your bms! This is a modified app and modified BMS115 just for the described error code. It worked for me.
```

---
## \#23 Posted by: czchoze Posted at: 2019-05-13T09:05:27.118Z Reads: 61

```
Hi friends. I have realy rare problem with my m365 BMS. The BMS works and reports unbalanced cells. BMS reports: cells 1-8 are 3.95V, cell 9 is 4.1 and cell 10 is 3.65V.  The problem is, that the realy voltage on the cells (measured by voltmeter) is the same about 3.95V. So the battery is balanced, but BMS reports bad values. Have someone an idea? Thank you very much
```

---
## \#24 Posted by: Bredli Posted at: 2019-06-25T21:34:02.685Z Reads: 55

```
Thank you for your bms fw. I had same problem when I changed BMS.
```

---
## \#25 Posted by: Nand Posted at: 2019-07-28T14:43:22.639Z Reads: 46

```
I also replaced my dead m365 BMS with an AliExpress part and everything initially worked OK until the user (a family member who wishes to remain anonymous) decided to upgrade the firmware to 152 which triggered the 2-2 error.

Since the base post is more than one year old (April 2018) I just would like to be sure that this fix still works without any unwanted side-effects.  It just resets the "BMS password" I hope, nothing else?
```

---
## \#26 Posted by: Mr.Blaze Posted at: 2019-08-05T09:32:23.072Z Reads: 43

```
Hello guys, my batteries are working fine. Since i have 2 M365, have any of you tried to change it for 12S battery? And which BMS did you use? If not, what do you think about that idea?
```

---
## \#27 Posted by: Surfer Posted at: 2019-08-05T12:11:43.719Z Reads: 43

```
Motor side no problem, but you will play to the Russian roulette when connect 12s to the esc, maybe magic smoke happens, usually 1s more convenient to not reaching the limits.
```

---
## \#28 Posted by: Fuzzdnb Posted at: 2019-08-06T17:30:25.770Z Reads: 42

```
I have the same 2-2 bms password issue after updating to firmware 1.5.2. With a xiaomi m365 scooter but with a different battery since the original one was not working.
How can i solve this step by step?
```

---
## \#29 Posted by: Nand Posted at: 2019-08-06T19:39:00.974Z Reads: 44

```
I downloaded the tools "chickengun" mentioned in his May 8 post but it did not work.
The com.m365downgrade-v7_PATCHED_BMS.apk app connects to the scooter and is able to retrieve its status but the BMS115fix.bin flash process stalls after 2% and exits after 10 retries.
```

---
## \#30 Posted by: ron Posted at: 2019-08-06T20:10:41.703Z Reads: 44

```
Here you go.

Botox did a 12s4P upgrade with a flashable 12s BMS.

Here The Link to his github Project page: https://github.com/BotoX/xiaomi-m365-compatible-bms

And here some pics of his battery: https://cloud.botox.bz/apps/gallery/s/94drnBJfjacBDnr
```

---
## \#31 Posted by: Ulysse Posted at: 2019-08-21T15:22:46.529Z Reads: 38

```
Hello, excuse me, 
I have the same concerns as the previous messages... 2bips long, 2 short beeps.
Have solutions been found since? thank you so much for any information !

Regards
```

---
## \#32 Posted by: Stapi Posted at: 2019-08-22T13:37:05.584Z Reads: 30

```
I have same issue. Have you found out what was that?
```

---
## \#33 Posted by: teddysurf Posted at: 2019-09-06T20:49:53.976Z Reads: 25

```
 I know this is months old and you probably won’t see this but I just wanted to say thank you because this fixed my error 22 that I was trying to figure out for two weeks. I’ve never had sexual thoughts towards a man before but you’ve come the closest...
```

---
## \#34 Posted by: Chris-H Posted at: 2019-10-14T19:08:15.796Z Reads: 17

```
On the BMS board is a micro reset button located near the top. No need to remove water seal. just pierce the seal near the button and press it. I used a micro screwdriver for this. a cocktail stick or similiar should give enough leverage to press it. Afterwards you should get a slow flashing blue LED after reset. If it flashes red, there remains some other BMS issue that requires further investigation.
```

---
## \#35 Posted by: Chris-H Posted at: 2019-10-14T19:11:04.712Z Reads: 17

```
Put the original battery back in. Then diagnose from there.
```

---
