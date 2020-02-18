# 1st build, need advice

### Replies: 12 Views: 329

## \#1 Posted by: Duy Posted at: 2019-04-07T17:09:16.014Z Reads: 101

```
Hi, im a uni product design student working on a project for my final, i need help comfirming my parts list will work together before i start buying. Here are the parts list:

MOTORS:
[https://www.banggood.com/24V-42V-550W-70KV-Electric-Longboard-Skateboard-Brushless-90mm-Dual-6364-Hub-Motors-Drive-Kit-p-1186579.html?rmmds=search&cur_warehouse=USA](https://www.banggood.com/24V-42V-550W-70KV-Electric-Longboard-Skateboard-Brushless-90mm-Dual-6364-Hub-Motors-Drive-Kit-p-1186579.html?rmmds=search&cur_warehouse=USA) 

BATTERIES:
[https://hobbyking.com/en_us/zippy-flightmax-3000mah-5s1p-20c.html](https://hobbyking.com/en_us/zippy-flightmax-3000mah-5s1p-20c.html)
i will be buying of these so it becomes a 10s1p battery consisting of 37v and 20a discharge?

BMS:
[https://www.ebay.co.uk/itm/10S-Li-ion-Lithium-Cell-36V-40A-18650-Battery-Protection-BMS-PCB-Board-Balance/232864260321?epid=23024661399&hash=item3637caa0e1:g:NBcAAOSwGZxbWie1&frcectupt=true](https://www.ebay.co.uk/itm/10S-Li-ion-Lithium-Cell-36V-40A-18650-Battery-Protection-BMS-PCB-Board-Balance/232864260321?epid=23024661399&hash=item3637caa0e1:g:NBcAAOSwGZxbWie1&frcectupt=true)
I will add in a BMS instead of a balance charger for ease of use, the bms is rated 40a but my battery setup is 20a, this can still work right as my max amp draw is lower than bms itself?
Also must i charge the batteries with a balance charger first then install the bms? 

ESC: 
[https://www.banggood.com/Electric-Skateboard-Longboard-Controller-With-Remote-Dual-Motors-ESC-Substitute-p-1202299.html?rmmds=search&cur_warehouse=CN](https://www.banggood.com/Electric-Skateboard-Longboard-Controller-With-Remote-Dual-Motors-ESC-Substitute-p-1202299.html?rmmds=search&cur_warehouse=CN)

LAPTOP CHARGER STYLE:
[https://www.amazon.co.uk/TangsFire-battery-electric-DC5-5mm2-1mm-connector/dp/B07FT4RY9L/ref=sr_1_1_sspa?keywords=42v+charger&qid=1554653333&s=gateway&sr=8-1-spons&psc=1](https://www.amazon.co.uk/TangsFire-battery-electric-DC5-5mm2-1mm-connector/dp/B07FT4RY9L/ref=sr_1_1_sspa?keywords=42v+charger&qid=1554653333&s=gateway&sr=8-1-spons&psc=1)

CHARGING PORT: https://www.amazon.co.uk/HSeaMall-Socket-Connector-Adapter-Dustproof/dp/B07D4F15Y4/ref=sr_1_fkmrnull_1?keywords=HSEAMALL+20PCS+5.5+X+2.1+MM+DC+POWER+JACK&qid=1554656009&s=gateway&sr=8-1-fkmrnull
```

---
## \#2 Posted by: ZachTetra Posted at: 2019-04-07T17:16:32.782Z Reads: 84

```
[quote="Duy, post:1, topic:89711"]
20a discharge
[/quote]

Safe discharge rate if a lipo is defined as the C rating times the ampacity in Ah

3Ah * 20C continuous is 60A continuous
3Ah * 30C burst is 90A burst

-----------

The motors are rated for about 15A each but may draw slightly more if you are maxing the throttle up hill, the BMS could suddenly cut power so be careful

In all likelihood it will not pull more than 10A and you should be fine, my hubs are comperable and pull 19A max speed uphills


---------

The ESC is complete crap, it is only designed for 6s or 7s and a max amp rating of 12A which is way to small

Try this if you want cheap and simple, it's not spectacular quality but I run a dual hub budget board with it and it's very nice to use
https://www.ebay.com/itm/Dual-motors-longboard-skateboard-control-modula-ESC-Substitute-with-remote/323326552273?hash=item4b47c3a8d1:m:mxSlsLM_-dEIr0XuDFII9Lg
```

---
## \#3 Posted by: Andy87 Posted at: 2019-04-07T17:24:21.749Z Reads: 65

```
[quote="ZachTetra, post:2, topic:89711"]
3Ah * 20C continuous is 60A continuous 3Ah * 30C burst is 90A burst
[/quote]

And than take half of this value and you have nearly the real life discharge values.
```

---
## \#4 Posted by: Duy Posted at: 2019-04-07T17:33:04.498Z Reads: 60

```
Oh I see now, thanks for the information zach. Do you have a link where I can buy the ESC from UK as I’m from there?
```

---
## \#5 Posted by: Duy Posted at: 2019-04-07T17:34:14.161Z Reads: 57

```
Thanks Andy, really nice info. You guys are awesome!
```

---
## \#6 Posted by: ZachTetra Posted at: 2019-04-07T17:45:04.580Z Reads: 54

```
I don't know what link to give you because that sweet USA privilege but make sure the ESC is rated for 10s specifically and at least 30A or about 600W per motor

Always overspec the ESC and battery if you can
```

---
## \#7 Posted by: Duy Posted at: 2019-04-07T18:06:03.146Z Reads: 52

```
I just remembered that the esc I linked may actually support 10s. So, a while back, I read that in the reviews sections, customers reported that desoldering the connection between 6s and 7s points allows the esc to support 10s. ![26|690x431](upload://hcaatXJsRzA1Hnb9ueRieSJhfok.png) 
![38|690x431](upload://w4be7E8apKX9zYQNUumFaR5rkpH.png)
```

---
## \#8 Posted by: Duy Posted at: 2019-04-08T12:10:24.639Z Reads: 36

```
Got a question. If i change my batterys from 2x lipo 5s 3000mah 20c, to 2x lipo 5s 5000mah 20c it will still work with the BMS (10s, 40a) t right? 

Trying to achieve a little bit more range for the build
```

---
## \#9 Posted by: Superflim Posted at: 2019-04-08T12:15:16.689Z Reads: 35

```
Yes will work
```

---
## \#10 Posted by: Duy Posted at: 2019-04-29T14:16:54.255Z Reads: 22

```
For some reason my hub motors are not working. Shouldnt there be sound coming from the hub motors? There is no sign of power coming from them. Though when esc is off and i spin one of the hub motor wheels it automatically powers on the esc. can anyone help me please? image below shows wiring
![IMG_0926|666x500](upload://fCM3GkCwIrZLbmPvPuhfTE4Cmnf.jpeg)
```

---
## \#11 Posted by: Duy Posted at: 2019-04-30T00:20:54.114Z Reads: 14

```
NEVER MIND!
Got it work by disconnecting the power and reconnecting it to ESC again. There were sparks when connecting battery to ESC the first time, and also the second too when reconnecting, but it worked arfterwards somehow. :slight_smile:
```

---
## \#12 Posted by: ZachTetra Posted at: 2019-04-30T00:23:04.535Z Reads: 14

```
[quote="Duy, post:11, topic:89711"]
There were sparks
[/quote]

You need a loop key in-between the ESC and BMS, or replace the battery plug with an XT90s

Use the sensors if you can, way way better start, if a wheel just vibrates when you try to drive it, keep swapping phase wires
```

---
