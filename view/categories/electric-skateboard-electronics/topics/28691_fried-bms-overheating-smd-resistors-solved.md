# Fried BMS? Overheating SMD Resistors \[SOLVED\]

### Replies: 16 Views: 2542

## \#1 Posted by: rakejagland Posted at: 2017-07-26T14:24:07.632Z Reads: 132

```
OK, so I have not found any other topics that are in line with my problem. The last assembly to my build is wiring the BMS for just charging. I'm bypassing it for discharge. It seemed fairly simple, but when I turned the power on after charging for a little bit, It started to smell super hot. I immediately powered down and saw that one of the tiny resisters for one of the balance wires was very hot and slightly charred. You can see in the picture below.<img src="/uploads/db1493/original/3X/0/a/0aa2eb168c9144d6f28f8a8c3830bb2f7e000344.jpg" width="666" height="500">
It is the 4th cell of my 8S battery series. It is an 8S BMS and here are the links to the batteries and charger I used.
Charger: https://www.amazon.com/HEBANG-Three-stages-Lithium-Battery-interface/dp/B01IEB8V6Q/ref=sr_1_1?s=industrial&ie=UTF8&qid=1498402374&sr=8-1&keywords=22.2V+lithium+battery+charger
Batteries: https://hobbyking.com/en_us/turnigy-5000mah-4s1p-14-8v-20c-hardcase-pack.html
BMS: https://hobbyking.com/en_us/8s-li-ion-pcm-charge-4a-discharge-10a.html

I followed the guide for my  BMS provided on the BMS website (excluding discharge) and I wired the balance wires according to tutorials on YouTube. (Wired 8 through 1 starting with the positive wire of first battery, skipping positive of second battery in series and wiring the last negative to B-)

It is surprising that it overheats when the charger is disconnected and the power switch is on because it should be wired for only balance charging and not discharging. The P- is left alone. I just wired the B- and C-. Also confused as to why it just overheats one of the series of resistors and not all of them. Is this a hardware problem or did I wire something wrong?
```

---
## \#2 Posted by: Namasaki Posted at: 2017-07-26T14:54:50.634Z Reads: 119

```
From your description it sounds like you wired it incorrectly. 
Can you provide a diagram of how
 You wired the batteries with the bms including the mains and balance leads?
```

---
## \#3 Posted by: rakejagland Posted at: 2017-07-26T15:49:52.689Z Reads: 113

```
@Namasaki Yes, I followed the general instructions from this vid: https://www.youtube.com/watch?v=F_paouc06Cg&t=144s

Here is a diagram of my wiring: <img src="/uploads/db1493/original/3X/c/d/cd1ad2135e719ed19e3a80bbceb2f79c0648d2b7.jpg" width="690" height="292">

Overheating occurs on resistor following the path of the 4th balance cable. (B8 is on top)

Thanks
```

---
## \#4 Posted by: JdogAwesome Posted at: 2017-07-26T16:07:23.088Z Reads: 101

```
Well those resistors are for balancing the individual cells so it could have possibly been that your cells are like seriously un balanced, I would check that first. Also it could be a faulty BMS and you might need to get a new one if you can't fix it, but that's a last resort.
```

---
## \#5 Posted by: MontPierre Posted at: 2017-07-26T21:55:15.180Z Reads: 92

```
I have very similar problem. I'm very certain that my wiring is correct - see diagram ( bypassing discharge) . I have just connected my Ebay BMS and even without power supply it got very hot and started smelling ( is it normal to get how without power supply connected? ) . No damage on the surface but I'm getting concerned. 

<img src="/uploads/db1493/original/3X/b/4/b41f0b28d400e6ca4d8af3fec67d06fe0255f8b6.png" width="405" height="500">


Brick charged is giving 41.8V as well but it turns green when connected.

Batteries as whole - 10s lipo ( 2x3s + 2x2s)- are currenlty 37.8V together as a pack. 

Here is my BMS


----------


<img src="/uploads/db1493/original/3X/1/5/159bd691b7bc73f78cba99d7373181da98679938.JPG" width="375" height="500">

and supplied diagram 

<img src="/uploads/db1493/original/3X/3/7/37847227d4d5a88a340936189674f020c750d23c.jpg" width="649" height="500">

<img src="/uploads/db1493/original/3X/9/3/93b7d8f52933144b4d6a26c64e21f8af82a28ef7.png" width="667" height="500">



----------



I know it costed only £8 but I was hoping I'll get at least few weeks out of it haha.

I have just checked cells  voltage it looks like my 2s lipos are lower than 4s - but individual cells are balanced in each. 

3s 
1. 3.83 
2. 3.82
3. 3.83

3s
4. 3.83
5. 3.83
6. 3.82

2s
7. 3.72
8. 3.73

2s
9. 3. 72
10. 3.73

Could this be a reason BMS is acting up and not taking Voltage from power supply given specs of my BMS above?
```

---
## \#6 Posted by: Jinra Posted at: 2017-07-26T22:00:43.095Z Reads: 82

```
Where is battery negative on the balance leads in that picture?
```

---
## \#7 Posted by: MontPierre Posted at: 2017-07-26T22:18:01.721Z Reads: 77

```
UPDATE:

Not sure if I broke it off or it fell off by itself but no wonder now why its heating up.... - I guess it's time to invest in proper BMS (emailing BESTECH now). 

<img src="/uploads/db1493/original/3X/f/d/fdc966ec10e85b9fbbc3949b64a4d365b78e3e61.JPG" width="375" height="500">
```

---
## \#8 Posted by: Jinra Posted at: 2017-07-26T22:20:52.046Z Reads: 75

```
I don't think this is a quality issue, you'll want to prod the header with a multi-meter and triple check before plugging anything in. I learned the hard way as well.
```

---
## \#9 Posted by: MontPierre Posted at: 2017-07-26T22:33:02.496Z Reads: 77

```
Yeah, I could have also plugged in balance cables before connecting negative B- wire. I wish there was step by step instruction attached - now I know. I might get one more of those and give it a second chance.
```

---
## \#10 Posted by: rakejagland Posted at: 2017-07-27T14:51:12.872Z Reads: 68

```
I tried fully charging the batteries @JdogAwesome but my charger said it was fully charged and balanced at 26V instead of the 29V that it was new fully charged. It still overheats within 5 seconds of turning the power on. 

I am going to try one more thing when I get home today and I'll reply how it goes @MontPierre since it looks like we have very similar problems. I am going to completely remove the BMS from the board and run it with what it has. I'll see if I can use regen braking to get up to near full charge. If I can get back up to charge, then I know my battery cell isn't damaged. After that, I'll reinstall the BMS (THE CORRECT WAY AND CORRECT ORDER) and see if the BMS is done for or not. Prob going to have to order another one looks like...

Thanks for all the help everyone, I hope we can get these problems sorted.
```

---
## \#11 Posted by: MontPierre Posted at: 2017-07-27T15:22:14.744Z Reads: 69

```
Yeah, I think I fried mine because I have connected balance wires first and then charge and B-. Only later I discovered on some other listing instruction:


> -In order to achieve the best performance of BMS and to run the longest distance, all the battery must be matched well (Each battery voltage ≦0.05V, IR≦15 mΩ,capacity≦30mAh) to make sure the better consistency of the battery.
>  
> -Cell must be connected in parallel first, after then connected in series
>  
> -Order of connection:
>  
> Step1: Connect charging /discharging wire , battery pack negative wire
>  
> Step2：After confirm the wires are connected OK, plug the connector cable in the BMS
>  
> DO NOT plug CONNECTOR CABLE in the BMS before connect wire!!


Bummer!
```

---
## \#12 Posted by: rakejagland Posted at: 2017-07-27T19:07:50.113Z Reads: 60

```
I also have one more quick question. I'm almost certain the BMS is blown the more that I look into it, so I'm already in the market for another one. Should I invest in one that has the capability of discharging to the motors at a high enough amperage? And if so, for my 8S setup, how many amps would be needed to discharge without limiting the output capable from the other components? Here are my other components:

(2x) Batteries: https://hobbyking.com/en_us/turnigy-5000mah-4s1p-14-8v-20c-hardcase-pack.html
VESC: diy-electric-skateboard-kits-parts/vesc-the-best-electric-skateboard-esc/
Motor: diy-electric-skateboard-kits-parts/electric-skateboard-motor-6355-190kv/
```

---
## \#13 Posted by: MontPierre Posted at: 2017-07-27T19:42:32.319Z Reads: 63

```
Your Motor has max 80A so I would go with BMS for up to 80A.

Here is good one, I'm thinking of buying it. It is for 10s but they have other options. You will need 8s.

http://bestechpower.com/37v10spcmbmspcbforli-ionli-polymerbatterypack/PCM-D223V1.html


And here are the prices as of yesterday with shipping to UK - 3-5 days DHL I think 9 just to give you an idea, yours might be few dollars cheaper). You have to order at least two - they are made to order. In the email I was told :

> We need around 7-9 working days for production.  And 3-5 days for shipping.


<img src="/uploads/db1493/original/3X/2/1/21bde976797351a61e4dc91c9079bc17e3bdbc51.png" width="690" height="273">


Where are you based?
```

---
## \#14 Posted by: SilentException Posted at: 2017-07-27T19:53:12.972Z Reads: 57

```
[quote="MontPierre, post:13, topic:28691"]
We need around 7-9 working days for production.  And 3-5 days for shipping.
[/quote]

This timeline seems correct, from my experience. I payed them on July 5th, shipment was sent out July 18th. 

DHL shipping only and it is to expensive IMO. But fast, the package was in my country on July 21st but held by customs.

In EU, you will be charged with import taxes and customs charges, which with DHL (as customs service provider) will not be cheap. I'm additionally need to pay more at least 23% of the total value and some fixed charges (around 10-15€).
```

---
## \#15 Posted by: rakejagland Posted at: 2017-07-27T22:14:26.896Z Reads: 56

```
@MontPierre I removed the bad BMS and charged the batteries. None of the cells were damaged it seems because I was showing full voltage and it discharged fine. I am ordering a new BMS and migh (or might not) update this topic once it comes in. Once again, since we don't want to make the same mistake again, here is a website that provides good step-by-step instructions on wiring a BMS. Forget about the specific product, just look at the diagrams and instructions. 

http://www.batterysupports.com/24v-256v-8s-30a-8x-32v-lifepo4-battery-bms-lfp-pcm-smt-system-p-246.html
```

---
## \#16 Posted by: MontPierre Posted at: 2017-07-27T22:24:42.173Z Reads: 51

```
Exactly! Ordering new bms and following instructions;) good luck and let me know how it works!

Getting bestech?
```

---
