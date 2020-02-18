# Wallet Breaker &#124; custom 31&rdquo; deck &#124; 190mm Paris racing/Caliber combo &#124; 149kv SK3 &#124; 3x 4S 6.6A 60C LiPo &#124; Chaka VESC&hellip;.what soldering will need to be done here?

### Replies: 17 Views: 1519

## \#1 Posted by: itsmikeholland Posted at: 2016-06-04T21:28:34.264Z Reads: 186

```
<img src="/uploads/db1493/original/2X/e/e55b51fc899114046b9d3e7765660282c5c5f852.jpg" width="690" height="388">

I should first mention that the shape of the board is not final, after a couple beers I decided to hit it with a hack saw to reduce its size and weight. I'm gonna trim it up with a table saw after everything arrives. Rides awesome.

Here's what I currently have, the motor and batteries are both 4mm plugs, the switch appears to be larger, I'm assuming 5.5mm. I have a motor pulley and a single caliber truck coming from torque boards, as well as a chaka vesc with 4mm connectors. 

I'm torn between whether to wire my batteries in series or parallel, since I have a 3x 60c 4s batteries. I'm not sure if its gonna be healthier for the electronics to run 12s or if 4s at 60c is enough for city commuting with some big hills.

Motor: Turnigy Aerodrive SK3 - 6374-149kv Brushless Outrunner
Batteries: 3x Turnigy 6600mAh 4S 14.8V 60C
Torque Boards power switch
12mm 15/36T pulley system
90mm flywheels

I'm still waiting to order the caliber truck, torqueboards receiver, and a chaka vesc with 4mm connectors and an anti spark, since it appears to be in stock.

What soldering am I going to need to do? Can't I just buy 4mm to 5.5mm adapters and not need to solder anything? I'm building my own enclosure since I'm going to make my board as short as possible once all the parts arrive and I can visualize where everything can fit. 

Thanks in advance for the help! This forum rules!
```

---
## \#2 Posted by: treenutter Posted at: 2016-06-04T22:01:08.242Z Reads: 155

```
@itsmikeholland looking good. I think that you might not need an antispark switch if you already have TB's power switch. Just a thought to save some money. 

In terms of soldering, you'll need to get connectors for those motors and solder them on, unless you're going to use the connectors already there. You'll also need a serial or parallel cable to wire them all together in whichever manner you're thinking of (I'm guessing serial to get 12S). 

If you got an Ollinboard VESC with 4mm connectors, you won't need to solder the motor-side of the ESC unless the cabling isn't long enough.

You'll need to file a flat spot on the motor shaft of your SK3, you can use a dremel tool or a hand file.  

Also, could you rename this post to describe your build like this:

Project Name | Deck Name | Trucks | Motor type | Mounting method | Voltage/Battery | ESC
```

---
## \#3 Posted by: Namasaki Posted at: 2016-06-04T22:10:33.541Z Reads: 153

```
Every hobbyist should be able to solder. You need to learn how.
There are plenty of videos about soldering on youtube.
Here are some important tips:
For heavy gauge wire and connectors, get a high power soldering gun Like This:
http://www.amazon.com/D550PK-120-volt-200-watt-Professional-Soldering/dp/B00002N7S1/ref=pd_sim_469_22?ie=UTF8&dpID=41AbTn5FVJL&dpSrc=sims&preST=_AC_UL160_SR158%2C160_&refRID=0BHQPJ96VH9WYDAV9AMD
These are best in my opinion because they heat very fast and its easier to keep the heat localized when soldering.
60/40 lead base solder is very easy to use.
When you purchase connectors, get extras in case you mess up.
5.5 mm bullet connectors are what come on the HV switch
I use 5.5mm bullets on batteries and Esc's. You can also use them on motor wires. They are probably the easiest to solder.
You will also need something to hole the wire and connector while your soldering it.
Like this: 
http://www.amazon.com/ProsKit-900-015-Helping-Hands-Soldering/dp/B002PIA6Z4/ref=sr_1_4?s=hi&ie=UTF8&qid=1465078034&sr=1-4&keywords=helping+hands
And this is great for cleaning the soldering tip:
http://www.amazon.com/Hakko-599B-02-Solder-Cleaning-Holder/dp/B00FZPGDLA/ref=pd_sim_469_1?ie=UTF8&dpID=51B7RqNpe1L&dpSrc=sims&preST=_AC_UL320_SR278%2C320_&refRID=0ZFS92RX44RVNSAA8W3T
```

---
## \#4 Posted by: itsmikeholland Posted at: 2016-06-04T22:15:22.312Z Reads: 128

```
Thanks for all the recommendations! shouldn't I just replace the 5.5mm connectors with 4mm, since basically every other piece is 4mm? I was hesitant to commit to soldering because this board has been a non-stop "oh wait, I need to buy all this other gear to make this one piece work", my costs are about to go over $900 and I was kinda freaking out since I originally estimated it to be under $800. So this is all I'll need to solder everything? $60 isn't a bad investment, I can probably save that much by not buying plug and play.
```

---
## \#5 Posted by: Namasaki Posted at: 2016-06-04T22:21:15.855Z Reads: 122

```
Tools are an investment that will last a lifetime. These soldering tools are relatively inexpensive and chances are that you will need them again and again.
Besides I don't know of any 4mm to 5.5mm adapters. And even if  you could find them They would be expensive and make your wiring bulky and add resistance and increase the possibility of poor connections.
```

---
## \#6 Posted by: itsmikeholland Posted at: 2016-06-04T22:25:23.080Z Reads: 116

```
Thats how I see it, I actually have a soldering iron but wasn't able to use it to get the usb port off of my phones chip, so I think I'll have to buy new. I'll take your word for it and solder on new connectors for the power switch. I'm guessing I'll need heat shrink as well for the new connection?
```

---
## \#7 Posted by: Namasaki Posted at: 2016-06-04T22:31:52.826Z Reads: 115

```
oh ya, forgot heat shrink and a heat gun to activate it. Don't try to use a fire to activate shrink wrap like I seen some people do...
Heat guns are  inexpensive now on amazon
```

---
## \#8 Posted by: Namasaki Posted at: 2016-06-04T22:33:37.592Z Reads: 107

```
If your planning to use 4mm banana connectors, be advised that they don't fit very tight together and can work loose with vibration. The  5.5 mm bullets can handle more current and fit much tighter together.
```

---
## \#9 Posted by: itsmikeholland Posted at: 2016-06-04T22:48:31.817Z Reads: 107

```
fuhhh this isn't your fault, but this is exactly what I'm talking about. I'll just use the 4mm connectors for now, I don't want to accidently mess up $200 worth of explosive batteries for the sake of more current until I'm more comfortable with them. This should all be in the basic parts thread, it makes it seem like you can just buy 6 parts and be on your way!
```

---
## \#10 Posted by: Namasaki Posted at: 2016-06-04T23:12:35.349Z Reads: 107

```
Here's a funny story, I bought Zippy compact batteries and thought, awesome, they already come with 5.5mm connectors. Come to find out, they put the connectors on opposite of everything else. So I had to cut them off and re-connect anyway.
```

---
## \#11 Posted by: Namasaki Posted at: 2016-06-04T23:16:24.891Z Reads: 98

```
I was planning to use 5mm Ecs connectors at first so I bought a bunch of them then later went with bullets. 
Now I have all the Ecs connectors and parallel adapters just sitting in a spare parts box.
```

---
## \#12 Posted by: itsmikeholland Posted at: 2016-06-04T23:20:15.208Z Reads: 102

```
d'oh! I have a feeling that my build is gonna turn out awesome though, I think I'm just stressing because I've spent so much money and am still pushing myself to and from work and working 60 hours a week. Once I get all the parts and am able to cruise, it's gonna finally feel worth it. thanks for all of your input!
```

---
## \#13 Posted by: Namasaki Posted at: 2016-06-05T02:48:28.159Z Reads: 92

```
Do you live in Holland?
Or is that your name?
```

---
## \#14 Posted by: itsmikeholland Posted at: 2016-06-05T02:51:55.064Z Reads: 87

```
Nah i live in los angeles, holland is just my last name.
```

---
## \#15 Posted by: Namasaki Posted at: 2016-06-05T02:52:38.270Z Reads: 88

```
What do you need to change connectors on?
```

---
## \#16 Posted by: itsmikeholland Posted at: 2016-06-05T03:23:25.949Z Reads: 91

```
Im thinking ill only do it on the power switch,  since its the only one thats unlike the others. From 5.5mm to 4mm. I actually think my roommate might have the right tools. Do you think its gonna make a significant difference in performance to have the smaller connectors?
```

---
## \#17 Posted by: Namasaki Posted at: 2016-06-05T03:59:27.852Z Reads: 95

```
it should be fine with 4mm connectors. Your not gonna be pulling a lot of amps with 12s voltage. Maybe 30 amps if your going up a steep hill.
I'm using 4mm banana bullets on my motor wires and its fine.
If they get loose, you can tighten the banana version by taping the tip of the male connector on a piece of wood to expand the ribs. Just be careful not to over do it.
If it's the other type similar to the connectors on your switch only smaller then you can press a small phillips screw driver into the end of it and spread it a little to make it solid connection.
```

---
