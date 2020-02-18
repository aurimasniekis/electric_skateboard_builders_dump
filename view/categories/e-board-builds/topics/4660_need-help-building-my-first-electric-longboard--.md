# Need help building my first electric longboard &gt;_&lt;

### Replies: 6 Views: 1668

## \#1 Posted by: ouch_fiyah Posted at: 2016-06-14T02:30:25.254Z Reads: 149

```
Hey guys,

I've been trying to read diy's and lots of posts around the forum (which is pretty awesome, I can't wait to familiarize myself more). But man, there's a lot of information out there and it's kind of overwhelming me. For example, looking at someone's build list, I literally have no clue how/why they picked those parts. Then looking at parts individually, I have no clue if they will work together (I'm pretty new at longboarding AND electric kits).

I currently have a 40" drop through board with Churchill "raven" trucks and some basic 80mm wheels. I know I'll have to buy wheels that will be compatible with a wheel pulley. I generally just cruise around for fun and I don't live in an area with a lot of hills. Probably won't be commuting super long distances.

1) I've read you want a motor with a kv between 200-300(?), with 245kv being a common choice. Currently looking at Turnigy sk3 6364 unless someone can give me different options. I'm a bit unfamiliar with specs and brands.

2) For the motor mount, i've seen the words caliber and paris thrown around. And when I looked it up, they were actual trucks. What is the difference between those and the ones I currently have (Churchill Raven's), just the shape for the motor mount to slide on right? I don't have the ability to fashion my own motor mount so I'm assume I'll have to upgrade my trucks. Any good alternatives to caliber's?

3) I can see how the mechanical (non-electric) parts work, however it's a little confusing how people would choose 1 gearing ratio vs another. Could someone explain? Nonetheless, I was looking at diyelectricskateboard's single bolt on motor mount w/drive wheel kit 16/36t, unless someone can offer opinions/alternatives.

4) Can someone explain how to choose a battery, I read the sticky on "What is Battery "C" rating" and understand the battery's capacity and peak output. I also saw that they recommended a 60a peak battery. But how would I go about picking what type/brand/size battery? and how would you estimate a battery's range? (if I went with a sk3 6364 motor, 83(?)mm wheels, standard gearing, flat terrain, and I weigh roughly 170lbs/77kg). Carrying onto the next point, I saw ESC's are offered in 6s/12s variants, which I'm guessing has to do with the battery.

(Is it simple to carry extra batteries to switch out? or do you go with whatever capacity you can and just charge it at once?)

5) ESC - I've heard a lot of good things about VESC but I also heard there was a steeper learning curve for it. I've done some programming classes in college, do you guys think I would be ok with the VESC? Also, what other popular/easy/(or maybe)cheaper ESC's are there out there? 

6) Lastly, I don't have a 3d printer, but I did see the g2tb mini controller mod and I like it a lot. Are there any similar out-of-the-box small controllers? or would they be around enertion's thumb stick controller's price range (kinda expensive).

Not sure what my price range is. I could add the recommendations/everything up and try to compromise somewhere. I did see sl33py's priority part's post somewhere, which was pretty helpful. 

Thanks in advance!
```

---
## \#2 Posted by: Michaelinvegas Posted at: 2016-06-14T02:40:32.520Z Reads: 142

```
Ok gonna just throw this here for now fo you can reference them

http://www.electric-skateboard.builders/t/new-builder-list-of-known-and-commonly-used-parts/2983?u=michaelinvegas


And this to calculate: input your variables to calculate top speed

http://toddy616.blogspot.ca/2013/07/electric-skateboard-calculator.html?m=1
```

---
## \#3 Posted by: Jinra Posted at: 2016-06-14T02:50:36.906Z Reads: 134

```
> 1) I've read you want a motor with a kv between 200-300(?), with 245kv being a common choice. Currently looking at Turnigy sk3 6364 unless someone can give me different options. I'm a bit unfamiliar with specs and brands.

You could go for the SK3 motors and 245 isn't a bad choice depending on your battery configuration, but you may want to go lower if you plan on using the VESC and a 10s+ battery. You may hit the eRPM limit and cause your VESC to error out. You can check out this thread for more details www.electric-skateboard.builders/t/choosing-the-right-motor-kv-for-the-vesc/3125/55

> 2) For the motor mount, i've seen the words caliber and paris thrown around. And when I looked it up, they were actual trucks. What is the difference between those and the ones I currently have (Churchill Raven's), just the shape for the motor mount to slide on right? I don't have the ability to fashion my own motor mount so I'm assume I'll have to upgrade my trucks. Any good alternatives to caliber's?

Calibers are pretty standard for motor mounts because of the truck shape. Paris is good too since it's round, but may require welding. If you can get a mount to fit on your trucks, more power to you. Is there a specific reason you're trying to avoid calibers? Another option are surfrodz trucks which are compatible with some mounts as well.

> 3) I can see how the mechanical (non-electric) parts work, however it's a little confusing how people would choose 1 gearing ratio vs another. Could someone explain? Nonetheless, I was looking at diyelectricskateboard's single bolt on motor mount w/drive wheel kit 16/36t, unless someone can offer opinions/alternatives.

People typically gear for 1:2 to 1:4 depending on wheel size, motor configuration, battery voltage, and riding environment. Lower reduction leads to higher top speed and lower torque and vice versa. 16/36T is a good ratio which will give you higher top speed, but if you're running a single motor configuration you may want to drop down to a 14/36T setup depending on the hills you'll be taking on. Keep in mind hub motors have a 1:1 ratio. 

> 4) Can someone explain how to choose a battery, I read the sticky on "What is Battery "C" rating" and understand the battery's capacity and peak output. I also saw that they recommended a 60a peak battery. But how would I go about picking what type/brand/size battery? and how would you estimate a battery's range? (if I went with a sk3 6364 motor, 83(?)mm wheels, standard gearing, flat terrain, and I weigh roughly 170lbs/77kg). Carrying onto the next point, I saw ESC's are offered in 6s/12s variants, which I'm guessing has to do with the battery

'C' = amp hour/discharge amperage. So a 5000mah pack with 100amp discharge current is rated at 20C (20*5=100). If you're running a VESC you'll need 50amp continuous discharge current max. You can run lipos you find off hobbyking but I'd recommend getting an 18650 pack such as the ones you can find on Enertion's or DIYelectricskateboard's websites. They offer 10s/12s packs. Range is approximately 1km for every 10wh of the pack depending on conditions.

> 5) ESC - I've heard a lot of good things about VESC but I also heard there was a steeper learning curve for it. I've done some programming classes in college, do you guys think I would be ok with the VESC? Also, what other popular/easy/(or maybe)cheaper ESC's are there out there?

VESC doesn't require any programming knowledge, but you have to configure it right or it can easily break or brick. Check out all the VESC tutorials here http://www.electric-skateboard.builders/t/new-vesc-user-read-this-complete-walktrough-of-the-vesc/2980

> 6) Lastly, I don't have a 3d printer, but I did see the g2tb mini controller mod and I like it a lot. Are there any similar out-of-the-box small controllers? or would they be around enertion's thumb stick controller's price range (kinda expensive).

I use this $60 controller http://miamielectricboards.com/shop-1/handheld-electric-remote, there are also other choices you just have to look. GT2B is a solid reliable choice, and perhaps @FLATLINEcustoms can make you an enclosure for the mod.
```

---
## \#4 Posted by: ouch_fiyah Posted at: 2016-06-14T12:46:36.957Z Reads: 90

```
Thanks Michael! 

I've seen that post and actually still have it open on one of my tabs. Only thing was it was kinda hard just looking at parts, without much explanation on why in real-world situations one would be better than another. And I tried using that calculator before but I got confused the first time, finally see how it works now. :thumbsup:

**I also saw your cheap shopping list, super helpful
```

---
## \#5 Posted by: ouch_fiyah Posted at: 2016-06-14T14:04:28.976Z Reads: 88

```
Wow thanks for the thorough reply Jinra!

1) Using the toddy616.blogspot calculator, I would probably opt for a 10s battery and 190kv motor. 

2) And I figured if I could use the trucks I have now, I could save some money. But I will probably end up buying some calibers or clone for the project. 

3) There aren't many hills where I live, it's flat as far as the eye can see haha. Is there a big difference between 14, 15, or 16t other than a few mph/kph (for example, do I get a lot more torque for losing a few mph)? Looking at things I may opt for 15/16t since there's a better chance I could use my board to commute than going up and down hills.

4) Thanks for the input, I'll probably opt for a 10s 18650pack. But I do have a question about the chargers, for example (product/electric-skateboard-battery-epower-pack-10s3p/) comes with either a 2A or 4A charger. Do I have to constantly monitor and unplug it when it's done? or are these somewhat "smart" chargers. And roughly how long does it take to charge a 18650 10s battery with a 2A o 4A charger?

5) I'll most likely get a VESC, the walk-through didn't look TOO hard :grin:

6) That's a pretty cool controller! I'll definitely take a look at it.


Thanks again for the input, it really helped me out a lot
```

---
## \#6 Posted by: Jinra Posted at: 2016-06-15T01:36:05.334Z Reads: 74

```
  you'l be fine with 16T. Try to gear for ~25 mph.

 You can plug it and forget it since it has a bms. You can calculate charge times be looking at the amp hours of the pack to the charge amperage. Looking at about 2-3 hours on the fast charger.
```

---
