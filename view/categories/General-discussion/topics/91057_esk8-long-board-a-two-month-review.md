# Esk8 Long board a two-month review

### Replies: 5 Views: 952

## \#1 Posted by: junhyun Posted at: 2019-04-19T00:30:31.636Z Reads: 149

```
Hi~ Guys.

I'm going to write a two-month usage review.

[KakaoTalk_20190418_191410808_04|375x500](upload://8AoaZhA2PnEsl63DbAtZGw4LvW8.jpeg) ![KakaoTalk_20190418_191410808_05|375x500](upload://zpZUK0Eomm22WkXED6YYzWO9kcY.jpeg) ![KakaoTalk_20190418_191410808_06|666x500](upload://jiz2JVrEJkYaxT7wW3JAZPgGP2m.jpeg) ![KakaoTalk_20190418_191410808_10|666x500](upload://gkMdZdaQU8y7eutArdbEkIFHAas.jpeg) ![KakaoTalk_20190418_191410808_11|375x500](upload://nN7soe1f2WqkVDlvZgXc0izE7Cz.jpeg) ![KakaoTalk_20190418_191410808_12|666x500](upload://stf8RO1ThhujgT22vWCGVoXkeU6.jpeg) ![KakaoTalk_20190418_191410808_13|375x500](upload://A3oNgwOLqh0Zw5bI7y8ZYlrDwTw.jpeg) ![KakaoTalk_20190418_191410808_14|666x500](upload://awzG7fsthslY3lLfCaRVpgLZuRs.jpeg) ![KakaoTalk_20190418_191410808_15|666x500](upload://z0h9thOcXiVEW8qqXhjTdmBe3zh.jpeg) ![KakaoTalk_20190418_191410808_16|375x500](upload://5DbV2GzZMC3GoZle3UsW9TZ2CXq.jpeg) 




First of all, the specs are like this.

Motor : ailian 6384 170kv
ESC : Ezrun Max6
Truck : Evolve GT Truck
Wheel : ABEC11 107mm Wheel
Battery : 8S 12P 
Deck : Trampa Orrsom Deck
Motor Gear : 34T
Wheel Gear : 48T
The top speed : 65km/h

The first homework to solve was the wheelbase. The distance between the shaft and the shaft of the motorshaft must be rinsed, and both gears must be engaged to find the appropriate distance size. The gear has a different diameter depending on the module and the torsional angle of the gear count helical gear.
The appropriate wheelbase I found was 55mm to 65mm.




![%EC%BA%A1%EC%B2%98|690x304](upload://kbGJJUyVPkbtP48uLUQ8osUy9mJ.png) ![%EC%BA%A1%EC%B2%981|690x496](upload://80r39iUnXS8KKBIyVJB9G77ByAG.png) 




When the ABEC 107mm wheel was fitted and the 6384 motor was used, and the powertrain ride height was 10.19mm. But while there are certain ways to increase the gear ratio and to secure more ground clearance, I'm not a design front, and the gear ratio, wheelbase and ride height have been limited. 



Now to conclude,
1. Cloudyness is good because it is a belt-free gear.
2. The throttle is pulled and the brake is immediately reactive. This is likely.
3. There's a 'dead' sound coming in from the gear rotating, but it's quieter than the belt.



That's a good word, and as a long-board direct-gear drive drawback,

1. The biggest problem is gear ratio.
2. The cover is essential, so the ride height must be low.
3. Because it's a longboard that's weak for vibration, you can't help but wear a demage on the gears for a long time.
4. It's difficult to maintain.
5. There was no problem in winter, but the heating problem of the gearbox itself is thought to be serious in summer.
6. Powertrain itself weighs a lot.
7. Expensive burden.


![112|666x500](upload://udqOXu4e6XNIpU09gS4aMw5seBq.jpeg)
```

---
## \#2 Posted by: junhyun Posted at: 2019-04-19T00:39:00.614Z Reads: 135

```
I turned the translator around because I don't know how to speak English. I'm sorry that the sentence isn't smooth. :sweat_smile:
```

---
## \#3 Posted by: Grozniy Posted at: 2019-04-19T08:44:13.199Z Reads: 93

```
Great review
```

---
## \#4 Posted by: Netoa Posted at: 2019-04-20T09:28:26.643Z Reads: 62

```
@junhyun did you make the direct drive yourself?
```

---
## \#5 Posted by: MasterSpoon Posted at: 2019-04-20T10:16:08.676Z Reads: 53

```
That is an interesting setup, geared for a current top speed of 65km/hr seems a little high.

If your interested in dropping the top speed and hopefully getting a little more low end power back could try re-terminating the motor to WYE winding (170kv Delta should be 100kv in WYE / star) and changing the battery from 8s12p to 12s8p 

http://calc.esk8.it/#{%22batt-type-lipo%22:1,%22batt-cells%22:8,%22motor-kv%22:170,%22system-efficiency%22:85,%22motor-pulley-teeth%22:34,%22wheel-pulley-teeth%22:48,%22wheel-size%22:107}|

Vs 

http://calc.esk8.it/#{%22batt-type-lipo%22:1,%22batt-cells%22:12,%22motor-kv%22:100,%22system-efficiency%22:85,%22motor-pulley-teeth%22:34,%22wheel-pulley-teeth%22:48,%22wheel-size%22:107}|

Not going to be a huge change but 37.97 mph - 61.11 km/h (weighted) vs 33.5 mph - 53.92 km/h (weighted) might be enough
```

---
