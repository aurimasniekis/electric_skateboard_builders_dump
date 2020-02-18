# Is this BMS OK for 2 of these batteries in series?

### Replies: 7 Views: 1462

## \#1 Posted by: svenboard Posted at: 2017-09-05T01:34:29.815Z Reads: 93

```
Hey there,

Thanks for the great community!

I've been reading up everything I need to know for my build but I cant find one last piece:

BMS (Battery Management Systems): Not much information out there on which ones to get, if they're even needed etc.

I'm wondering if this BMS: https://hobbyking.com/en_us/6s-li-ion-10a-pcm.html would work with two https://hobbyking.com/en_us/multistar-high-capacity-6s-16000mah-multi-rotor-lipo-pack.html


Planning on running that together with an esk8 mosfet vesc and a 192 6374 motor.
```

---
## \#2 Posted by: krloz Posted at: 2017-09-05T08:05:25.096Z Reads: 82

```
Packs in series add up voltage and the number before the s
Packs in parallel add capacity and c rating and the number before the p
So two 6s packs in series equals a 12s pack
And that bms is for 6s not 12s
So, no
 Are you after a 6s setup or a 12s setup?

Edit. Without question mark it ain't a question
```

---
## \#3 Posted by: Yecrtz Posted at: 2017-09-05T10:29:46.071Z Reads: 68

```
If you are using only one of those batteries at a time, yes. 6s bms will work with a 6s battery. If you put them in series, like @krloz said, you get 12s. In that case it'll not work and you will need a 12s bms.

Also, the max discharge is 10a, unless you want to bypass the bms for discharging, that's too low.
```

---
## \#4 Posted by: svenboard Posted at: 2017-09-07T01:17:36.965Z Reads: 45

```
OK. So I guess this would be a better option: http://www.batterysupports.com/44v-48v-504v-12s-80a-12x-36v-lithium-ion-lipolymer-battery-bms-p-392.html

But could I go down to 60a?

Motor has peak 80a, if I use a 60a discharge, do I cap the motor then?


Im after a 12s 16000mah+ setup btw. And I am running a single Turnigy SK3 192KV 6374
```

---
## \#5 Posted by: krloz Posted at: 2017-09-07T09:19:00.292Z Reads: 43

```
It depends if you are planning on going above 60 BATTERY amps for more than quick bursts. Then if you are using the bms for discharge it will reboot your esc And that is bad.
```

---
## \#6 Posted by: Tomash Posted at: 2017-09-07T13:44:10.644Z Reads: 40

```
You got 16 Ah 12S battery, and motor with peak current of 80A. 
If you plan to use VESC with this setup (you probably are since 12S is 50V), you can always set the limit to current from battery in vesc setup.

Just put **battery max** value in the safe mode at around **40 (40A)**, and **motor max** to your motor value: **80A**
And **40A** for the battery max, since vesc, at least **4.12 hardware one**, cant handle more than 35-40A continous current, before going nuclear.

**About BMS**. For your motor type, it would be best to get BMS 12S, with 80A discharge and 10A charge.

I recently made 2 e-skates, with the same type of battery/ capacity, (but 2x4S), and i use **8-20S BMS.** 80A discharge/10A charge
This bms can go with 8S as well as 20S. i use it with 8S, 33,6V at it works perfectly. It's BMS i bought in some e-bike store in my country.
I have twin vesc's, and two motor 6364 outrunner 245 kV,. Each motor is rated for 70A.

I setuped each vesc with: **70A - motor max, and 40A battery max**, and it works great, nothing overheating, nothing shuts down.

Here is **[the link](http://www.electric-skateboard.builders/t/first-build-twin-sk3-6354-260-kv-trampa-urban-carver/25856/12)** to my build thread. Maybe it will help you.
```

---
## \#7 Posted by: svenboard Posted at: 2017-09-07T17:46:22.362Z Reads: 26

```
Guys/Gals: Thank you, this is really awesome help!

I might get back to one of you when its time to wire the stuff!

Love you guys, thanks!
```

---
