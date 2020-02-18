# Battery Choice (lipo vs li-ion)

### Replies: 9 Views: 1652

## \#1 Posted by: Caydenfish Posted at: 2018-05-19T05:13:44.204Z Reads: 164

```
The entire time I have been planning my build, I have leaned more towards Lipos, due to my lack of knowledge about connecting 18650s with Nickel, however, after more research, I really want to use 18650s due to the ease of charging. I am planning a 10s build on a Turnigy 6374 192kv single motor. 

So my question is, would two sets of 10 18650s (https://www.ebay.com/i/253454362448?chn=ps&ul_ref=https%253A%252F%252Frover.ebay.com%252Frover%252F1%252F711-117182-37290-0%252F2%253Fmpre%253Dhttps%25253A%25252F%25252Fwww.ebay.com%25252Fi%25252F253454362448%25253Fchn%25253Dps%2526itemid%253D253454362448%2526targetid%253D399820205491%2526device%253Dm%2526adtype%253Dpla%2526googleloc%253D9028740%2526poi%253D%2526campaignid%253D1029894471%2526adgroupid%253D50980675872%2526rlsatarget%253Dpla-399820205491%2526abcId%253D1130056%2526merchantid%253D116340693%2526gclid%253DCjwKCAjw8_nXBRAiEiwAXWe2yQYUVZggBWUlr0D0ocTYacC9TTqWX4NaTkR3S84hEpK9dstelZLBFhoC9F4QAvD_BwE%2526srcrot%253D711-117182-37290-0%2526rvr_id%253D1535610766120%2526rvr_ts%253D76bfc62c1630abc667c34040ffeb5cd1&var=552626780278) connected in series work? If that doesnt make sense, I would make two seperate 10 battery long strips commected in parallel, then connect those together in series. I have a stiff but low board, so I don't want to stack the strips of batteries, instead I would like to yse a long enclosure to maximize clearance. Is there somewhere I could get battery holders that would support this power? That would make this way easier.

Lastly, are many RC Car shops willing to help? I would just need some guidance from someone knowledgeable, and am willing to pay.
```

---
## \#2 Posted by: MysticalDork Posted at: 2018-05-19T05:29:02.558Z Reads: 148

```
@Caydenfish 

A couple things: First, those HG2 cells aren't really "30A" cells. They start to sag pretty badly at 15.

Second, samsung 30Q cells perform better than HG2 cells, even though they're "only 15A" rated - They have less voltage drop  even at 20A.

Third, 2p is not enough, no matter what 18650s you use. You need at least 3p to get enough current and keep the voltage drop to a minimum.

Fourth, I personally don't trust mechanical cell holders much past about 5A/cell, no matter how robust - vibration just causes too many problems.

Lipos can be charged just like 18650s, and if you add a BMS, you can even use the same two-wire brick - You don't need a balance charger that way.
```

---
## \#3 Posted by: Caydenfish Posted at: 2018-05-19T05:32:34.095Z Reads: 132

```
So you would recommend I use my original plan of a 2x 5s 8000mah setup in series, going to a BMS? If I did this would I need a lipo specific charger or could I run a 3 pin female charging port to the BMS?
```

---
## \#4 Posted by: Caydenfish Posted at: 2018-05-19T05:34:01.200Z Reads: 126

```
I just re-read what you said, ignore the question about the Lipo balance charger, so I could use a 3 pin?
```

---
## \#5 Posted by: MysticalDork Posted at: 2018-05-19T05:39:35.564Z Reads: 123

```
@Caydenfish You only need two pins, positive and ground. Whatever type of plug you use is up to you. I've used XLR because I had them lying around, but they're a little big. Others use 5.5*2.5mm barrel jacks. I've also seen aviation type plugs with screw collars. 

Doesn't matter as long as the board matches the charger.

As long as the charger is designed for a 10s lithium battery, (37v nominal, 42v max) it doesn't care whether it's 18650 or lipo pouches. the chemicals are the same inside.
```

---
## \#6 Posted by: Caydenfish Posted at: 2018-05-19T06:15:27.290Z Reads: 113

```
Half of the diagrams of 10s BMS's I am seeing have the charge port negative going to P-, whereas others have it going to Ch-.... Whats this about?
```

---
## \#7 Posted by: MysticalDork Posted at: 2018-05-19T06:22:00.352Z Reads: 111

```
Depends on how the BMS is laid out. There is more than one way to design a BMS is all.
```

---
## \#8 Posted by: b264 Posted at: 2018-05-19T06:30:18.775Z Reads: 107

```
[quote="Caydenfish, post:1, topic:55968"]
I really want to use 18650s due to the ease of charging.
[/quote]

You can use a BMS and regular 2-pin charger for lipo as well.  Why more folks don't do it is beyond me.  I have one esk8 set up that way.  One single 5.5mm x 2.1mm charger jack, 2-conductor.
```

---
## \#9 Posted by: Caydenfish Posted at: 2018-05-19T06:33:45.807Z Reads: 99

```
Sweet, I think after reading more up on it I may do a 5x 2s 5Ah setup like @Namasaki did in (http://www.electric-skateboard.builders/t/high-power-10s-lipo-battery-pack-with-bms/10014) the wiring diagram he included seems like it will make this whole process so much easier, plus the slimness of the 2s batteries will help with the slim enclosure I will need. Thank you both for your help! MysticalDork your the man! Thanks for the help on multiple of my threads!
```

---
