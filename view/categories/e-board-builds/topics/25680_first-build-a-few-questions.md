# First Build, a few questions

### Replies: 10 Views: 782

## \#1 Posted by: ShakeNBake7000 Posted at: 2017-06-19T10:30:29.674Z Reads: 83

```
Ok so, I'm new to this, so I don't know if I'm missing anything.
I'm going for a cheap first board.
The parts I'm planning to buy:
Deck: http://www.ebay.com/itm/222519778459?var=521367554733
Trucks, wheels and risers: http://www.ebay.com/itm/182587344126
Motor: https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6364-245kv-brushless-outrunner-motor.html?___store=en_us
2 Batteries: https://hobbyking.com/en_us/turnigy-5000mah-3s-25c-lipo-pack.html
ESC: https://hobbyking.com/en_us/hobbykingr-tm-x-car-beast-series-esc-1-8-scale-150a.html
Controller: https://he.aliexpress.com/store/product/Electric-skateboard-refitting-parts-DIY-800MAH-remote-receiver-2-4G-bench-technology-benchwheel/1967440_32791243047.html
Charger: https://hobbyking.com/en_us/imax-b6-dc-charger-5a-50w-copy.html
Motor Mount Kit: https://www.banggood.com/Electric-Skateboard-Belt-Motor-Mount-Bracket-Pulley-Screws-For-839097MM-Wheel-p-1105929.html

Ok, so those are the parts, and here are my questions:
Am I missing anything?
Do all my parts work with each other?
Are two 5000mAh batteries enough?
And will my charger come with the cables and connectors that are shown in this video to charge the board or do I need to buy them separately:
https://www.youtube.com/watch?v=O5gi35AtPSw
And do you have any suggestions for improving the build?
Sorry if I asked anything stupid I researched a lot and didn't understand much.
And English isn't my first language so sorry for any mistakes.
Thanks in advance.
```

---
## \#2 Posted by: Alanhunt123 Posted at: 2017-06-19T12:15:14.028Z Reads: 59

```
For the most part, it looks like you've found some decent parts that will get the board running. However, I believe that this setup will quickly leave you wanting more. 

5000mAh in a 6S configuration will result in 111 watt hours of energy (cell voltage * amp hours * number of cells, which is 3.7V * 5Ah * 6S). This will give you just under 10km, which goes by very quickly on an electric skateboard! You might consider getting a larger battery pack, like the 8000mAh packs from hobbyking. That, in 6S, would give you more like 15km, and if you stepped up to 8S would give you over 20km range!

My experience with that SK3 motor with the VESC speed controller is that you need at least 8S to get enough power out of it. But, you might have better luck with 6S using the speed controller you found, I haven't tried it. Perhaps someone else on this forum knows. 

Other than that, the build looks like it'll work. Do be careful when buying cheap parts. In my experience, it costs less in the short run, but costs more in the long run having to replace broken parts, and wanting to upgrade. 

Good luck with your first build, I hope it goes smoothly, and results in something you're satisfied with!
```

---
## \#3 Posted by: Alanhunt123 Posted at: 2017-06-19T12:21:43.964Z Reads: 49

```
Also, I don't think that battery has the right connector for the charger you found. You could buy an adapter or convert the batteries to XT-60 connectors, which does require knowledge of soldering. Never let the leads touch each other when removed from the connectors!
```

---
## \#4 Posted by: ShakeNBake7000 Posted at: 2017-06-19T13:55:16.694Z Reads: 50

```
[quote="Alanhunt123, post:3, topic:25680, full:true"]
Also, I don't think that battery has the right connector for the charger you found. You could buy an adapter or convert the batteries to XT-60 connectors, which does require knowledge of soldering. Never let the leads touch each other when removed from the connectors!
[/quote]

Thanks for the reply man! so two 8000mAh 3s would be what u meant? 
https://hobbyking.com/en_us/zippy-flightmax-8000mah-3s1p-30c-lipo-pack.html
this mabye?
and can you explain a little about what connector i need to buy and ill look up on how to connect it to the charger
edit: or mabye what charger will work with the battery
thank you very much for the reply man
```

---
## \#5 Posted by: Alanhunt123 Posted at: 2017-06-19T15:52:41.131Z Reads: 44

```
Those are precisely the batteries I was talking about.

In order to use them, you will need to change over your connectors for ease of use. I recommend XT-90 connectors with these batteries, as they can handle the current quite well. Here's a link to some.

https://hobbyking.com/en_us/nylon-xt90-connectors-male-female-5-pairs.html

Then you will either need to make or buy something similar to this to connect the batteries in series.

https://hobbyking.com/en_us/xt90-battery-harness-10awg-for-2-packs-in-series.html

In all, the wiring setup should look like this. I marked which plugs should be female and male with "F" and "M".

<img src="/uploads/db1493/original/3X/f/2/f2795875810340db7e23ce81a91fa980cf80eede.jpg" width="690" height="487">

Finally, you will need one of these adapters to be able to charge both batteries at the same time and ensure that the cells are balanced.

https://hobbyking.com/en_us/6s-battery-pack-balance-charge-adapter-lead.html

Make sure that battery towards the bottom in the above diagram is plugged into the balance lead with the black wire, otherwise you will get a big spark and harm your batteries!

To charge the batteries, leave the two batteries connected to the series adapter. Plug the free end of the adapter into the charger (which you may need to buy or make an adapter for). Then, plug in the balance lead adapter, and charge it as a single 6S battery.

You could also avoid using a lot of adapters by buying this battery, which has the same capacity. However, the Multistars are a bit lower quality, and might not last as long, and it also might not fit into your space requirements.

https://hobbyking.com/en_us/multistar-high-capacity-6s-8000mah-multi-rotor-lipo-pack.html

I hope this was helpful, and if you have any questions, feel free to ask!
```

---
## \#6 Posted by: ShakeNBake7000 Posted at: 2017-06-19T16:07:20.226Z Reads: 35

```
thank you for all the detail, really appreciated!
I understood everything except the part with the black wire, I get two connectors, one for each battery, but I need to plug the one with the black wire to the bottom battery? how to I know which one is the "bottom" one? 
really thank you for answering my stupid questions
edit:
forgot to ask, is there a charger that I can buy that won't require another adapter or is it necessary?
and what does the (copy) mean on the charger? the one i chose on hobbyking is copy and i dont understand what does it mean
```

---
## \#7 Posted by: Alanhunt123 Posted at: 2017-06-19T16:30:12.584Z Reads: 32

```
"copy" refers to the fact that it is not a genuine charger from iMax, but rather a knockoff made by some other company at a lower price. I have one, and it seems to work well enough, but this charger will be a little slow for charging an electric skateboard. It will be enough to get you started though.

What I meant by the black wire is that when you connect the two batteries in series, you will have one pack that has its main positive lead connected to the main negative lead of the other battery. This battery (the one towards the bottom of the diagram) should have its smaller balance lead connected to the balance adapter in the correct orientation (there are two possible ways to connect it, one of which will short the battery!). The correct orientation is for the bottom battery to be connected to the part of the adapter with the black wire.
```

---
## \#8 Posted by: Alanhunt123 Posted at: 2017-06-19T16:30:52.335Z Reads: 31

```
Oh, and either battery can be the "bottom" battery, just make sure it is consistent with both adapters which is which.
```

---
## \#9 Posted by: ShakeNBake7000 Posted at: 2017-06-19T16:56:00.310Z Reads: 28

```
I didn't understand what this part is <img src="/uploads/db1493/original/3X/7/3/730a1c00c29a8d1858769e059e382cac80dc876e.png" width="159" height="123">
is it this:
https://hobbyking.com/en_us/6s-battery-pack-balance-charge-adapter-lead.html
or this:
https://hobbyking.com/en_us/xt90-battery-harness-10awg-for-2-packs-in-series.html
in this video he didn't even connect the yellow connector to charge, it's really confusing me
https://www.youtube.com/watch?v=O5gi35AtPSw
and where are the black and red connectors to the charger itself? do I need to buy them too or do they come with the charger?
sorry for so many questions I get it if u don't want to answer anymore haha
```

---
## \#10 Posted by: xBRAZILx Posted at: 2018-02-01T01:29:31.556Z Reads: 12

```
i guess i watched this video at least 5 times and still dont know how the schema for charging throught balance leads work yet lol :face_with_raised_eyebrow: :sweat_smile:
```

---
