# Smart Charger Comparison

### Replies: 14 Views: 524

## \#1 Posted by: mikenyc Posted at: 2018-09-07T23:35:53.862Z Reads: 151

```
I'm going to be using a top mounted battery (12s8p) without a BMS on my next build for easy swapping between a couple different boards. 

I'm curious to hear if anyone has experience with either of these smart chargers, or anything similar.

https://www.amazon.com/dp/B07F6V87HS/ref=sspa_dk_detail_5?psc=1&pd_rd_i=B07F6V87HS&pf_rd_m=ATVPDKIKX0DER&pf_rd_p=a54d13fc-b8a1-4ce8-b285-d77489a09cf6&pf_rd_r=RTDC7CZXYHZF3J9DR6B5&pd_rd_wg=VHZWk&pf_rd_s=desktop-dp-sims&pf_rd_t=40701&pd_rd_w=97fRN&pf_rd_i=desktop-dp-sims&pd_rd_r=dd2da321-b2f4-11e8-b96a-75051c3f57a5

https://www.amazon.com/dp/B07DR8HW19/ref=sspa_dk_detail_1?psc=1&pd_rd_i=B07DR8HW19&pf_rd_m=ATVPDKIKX0DER&pf_rd_p=a54d13fc-b8a1-4ce8-b285-d77489a09cf6&pf_rd_r=NH1X2H0HPXXXFX3TT2ZC&pd_rd_wg=LKUWC&pf_rd_s=desktop-dp-sims&pf_rd_t=40701&pd_rd_w=JyXTB&pf_rd_i=desktop-dp-sims&pd_rd_r=428fcf43-b2f6-11e8-8742-1712fd196554
```

---
## \#2 Posted by: akhlut Posted at: 2018-09-08T00:19:47.498Z Reads: 131

```
I've been thinking about the cycle satiator for 5p, but 8p is gonna need lots of amps.

that second one looks pretty good.
```

---
## \#3 Posted by: deucesdown Posted at: 2018-09-08T01:05:26.700Z Reads: 120

```
To use a dual, usually you have to break the serial connection in your pack, as the grounds tend to be shared between the 2 sides.

For a huge pack, maybe something serious like this?

https://www.aliexpress.com/store/product/Chargery-C4012B-12S-LiPo-LiFe-LTO-AC-DC-1500W-500W-Balance-Charger-Power-LCD-Display-Lifepo4/2856009_32863521736.html
```

---
## \#4 Posted by: mikenyc Posted at: 2018-09-08T01:31:31.885Z Reads: 104

```
Yeah, it’s really going to be 2 6S packs connected in series. Though, I may borrow some elements of @michaelcpg’s pack design.
```

---
## \#5 Posted by: mikenyc Posted at: 2018-09-08T01:33:05.818Z Reads: 96

```
Yeah it’s pretty nice. Though it seems that you need to use DC to charge at high current on both channels at the same time.
```

---
## \#6 Posted by: Kug3lis Posted at: 2018-09-08T01:41:55.296Z Reads: 89

```
I was using similar setup. For DC power supply grab some 24V or 48V ~1-2kW Server Power supplies for extra cheap on ebay europe has https://www.servershop24.de/en/ 

But in the end I just grabbed simple 12S 8A charger and just bulk charging I got tired of disconnecting 12s to 6SP and other stories :)
```

---
## \#7 Posted by: mikenyc Posted at: 2018-09-08T02:09:41.461Z Reads: 84

```
I’ll probably wind up doing that most of the time. I’ll have a battery monitor to make sure they don’t drift too far apart. Good idea on the server power supply. I’ll see what I can find in the states.
```

---
## \#8 Posted by: Namasaki Posted at: 2018-09-08T04:00:19.440Z Reads: 75

```
This charger will charge up to 12s and up to 25a
It does require an external DC power supply though.
https://www.amazon.com/EVPEAK-1350W-Charger-Battery-Screen/dp/B01D4PORJW/ref=sr_1_2_sspa?ie=UTF8&qid=1536379501&sr=8-2-spons&keywords=12s+lipo+charger&psc=1
```

---
## \#9 Posted by: Cobber Posted at: 2018-09-08T04:18:50.443Z Reads: 69

```
:+1: for the server power supply
```

---
## \#10 Posted by: Hummie Posted at: 2018-09-08T06:34:21.124Z Reads: 57

```
wow never seen that before.  and it has a balance plug inlet for a 12s?  it looks like it.   very nice.
```

---
## \#11 Posted by: Goonman Posted at: 2018-09-08T06:36:16.250Z Reads: 56

```
I use two server power supplies. I followed the guide someone put up on an RC forum. Use them with  isdt sc-620. Personally I balance each pack first then parallel together stopping at 4.15v just in case one cell is out of balance. Gonna get another sc620 to speed things up. I use my packs in a variety of projects too.![15363884610932093052845|281x500](upload://mNNF8Y37C97RE4Gy8sKOflIQ5CD.jpg)
```

---
## \#12 Posted by: deucesdown Posted at: 2018-09-08T14:39:03.132Z Reads: 41

```
I have one. It comes with a breakout board for 12s. I tried to buy a 10s breakout board but they stopped responding. Will have to try making it myself if I want it badly enough.

It can do bulk charge (without balancing) at 12s, which is nice.
```

---
## \#13 Posted by: Hummie Posted at: 2018-09-08T14:42:49.711Z Reads: 41

```
It needs a power supply too?
```

---
## \#14 Posted by: deucesdown Posted at: 2018-09-08T15:22:11.317Z Reads: 38

```
Yes. I think its usually separate on high power chargers for heat.
```

---
