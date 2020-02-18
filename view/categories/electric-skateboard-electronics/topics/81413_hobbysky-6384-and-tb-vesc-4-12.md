# Hobbysky 6384 and TB VESC 4.12?

### Replies: 14 Views: 792

## \#1 Posted by: Allofyoush Posted at: 2019-01-19T19:55:38.992Z Reads: 118

```
I have a Hobbysky 6384 that I got for cheap on Ebay. Looks like it's in excellent condition, but I can't test it because the leads don't fit into the VESC. I'm getting some 5.5mm bullet connectors to solder onto it because it currently has 4mm. But my question is this: this has a 5pin sensor, but the VESC has a 6pin recepticle. Is it hopeless, or is there a way I can use the sensor? 
![IMG_20190119_144752|375x500](upload://dLm58JvwhyPs8TEvhmOr1lapmB4.jpeg) 
![IMG_20190119_143629|666x500](upload://vigFxVLQIfJ0W7bK4WzQs9k6wTO.jpeg) 

https://www.amazon.com/Hobbysky-Brushless-Outrunner-Sensorless-Skateboard/dp/B07FTS6RGX
```

---
## \#2 Posted by: venom121212 Posted at: 2019-01-19T20:00:45.021Z Reads: 109

```
Did you even try the search function man?
https://www.electric-skateboard.builders/search?context=topic&context_id=81413&q=Motor%20sensor%20wire%20adapter%20&skip_context=true
```

---
## \#3 Posted by: Allofyoush Posted at: 2019-01-19T20:01:13.589Z Reads: 108

```
yes. None of that is useful.
```

---
## \#4 Posted by: venom121212 Posted at: 2019-01-19T20:02:22.086Z Reads: 107

```
[quote="Allofyoush, post:1, topic:81413"]
But my question is this: this has a 5pin sensor, but the VESC has a 6pin recepticle. Is it hopeless, or is there a way I can use the sensor?
[/quote]

Many of those links directly answer this. Or can you not read?
```

---
## \#5 Posted by: Allofyoush Posted at: 2019-01-19T20:05:56.345Z Reads: 106

```
I've read some of them, and all I can see is an adapter with opposite voltage source and ground.
```

---
## \#6 Posted by: venom121212 Posted at: 2019-01-19T20:07:00.013Z Reads: 106

```
Try searching for 5 pin or 6 pin or something related to what you want to find. You're killing me smalls
https://www.electric-skateboard.builders/t/hall-sensors-5-wires-vs-6-wires/31626
```

---
## \#7 Posted by: Allofyoush Posted at: 2019-01-19T20:28:12.592Z Reads: 100

```
@venom121212 Just looked through all of it. I wanted to solder it myself, so I was looking for a tutorial, but the ones in the search weren't for the same thing. If it comes down to it, I can use
https://miamielectricboards.com/shop-1/oesc-motor-adaptor
or if I can find a detailed tutorial on which wires to solder to which, I can use this
https://www.banggood.com/Mini-Micro-JST-1_5mm-ZH-6-Pin-Connector-Plug-and-Wires-Cables-15cm-10-Set-p-1170230.html?gmcCountry=US&currency=USD&createTmp=1&utm_source=googleshopping&utm_medium=cpc_bgs&utm_content=frank&utm_campaign=pla-all2-rm-us-pc-purall&gclid=CjwKCAiAsoviBRAoEiwATm8OYD4qjPIX5mIQBK_Xus5AUgT9wd-DSPBg5q55ymnROBGKARAySiUy7BoCfl0QAvD_BwE&cur_warehouse=CN
```

---
## \#8 Posted by: venom121212 Posted at: 2019-01-19T20:34:32.350Z Reads: 91

```
https://www.electric-skateboard.builders/t/hall-sensors-5-wires-vs-6-wires/31626/10?u=venom121212

The 3 phase wires of the sensor order don't matter. Just make sure you match v+ and ground like the solution says.
```

---
## \#9 Posted by: Allofyoush Posted at: 2019-01-19T20:39:14.461Z Reads: 88

```
so it looks like the one I can skip over is temp, is that correct? on the Vesc it's next to 5v. Now all I'm unsure about is which colors on the Hobbysky correlate to which pin. In order, it's black, orange, white, yellow, red. From what I've seen, red is 5v, and black is GND, right? So the order of orange, white, and yellow doesn't matter. I'm just being extra careful so I don't blow up my VESC. I know starting unnecessary threads is frowned upon, but since nothing was exactly the same, I just wanted to be careful.
```

---
## \#10 Posted by: Andy87 Posted at: 2019-01-19T20:48:02.593Z Reads: 82

```
[](http://)Yes
```

---
## \#11 Posted by: venom121212 Posted at: 2019-01-19T20:49:24.468Z Reads: 79

```
If you asked this question instead of the original one, it wouldn't be frowned upon at all. Just make sure you search the basics of your question and we'll all be nicer :grinning:
```

---
## \#12 Posted by: Allofyoush Posted at: 2019-01-19T20:53:13.189Z Reads: 75

```
Ok, sorry. I just wasn't sure how to put it. The Banggood wires have a different color order, but I guess that doesn't matter. So I'll get this, then solder the red wire from the motor to the 5v wire and leave a space for temp.

Here's my build so far:
https://docs.google.com/spreadsheets/d/167cWqPTjEUCLcpPeNMNj8Ifrkz30whCtTQ1d6yCb6Tg/edit?usp=sharing
```

---
## \#13 Posted by: Sn4pz Posted at: 2019-01-19T22:56:55.401Z Reads: 67

```
Your google-fu must be some weak shiz if you can't use the power of *keywords* to find what you need :thinking:

As my math teacher used to say, "exhaust yourself and the libraries surrounding you  before coming to me for a drink, because I'll make you drink the whole jug"

Also keep in mind this forum isn't the only spot for esk8 advice, endlessphere has some great threads to familiarize yourself with parts and their intricacies
```

---
## \#14 Posted by: Martin Posted at: 2019-02-18T15:12:03.250Z Reads: 51

```
Hello !

Could you let me know how to convert sensor connector?

Motor -> VESC
Red -> 5V
Black -> GND
Is that right???
```

---
