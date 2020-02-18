# Help for BMS wiring and BMS cutoff limits needed

### Replies: 27 Views: 5335

## \#1 Posted by: oyta Posted at: 2017-05-02T22:35:00.806Z Reads: 712

```
## Summary
I have started to buy the parts I need for my first build. Next up is buying battery and BMS and weld it together. I have drawn a wiring schema that you can see below. Parts:

* 190 kv motor
* VESC 6
* 10s3p battery of LG HG2
* BMS Bestech HCX-D223V1 http://bestechpower.com/37v10spcmbmspcbforli-ionli-polymerbatterypack/PCM-D223V1.html

## Battery

LG HG2 Lion battery. Based on some reading this battery should do the job. Hard to find stores who sell good batteries in Norway, but these I found (even though quite expensive). Data sheet: http://keeppower.com.ua/download/2015-06/datasheet-LG_INR18650HG2-1.pdf

From what I read of the battery is "emtpty" when the voltage goes down to 2.5V and it should not charge above 4.29V.

## The BMS

I have looked at the Bestech http://bestechpower.com/37v10spcmbmspcbforli-ionli-polymerbatterypack/PCM-D223V1.html. There are several people stating they use these boards with integrated switches. So I emailed Lucy at Bestech and asked how the recommended to set the parameters for LG HG2 batteries in a 10s3p configuration.

>> What settings would you recommend?
>  
> I recommend over charge detection voltage in 4.25V+/0.05V
>                      Over discharge detection voltage 2.50V+/0.0625V
> Please check whether it is suitable for your project or not.

1. Based on the battery data sheet I would say that the over charge detection voltage should be set lower, to 4.2V. However, should I also have some margins? I.e. setting this parameter to e.g. 4.15V?

2. Over discharge is set to the bare minimum according to the battery data sheet. Should I have some margins on this parameter? E.g. set it to 2.7V?

3. Is release voltage ok to have 0.2 V from the detection voltage? I.e. Over charge release voltage at 4.05V and Over discharge release voltage at 2.7V?

## Wiring and switch
<img src="/uploads/db1493/original/3X/e/a/eac56bed60636aaa794def0c3243f7b71fb3a7c7.png" width="666" height="500">
Two drawings - one with an X90s anti spark to be able to break the loop and the other without.  Does this wiring look sane? :thinking:
 
4. I guess I could do without the X90s or is it needed to disconnect the VESC while charging? According the Bestech BMS information the BMS Switch must be ON while charging! That means that the VESC do have power while charging. As long as the BMS is doing things right I guess that should be ok?

Thanks for any feedback on the wiring, BMS choice, switches and all other!

Edit: Changed the wiring.
```

---
## \#2 Posted by: mptrs Posted at: 2017-05-02T22:46:40.266Z Reads: 578

```
Think there is something wrong.

There should be a P- that will go to the - of the VESC.
And the C- is for the charge port.

https://www.electric-skateboard.builders/t/high-power-10s-lipo-battery-pack-with-bms/10014/72?u=mptrs
```

---
## \#3 Posted by: oyta Posted at: 2017-05-03T06:00:23.840Z Reads: 556

```
Yes - you are correct, @mptrs!  I updated the wiring schema. Thanks :slight_smile:
```

---
## \#4 Posted by: oyta Posted at: 2017-05-03T19:10:47.608Z Reads: 522

```
Does anyone have any experience with LG HG2 and BMS settings? Over charge detection and over discharge settings are preconfigurable on the Bestech BMS.

And - what happens with regenerative power while breaking - will it function with a BMS between the VESC and the battery?
```

---
## \#5 Posted by: mptrs Posted at: 2017-05-03T20:54:57.115Z Reads: 473

```
No problem, happy I could help. I'm in the middle of all this right now as well.

For your other question, maybe @Namasaki can help out. He knows allow about BMS, wiring etc.
```

---
## \#6 Posted by: Namasaki Posted at: 2017-05-03T21:56:09.819Z Reads: 449

```
[quote="oyta, post:4, topic:22263"]
And - what happens with regenerative power while breaking - will it function with a BMS between the VESC and the battery?
[/quote]
The regenitive charging does work with the Bestech bms and it prevents over charging from regenitive brakes.

Some of the parameters of the Bestech bms are adjustable at the factory and can be specified during the order process.
```

---
## \#7 Posted by: oyta Posted at: 2017-05-03T22:01:39.260Z Reads: 414

```
@Namasaki thank you!

I think I will follow the white paper and set the over charge detection voltage to 42V.  The over discharge I will set to 25V.

For more control during use I can use the cut off on the VESC for discharge. I will buy a charger that goes to 41V: http://www.groetech.de/index.php?main_page=product_info&products_id=837

This way I will stay clear of the upper and lower voltage limits of the battery.
```

---
## \#8 Posted by: treenutter Posted at: 2017-05-04T14:39:59.627Z Reads: 404

```
[quote="oyta, post:1, topic:22263"]
Based on the battery data sheet I would say that the over charge detection voltage should be set lower, to 4.2V. However, should I also have some margins? I.e. setting this parameter to e.g. 4.15V?
[/quote]


I agree w this but make sure that the charger you use doesn't contraindicate the over-charge detection threshold you've chosen... if the charger is charging to 4.2V but your BMS cuts off at 4.15V that wouldn't be good...
```

---
## \#9 Posted by: oyta Posted at: 2017-05-04T19:46:24.069Z Reads: 375

```
Good point! So maybe 4.25V over charge is ok. I will keep the settings as Bestech recommended with 4.25 Volts over charge and 2.5 Volts discharge.
```

---
## \#10 Posted by: tonystark Posted at: 2017-05-08T20:13:10.314Z Reads: 360

```
Hey, I tried to buy BMS from the website following that link that you shared but it seems like there is no option to buy. Can you suggest me how does it work? BMS is the only thing that holds be to finish my longboard. thanks mate
```

---
## \#11 Posted by: oyta Posted at: 2017-05-23T19:57:04.633Z Reads: 341

```
I communicated with Lucy at lucy@bestechpower.com. Hope she is real because I ordered two! :) I can give you a heads up if I ever get the BMSes :wink:
```

---
## \#12 Posted by: oyta Posted at: 2017-06-02T06:01:44.601Z Reads: 330

```
@tonystark I just received the BMSes! So you can contact Lucy and order through her.
```

---
## \#13 Posted by: Youssless Posted at: 2017-06-06T08:23:10.931Z Reads: 324

```
Hey, sorry to necro this but I noticed that your schematic with the loop key is connected to the positive wire. This is fine if you're wiring it to the female connector but if you're using a male you should connect it to the ground wire instead to prevent damage/injury if you or someone accidentally touches the exposed parts of the male connector.
```

---
## \#14 Posted by: TunaTee Posted at: 2017-09-26T13:25:17.652Z Reads: 273

```
Hello, can you post a build picture of your final product?
```

---
## \#15 Posted by: Lionpuncher Posted at: 2017-09-26T14:58:47.427Z Reads: 266

```
 Had anybody adjusted any factory parameters in the comfort ood their own home? Or is it kinda like once those settings are set that's it?
```

---
## \#16 Posted by: oyta Posted at: 2017-09-26T16:01:06.638Z Reads: 269

```
http://www.electric-skateboard.builders/t/portable-custom-birch-fiber-glass-enertion-trucks-6355-190-kv-enertion-motor-mount-10s3p-lg-hg2-vesc-6-beta/26397
```

---
## \#17 Posted by: TunaTee Posted at: 2017-09-26T16:12:57.075Z Reads: 264

```
<img src="/uploads/db1493/original/3X/6/a/6ae7592f95ee479f4e5072780973d13976cba078.JPG" width="666" height="500">
Can you please look over my design? Did I get it right?
```

---
## \#18 Posted by: Namasaki Posted at: 2017-09-26T16:17:09.414Z Reads: 253

```
The parameters are factory set. 
You have to request them when ordering the bms. 
This is the case with Bestech
```

---
## \#19 Posted by: Lionpuncher Posted at: 2017-09-26T16:39:55.128Z Reads: 246

```
Ok thanks @Namasaki.
```

---
## \#20 Posted by: mynamesmatt Posted at: 2017-11-15T01:34:30.990Z Reads: 224

```
@TunaTee    
Before you dive in to building an electric skateboard, you should do some fundamental research on the basics of electronics. Not having an understanding of these basics can have a serious effect on the overall performance of your board.
To answer your questions:
1. The voltage meter (voltmeter) sits across your positive and negative wires. In your case, the voltmeters positive wire should connect in parallel to the positive wire of your battery 1, and the negative wire of your voltmeter should connect in parallel to your negative wire of your battery 3.
2. I dont know what you're after here
3. Yes, the thickness of the wire has an extreme effect of the flow of electricity. If you have a 1mm wire with 80A of current flowing through it, it will melt the wire. I recommend checking what amount of current you will have flowing through the wire and then buy wire that is rated at that voltage and amperage.
Hope this helps
Matt
```

---
## \#21 Posted by: clvnng Posted at: 2017-12-12T18:22:38.150Z Reads: 203

```
@oyta thanks os much for providing your BMS wiring diagram that helps alot. 
I just had one question, how is your regen breaking working? When the battery is fully charged does it regen break well still? 
I read some horror stories of BMS's cutting off and they have to bypass the BMS for discharge and only use it for charging.
```

---
## \#22 Posted by: Zen Posted at: 2017-12-16T21:38:46.903Z Reads: 200

```
Hi my BMS isn't discharging properly. Can anyone tell if this chip error might be a cause? Thanks.
<img src="/uploads/db1493/original/3X/c/2/c2e5fef15721908199606f47fc909186b537e915.jpg" width="634" height="500">
```

---
## \#23 Posted by: Redfire1 Posted at: 2018-04-23T21:07:36.948Z Reads: 155

```
![image|666x500](upload://fW1svt2mE6xRfSiLTrUeV2vEwTs.jpeg)![image|375x500](upload://g6WL22kPio7ud6d0KgSMKHe1Qxp.jpeg)![image|375x500](upload://B4GDDptr80b4WI9hDII92Dx4rR.jpeg)![image|375x500](upload://5DrLOx5jEy5Tf7WWbkhHsYPxEh1.jpeg)![image|375x500](upload://tS423BkwH32by7kLTxzDVeVEvEr.jpeg)![image|374x500](upload://xQmbcPeELyq0xB4YKGCqqaGpYEp.jpeg)
```

---
## \#24 Posted by: longboardshort Posted at: 2018-05-26T17:25:06.218Z Reads: 129

```
When installing bms for first time, should lipos be fully charged or at storage charge? They’re brand new and came at 30%
```

---
## \#25 Posted by: MannyM0E Posted at: 2018-05-26T22:09:36.360Z Reads: 128

```
On my lipo I made sure they were fully charged before installing the BMS
```

---
## \#27 Posted by: Narnash Posted at: 2018-07-11T11:40:06.936Z Reads: 108

```
I guess you already finished your battery setup, but just in case it might help someone else.

When you connect your LiPo (the same thing for Li-Ion) to a BMS, you should ensure at first that they are not faulty of course, and than that they are balanced. It doesbt really matterif they are fully charged to 4.2V (4.1V) or all balanced to maybe 3.85V, just the same Voltage (+/- 0,05V max.)
```

---
## \#28 Posted by: CanadianBacon Posted at: 2019-07-23T22:50:31.354Z Reads: 20

```
Hi im having trouble installing my lithiumbatterypcb 12s 60A bms. I tried contacting the company but one week and no response so im asking here.

I have C- and P- connected to negative wires to xt60 connectors.
I have B- connected to the negative of my battery.

Next I try to solder the balance wires. The bc0 wire is black so I solder it to the negative of my pack alongside the B-.
However... When i touch the bc1 wire to the series connection 1 it makes a high pitch noise from my bms. 

My bms also has bc15 as a red wire. When I connect that to the positive I see the light on the Bluetooth flash for a second and it makes a spark. But still when I connect bc1 after back to the high pitch noise which is worrying. 

Here's a short video to try help explain.

[details="Summary"]
[https://photos.app.goo.gl/gFKbLTFnitHXDyzG9](google drive link)
[/details]

maybe i need to connect positive wires from c- and p- first.. or maybe my bms works backwards starting from bc15...
or maybe its simply that the bms only handles 60A and my battery is 12s3p samsung 30q...

**SOLVED**

so it turns out. 
i had to connect the positive from the c- and p- first and then the bc15 wire which was red. then the bluetooth on my bms turned on.

Then I had to solder the wires backwards from bc14 - bc13 - ... - bc1 and then finally it worked!!! lol
would have been nice if the manufacturer of my bms told me that or had instructions on their site or shipped with bms but whatever it turned out ok.
```

---
