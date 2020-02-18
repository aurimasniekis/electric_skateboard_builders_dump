# Hub Motor stutters and no torque

### Replies: 25 Views: 812

## \#1 Posted by: JulianS Posted at: 2018-09-12T12:28:32.029Z Reads: 109

```
Hi guys, I ordered this hub motor from china: https://de.aliexpress.com/store/product/Maytech-Free-Shipping-1pcs-truck-for-single-motor-and-1pcs-70mm-hub-motor-for-electric-longboard/1630416_32820824995.html?spm=a2g0x.12010612.8148356.60.331d43056Wvysp

I attached to the vesc and set the parameters, but the motor has almost no torque at startup. I can hold it with 2 fingers in place. When I push the board a little it's enough to keep board rolling but thats it, topspeed is like 10km/h

I resoldered the bullet connectors and tested the connection between the phases (shorted, as it should be)

My best guess is a faulty motor or something off with my settings. I took of the sensor to elimate a fault source and did the motor detection. Changing the Current to 1A lets the motor spin. But the result seems off to me, esp the BEMF Coupling is very high. The tool actually caps it at 900. 
![image|552x143](upload://v0qJNjmabEQf8jV9pmCPtUUvILb.png)

The Vesc works fine, I tested it with a different motor. 
I also tried FOC with sensors mode. That stops the sputtering and gives it more torque. But the top speed is less then impressive.
![image|690x47](upload://zRqYWMBB9UNZORrFBuDGHZj8T8b.png)

Can it be that the hub motor has so little torque? Can I fix something about my settings?

Regards
Julian
```

---
## \#2 Posted by: mynamesmatt Posted at: 2018-09-12T12:35:26.954Z Reads: 96

```
what are your motor min/max and battery min/max values?
```

---
## \#3 Posted by: Sn4pz Posted at: 2018-09-12T12:42:02.938Z Reads: 90

```
your motor maX and min probably arent configured right :thinking:
```

---
## \#4 Posted by: JulianS Posted at: 2018-09-12T12:57:07.168Z Reads: 88

```
![image|417x324](upload://4sj34Rba8cFHYc9wTrhOtVXqpNy.png)

I set it to 30 Amps, bc the motor is only rated for 22
```

---
## \#5 Posted by: Sn4pz Posted at: 2018-09-12T12:59:27.079Z Reads: 74

```
make sure you do bldc motor detection

but also maybe lower the batt amps? that little motor might not know what to do with 60a :laughing:
```

---
## \#6 Posted by: JulianS Posted at: 2018-09-12T13:04:02.933Z Reads: 74

```
Yeah, I did the BLDC, see my first screenshot :slight_smile:

Why would the motor get more then 30Amps when I set the current? When testing with the tool the current never exceedes 3A anyway.
```

---
## \#7 Posted by: rey8801 Posted at: 2018-09-12T13:07:35.598Z Reads: 74

```
It's different load and unload. When you are riding the board the current will rise. After you did the motor detection did you apply the values? You have to write them in your vesc otherwise you only did the detection. Plus I see you battery values wrong. Which battery do you use? I guess small for that small motor. - 40 will kill your battery, same for the discharge. Although your motor will never take that much. Please see this video and repeat all the steps https://youtu.be/v1glLDO-EjA

Just out of my curiosity why did you choose this motor over the other well tested? It's also quite expensive to be a single drive.
Good luck
```

---
## \#8 Posted by: JulianS Posted at: 2018-09-12T13:16:01.321Z Reads: 71

```
Thanks, I check out the video!

That it doesn't take a lot of current without load makes sense, but when I block the wheel the current should rise. (More Torque, more Current)

The battery is a 40C 4500mAh, which should deliver up to 200A (constant), the charge rate is not specified, but I assumed it to be around 10C.

Yeah, applied the values. But as mentioned its weird that the detection suggests 1893 for the coupling but when I click apply its only 900. There is probably a good reason for that. My outrunner motor works fine with the vesc.

TBH, I didnt do a lot of research, the requirement was that it needed to be delivered to germany and within budget. There probably is a section for tested motors around here I assume? :slight_smile:
```

---
## \#9 Posted by: Benjamin899 Posted at: 2018-09-12T13:23:41.662Z Reads: 65

```
you need to increas the duty and leave the other values as is, as far as i know
```

---
## \#10 Posted by: rey8801 Posted at: 2018-09-12T13:26:10.581Z Reads: 65

```
Ah ok you use LiPo battery, that's why the values. Way too much power for that motor anyway.
No there is no a section for that and I am totally pro to testing out new thing. I said that because I run hub motor for the past 2 years and they need to be bigger to work better. For the same price you could get way more powerfull motor. Actually even a dual set up.
Anyway if you did the all step shown in the video then I do not know. maybe that is the power of the motor. I hope not because it won't bring you far. The first slightly incline and you are stocked.
```

---
## \#11 Posted by: JulianS Posted at: 2018-09-12T13:34:44.735Z Reads: 61

```
Thanks for your help anyway! :) I'm just testing things out. The outrunner I had before was way to powerful and heavy so I tried something more subtle. Do you have a recommendation for something light thats strong enough to get me to 20km/h?

I'm gonna resolder the connections and open the motor up. I also contacted the vendor about their controller values.
```

---
## \#12 Posted by: rey8801 Posted at: 2018-09-12T13:50:27.995Z Reads: 59

```
Most of the hub motors out there come as dual set up. You can pair them with a cheap ESC if you want them as kit or used 2 vesc or a dual unit like the one Flipsky is selling ofr 100 Euro 4.20 hardware. If only need another vecs then take the flipsky 4.12 for 50-60 Euro is a best buy.
Hub motor I advice. Diyeboard, meepo, ownboard, wowgo all the same, 90mm wheels. They ar e250Watt except the one from diyeboard 500W. They look the same, but these are the specs. They are 75kv. I have the diyeboard one with a 10s3p battery, 38kmh and great torque.
Then if you want something more and still stay in the price, I tested and now organising a group buy for these hub motors. Same as torque board was selling, but I could get it for less then half. https://www.electric-skateboard.builders/t/review-and-eu-usa-group-buy-90mm-mad-hub-motors-75kv-or-130kv-dual-170-euro-1st-round-closed/62002/121?u=rey8801
I advice to use them dual but also singel is possible. 75Kv or 130Kv version. These are really strong. The strongest I tried.
Other ones are the maytech one, good motor, but expensive, get too hot and the PU is shit.

So to me in that price range the Diyeboard hubs, or better the MAD hubs.
```

---
## \#13 Posted by: JulianS Posted at: 2018-09-12T14:14:46.781Z Reads: 53

```
Yes, I have the maytech one. I heard they are solid, thats why I'm so dissapointed with the performance. I just tested it out again with FOC. It works okay but the torque is really small and topspeed is like 15km/h on a 6s.

Thanks for your advice!
```

---
## \#14 Posted by: rey8801 Posted at: 2018-09-12T14:19:56.851Z Reads: 50

```
I was talking about the 90mm maytech one not the one you have
```

---
## \#15 Posted by: visnu777 Posted at: 2018-09-12T17:18:15.039Z Reads: 43

```
In case you don't know it:

http://calc.esk8.it/#{"batt-type-lipo":1,"batt-cells":6,"motor-kv":60,"system-efficiency":85,"motor-pulley-teeth":1,"wheel-pulley-teeth":1,"wheel-size":70}|

You won't Get any more speed out of it.
```

---
## \#16 Posted by: JulianS Posted at: 2018-09-12T18:01:50.288Z Reads: 38

```
Yeah, thanks, did my own math but maybe it went wrong somewhere :) I assumed 25V for 6s (fully charged)
```

---
## \#17 Posted by: Pedrodemio Posted at: 2018-09-12T18:06:19.872Z Reads: 36

```
Wait, are you testing using the arrows on the keyboard or the remote? If is the keyboard the default max current is 3A, you can change it in one of the bottom tabs on VESC tool
```

---
## \#18 Posted by: JulianS Posted at: 2018-09-13T08:13:45.874Z Reads: 32

```
Ah, thanks, thats a good hint :) Seems FOC seems to work okay, the top speed just isnt great, even on a full battery.
```

---
## \#19 Posted by: rey8801 Posted at: 2018-09-13T08:21:32.353Z Reads: 32

```
That's due to the motor, as I said to small and single. On the other hand is for sure lighter. Next time go for a bigger hub motor if you want torque and speed :grin:
```

---
## \#20 Posted by: JulianS Posted at: 2018-09-13T09:37:49.775Z Reads: 27

```
Yeah I expected lower speed and torque, but not that little :slight_smile: gonna play with the configs some more. If I can get it to work in BLDC, i get some extra speed out of it. Also considering to bump up the voltage. It’s officially rated for 8s, has anybody ever experimented with going up to 12s?
```

---
## \#21 Posted by: rey8801 Posted at: 2018-09-13T09:41:22.946Z Reads: 25

```
I think you won;t find a lot that bought them. I remember a dual hub motors build with similar size from like 2016  but also in that case was 8s. Probably worth it to try 10s but to me if you have to spend more money on it just get better motors and solve your problem.
```

---
## \#22 Posted by: visnu777 Posted at: 2018-09-13T09:41:25.409Z Reads: 26

```
My first buy was a similar hub (Maytech-Style, not genuine) dual setup, with 10s I made it to 28 km/h.
```

---
## \#23 Posted by: JulianS Posted at: 2018-09-13T09:46:03.537Z Reads: 24

```
I'm trying to build a minimum weight config, since I'm manly using it in an urban environment. Thats why I went for the 70mm. I think if I can get it to 25km/h I'd be pretty happy with it. Do you know if there are any better 70mm motors? How much is the weight difference actually?

Already have the batteries lying around, they are 6s though so I can go for 12s or nothing :stuck_out_tongue:

Thanks for all your helpful answers!
```

---
## \#24 Posted by: rey8801 Posted at: 2018-09-13T09:49:46.753Z Reads: 24

```
maytech hubs have a good motor so  Ibelieve you have a good 70mm hub motor, just with it's limit. At 12s if it doesn't brake you should be able to reach 25kmh on flat good road. It also depends which vesc ar eyou using not all of them support 12s
```

---
## \#25 Posted by: rey8801 Posted at: 2018-09-13T10:05:28.780Z Reads: 25

```
If you want more torque for 70mm hubs. This one is a dual set up, cheap and will do the job. You can also pair them with a cheap ESC (if you use Liion cells) to stay low in cost and light. I always advice VESC though.
```

---
