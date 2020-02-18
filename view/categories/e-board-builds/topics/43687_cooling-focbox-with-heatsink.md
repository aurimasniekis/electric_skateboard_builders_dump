# Cooling FOCBOX with heatsink!

### Replies: 29 Views: 2573

## \#1 Posted by: Jerome Posted at: 2018-01-14T12:07:41.616Z Reads: 444

```
Conscious of the importance of cooling down power electronics , I decided to measure the FOCBOX mosfet temperature using the bluetooth module and the iphone app.  This post will be a comparison like for like. 
2 rides 1 day apart,  same set up same rider  , me :slight_smile: ,   The heatsink was mounted using a thermal compound with 4-5W/mk of thermal conductivity to improve the contact.  The heatsink is slightly greater than the FOCBOX baseplate. 
RESULT !!!  :   max temp reached  80degC without and 63degC  with the heatsink , so it definitely works!!

I think I will safely raise the max current limit knowing the cooling is improved

Given how wide the FOCBOX is ,  this method is better than adding a fan from a thermal conduction standpoint.  A fan would be useful only if a heatsink is present as the heat exchange surface is much increased.


![pics|690x292](upload://heEjdC255N7TlKcNV8dVIXtLYLJ.jpg)

![stats|690x238](upload://psfE5dk6R1cRnhYMYX27va5gZPA.PNG)

![without heatsink|690x239](upload://4FpsBy2WKbiyw7noy6oD5KvgkZn.png)

![with heatsink|690x231](upload://wTfa0QDXeXpCp0mLnA9r82pejt6.png)


tell me what you think  ;)
```

---
## \#2 Posted by: b264 Posted at: 2018-01-14T12:32:08.757Z Reads: 407

```
This is very interesting; thank you for sharing
```

---
## \#3 Posted by: Ronny_CTS Posted at: 2018-01-14T12:52:05.622Z Reads: 393

```
This solution has crossed my mind several times. Is the heatsink exposed to the wind while riding or is it hiden in your encolsure?
```

---
## \#4 Posted by: b264 Posted at: 2018-01-14T12:55:14.200Z Reads: 389

```
It looks like there's just a few holes drilled, but I don't know if any holes are drilled on the other side, allowing for flow ...
```

---
## \#5 Posted by: Riako Posted at: 2018-01-14T12:59:53.063Z Reads: 379

```
Thanks for this sharing mate !! I was asking myself if I really had to do this :blush:
I think, you convinced me ;)
what weither and ambient temperature is it in yr country ?
```

---
## \#6 Posted by: Jerome Posted at: 2018-01-14T13:05:05.523Z Reads: 367

```
Yes part of the heatink is exposed to air, it is extending out of the enclosure.  But to make it waterproof I taped it over, still we get heat transfer
```

---
## \#7 Posted by: Jerome Posted at: 2018-01-14T13:06:34.236Z Reads: 355

```
Hi Riako
I rode this in Stafford 🇬🇧, it was 0 degC these days outside. So what we measure is only temperature rise:) !!!
```

---
## \#8 Posted by: Jerome Posted at: 2018-01-14T13:07:46.238Z Reads: 346

```
Look at the pic with the compound, part of the heatsink is out
```

---
## \#9 Posted by: Riako Posted at: 2018-01-14T13:20:14.743Z Reads: 347

```
wow :open_mouth: that is really interesting so !!
I used to ride under vesc6 FOC  dual 6374 130kv 12s(12Ah)
But it dont exceeds 45°C ("hard ride") / 34°C (under snow time) in a closed box.
But for my esk8 I will use Fox so your report is very interesting, especially since I was thinking about to put everythingin a closed and watterproof box too ... :sweat_smile:
```

---
## \#10 Posted by: Jerome Posted at: 2018-01-14T19:36:33.154Z Reads: 319

```
Having a dual setup would divide your current need by 2 therefore each speed controller would heat up much less. You have 130kv motors so they will draw even less current than mine being 149kv.

Where/how did you measure the temperature ?

I m on single motor set up. 6374 149kv 12S 5Ah
```

---
## \#11 Posted by: Surfer Posted at: 2018-01-14T20:25:40.045Z Reads: 301

```
Really guys I don't understand how cool my vescs ( Maytech ) are going under hard riding without any cooling,  with 2 6355 16/36 I never go up than 40~45 degrees. Riding a raptor 2 also around 50~55 degrees Max, and I'm a heavy rider, 110kg fully pack.🤔
```

---
## \#12 Posted by: E1Allen Posted at: 2018-01-14T22:52:35.633Z Reads: 281

```
You have to pull hard up a decent hill to get temps to come up.  I have dual FOCBOX mounted on an aluminum plate.


https://metr.at/r/T6UPp
```

---
## \#13 Posted by: Riako Posted at: 2018-01-14T23:30:36.754Z Reads: 275

```
Ok, that perfectly make sence to me :blush: Love this topic ! Thx for the infos Im missing !!
It will be a dual esk8 but only use the beautifull days (potentially hot).
I got it with Ackmaniac and metr.app (around Paris, I got some VDLA on [my build](http://www.electric-skateboard.builders/t/darth-vapor-street-fighter-offroad-130kv-vesc6-foc-12s12ah-custom-x-mount-carbon-deck/31680/61) ) spec are 70amps motor max, 65 amps batt max on itch v6.
But E1Allen seams to be dual too ... maybe the not the same ambiante temperature, but almost same as your single. Surfer ... wow your V4.xx stay super cool ! Air forced ? I gonna take a look at your build ;)  


Also, I'm running hard my e-dirt scooter under fox seens friday (vs. VESC 4.10 before ), its actually open air, I will put my BT module on it to see the temp (its less than 5/10°C outdoor). And then made the upgrade to see the profit ! 

I think its a good point and always could help our build (especially this summer).
```

---
## \#14 Posted by: E1Allen Posted at: 2018-01-14T23:56:46.450Z Reads: 250

```
That was going up a steep hill on 18/36 with 107mm wheels. Was still accelerating when I backed off at 37mph but the temps were climbing quick.

Maybe 25c ambient temperature
```

---
## \#15 Posted by: DeathCookies Posted at: 2018-01-15T12:42:38.471Z Reads: 241

```
[quote="Jerome, post:1, topic:43687"]
tell me what you think  :wink:
[/quote]

Hard to tell anything about it... These are two completely different runs!
But at least we can say that the focbox runs cooler
```

---
## \#16 Posted by: laurnts Posted at: 2018-01-15T12:45:11.641Z Reads: 236

```
Nice Research!
```

---
## \#17 Posted by: Jerome Posted at: 2018-01-15T12:51:37.134Z Reads: 241

```
[quote="DeathCookies, post:15, topic:43687"]
we can say that the focbox runs
[/quote]

Hi Death cookies ,  these are the same runs...... ,   same rider / average power  / speed   ride time with a few diff

the point was to demonstrate if we can extract heat using this method and the answer is yes.  Therefore it makes for a safer design
```

---
## \#18 Posted by: Surfer Posted at: 2018-01-15T12:52:08.951Z Reads: 231

```
If I'm not wrong when you go 10s the vesc is running cooler and the motors hotter, with 12s vesc is going hotter and motors cooler, it will be nice if someone can confirm that 😏
```

---
## \#19 Posted by: Jerome Posted at: 2018-01-15T12:54:32.878Z Reads: 230

```
[quote="Surfer, post:18, topic:43687"]
h 12s ves
[/quote]

voltage will only affect your top speed, and battery current  that is it.   motor current is always the same regardless

but in this regard 12s will draw less battery current so the VESC will be a little cooler
```

---
## \#20 Posted by: DeathCookies Posted at: 2018-01-15T14:39:40.110Z Reads: 225

```
[quote="Jerome, post:17, topic:43687"]
these are the same runs
[/quote]
You mean one VESC has a heatsink and one has not while you captured both datas?

Well, i think you have here two different runs with the same Setup but still not the same run.
I can clearly see that both runs differs in Terms of Speed. Round about 6:40 you have one time a complete stop and one time not. So the difference will add up over the entire run thus making it not well analyseable.
```

---
## \#21 Posted by: Jerome Posted at: 2018-01-19T08:52:27.373Z Reads: 209

```
That s because I have to stop and adapt the speed depending on traffid of course :slight_smile:, what matters is the avg speed and current , load.... and they are super similar , one day apart same road on my way to work.
I will improve the design by placing the fins out in the air flow in a different way.
```

---
## \#22 Posted by: meesie Posted at: 2018-01-20T13:14:28.843Z Reads: 200

```
I think @DeathCookies  means different runs as in 1 on monday and 1 on tuesday (for example.)

With “same run” @Jerome  means the same route, same rider, more or less same speed. It IS indeed on a different day, but that’s for comparison

Argument settled?
```

---
## \#23 Posted by: Jerome Posted at: 2018-02-02T17:47:51.537Z Reads: 172

```
Well said it is a comparison on overall ride output
```

---
## \#24 Posted by: Psmrman90 Posted at: 2019-01-27T21:03:42.262Z Reads: 82

```
I hate to rehash this, but I can't seem to find what a safe operating range temp for the focbox single
```

---
## \#25 Posted by: Sn4pz Posted at: 2019-01-27T21:33:44.998Z Reads: 75

```
90 c cutoff 100c max operating
```

---
## \#26 Posted by: Psmrman90 Posted at: 2019-01-27T21:44:37.482Z Reads: 69

```
90 c as in 90° Celsius? Wanting to be clear because I know batteries discharge with some weird C.  My focbox got up to 60° Celsius today, wanting to make sure that's not risky at all
```

---
## \#27 Posted by: Andy87 Posted at: 2019-01-27T21:47:36.078Z Reads: 68

```
You have an over temp protection.
If your focbox get too hot it starts powering down.
Feels like a battery cut off.
Usually it starts at 80 degree Celsius
```

---
## \#28 Posted by: Psmrman90 Posted at: 2019-01-27T21:48:25.888Z Reads: 70

```
Thanks a lot, good to know
```

---
## \#29 Posted by: Arek Posted at: 2019-01-27T21:48:37.175Z Reads: 69

```
Once I get my unity, and if it will be overheating, I'll cool it down with some heatpipe based cooling, like the one used in laptops:
https://www.ebay.co.uk/itm/Dell-Latitude-E5520-Laptop-CPU-Heatsink-Dell-00NGRW-0NGRW/153259823108?epid=1078475112&hash=item23aeff5004:g:vwoAAOSwQ5pb62Sl:rk:7:pf:0
If used it's dirt cheap.

And these are very efficient yet low profile so you can fit it almost everywhere.


Or heatsinks from low profile 1U servers:
https://www.ebay.co.uk/itm/HP-Proliant-Blade-BL460C-410304-001-Heatsink-Cooler-409495-001/361651588969?hash=item54341d4f69:g:43QAAOSwaB5Xjitv:rk:58:pf:0
Also good source of cheap and quality heatsinks.
```

---
