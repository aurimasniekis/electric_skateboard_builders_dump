# Voltage Meter and Charging Port Diagrams

### Replies: 19 Views: 2557

## \#1 Posted by: Smorto Posted at: 2017-01-08T20:50:07.582Z Reads: 271

```
Hi all. I have done a fair amount of reading about diagrams and such on this forum, though super complex diagrams confuse me as I don't have the best understanding of circuits and wiring, in Esk8s.

I spent a little time today making these diagrams of potential things I would like to add to my super simple wiring I will be using on my first build. The wiring I will be using currently is the same as the diagram for the voltage meter but without the voltage meter if that makes any sense :slight_smile:. The first link is to a potential diagram for an LED voltage meter such as this one, [Voltage Meter](https://www.amazon.com/dp/B01CFNTNRA/ref=twister_B01CFKORCO?_encoding=UTF8&psc=1). I designed the Voltage Meter diagram to have the meter after the loop key so it will only turn on once the board turns on, though I am not sure if it will work. The second link is to a potential design of a charging port. I am fairly sure that the Voltage Meter diagram will work but am not so sure about how well the Charging Port wiring will function. These changes are all being made in an effort to achieve the final goal of having an enclosure that I don't need to open for charging or to check voltage.

This is the link to the google drawing of the [Potential Voltage Meter Wiring](https://docs.google.com/drawings/d/1OTONGWbgS9XbY82Uh9YTEgZYb8_zqEJVXfqQTjNvynY/edit?usp=sharing).

This is the link to the google drawing of the [Potential Charging Port](https://docs.google.com/drawings/d/1MeIy4zcjSTfMRzbmevLVJVmHHMrQ42v8yO28ufnNSbY/edit?usp=sharing).

Thanks in advance for your help!
```

---
## \#2 Posted by: mmaner Posted at: 2017-01-08T21:40:21.508Z Reads: 250

```
The voltage meter connection looks fine.  The charging port diagram will work but it doesn't need to be separate. 

As you are discharging in series you can charge I'm series as well.  Just move the positive to the other batteries positive and connect the balance wires to a x2 3S to 6S adaptor like this one.  https://www.amazon.com/JST-XH-6S-3S-BALANCE-ADAPTER/dp/B01BZLE7F6
Mount the 6S side to the enclosre.
```

---
## \#3 Posted by: Smorto Posted at: 2017-01-08T21:53:27.035Z Reads: 233

```
I see what you are saying, however there are two problems. The first is that I have two 4s batteries so that connector will not work :slight_smile:. The second is that I would do that as it is clearly the easier option but I only have a 6s capable charger, not an 8s. Thanks for the confirmation of the voltage meter connection.
```

---
## \#4 Posted by: mmaner Posted at: 2017-01-08T22:18:48.318Z Reads: 220

```
If you can come up with an 8S charger, there are x2 4S to 8S adaptors too.  Good luck.
```

---
## \#5 Posted by: Smorto Posted at: 2017-01-08T22:35:23.060Z Reads: 205

```
Yes, I will look into it but as a student I am on a budget as you can imagine :relaxed:. Are you sure that the configuration for the charging port would work though because that would be the cheaper route.
```

---
## \#6 Posted by: mmaner Posted at: 2017-01-08T22:48:21.939Z Reads: 197

```
The charging configuration will work, just make sure you include the balance connections. You can technically charge lipos without balance charging, but it's not a good idea.  Cell drift is the death of lipos.
```

---
## \#7 Posted by: JdogAwesome Posted at: 2017-01-08T22:56:32.243Z Reads: 197

```
I'd recommend using an 8S BMS because having to charge each battery like that and having your JST balance connectors coming out of your board is a huge pain in the ass because they can get corroded. And I can't stress this enough, DONT cheap out on things! I get that your on a budget, I was to when I first built my board, but I only ended up spending way more money fixing the problems I could have just prevented if I had just spent a little more in the beginning.
```

---
## \#8 Posted by: Smorto Posted at: 2017-01-08T23:48:06.771Z Reads: 185

```
Hmmmmmm, as of right now, I am probably going to stick with my setup without a BMS. This is simply because I already have the charger, and the materials to make the charging setup/diagram I have designed. Would putting an empty (empty meaning no wires coming off from it) JST balance cable on the protruding one help prevent corrosion? How about a rubber cover? I would use a defiantly use a rubber cover on the XT60 connectors that would be sticking out. On the next build (I am already thinking of the next one before this one is done :slight_smile:) I defiantly plan on using a BMS as well as making my own Liion 18650 pack. Thanks for your help!
```

---
## \#9 Posted by: JdogAwesome Posted at: 2017-01-09T00:02:28.175Z Reads: 171

```
No I already tried that lol. Water still gets in there and just ruins them. You could try making some sort of rubber cover for it with silicon or something. Also you can get an 8S BMS on AliExpress for right around $20 FYI.
```

---
## \#10 Posted by: Smorto Posted at: 2017-01-09T00:19:36.369Z Reads: 178

```
How about making a rubber cover out of Proto Putty? https://www.youtube.com/watch?v=7fwytA5r2Mw
The problem with the BMS for me is I have absolutely no idea how to set one up. I have read of how to do it but for some reason it goes right over my head.
```

---
## \#11 Posted by: JdogAwesome Posted at: 2017-01-09T00:38:55.304Z Reads: 168

```
Yeah I think that putty might work perfectly! I know GreatScott on YouTube has a build log of his EBoard were he used a JST connector coming out of his enclosure so you might want to check out how he went about doing it. Also wiring up a BMS is super simple, you just connect your JST connector into it, and wire your charging port to it. Plenty of people on here have done it so you could totally figure it out.
```

---
## \#12 Posted by: Smorto Posted at: 2017-01-09T00:52:33.686Z Reads: 158

```
I think I'll go the route of the exposed connector/putty for now and tackle the BMS later. Thanks for everything btw. If you don't mind me asking, soldering the voltage meter directly into the power cables should be alright correct? And in my setup the meter would only turn on once the board turns on right?
```

---
## \#13 Posted by: benwong Posted at: 2017-01-09T00:57:41.490Z Reads: 151

```
What charger u using? 
Single channel or duo? 
I have a same charging setup with you too. 
But when hook up to my dual channel charge, my charge get spark and dead.
```

---
## \#14 Posted by: Smorto Posted at: 2017-01-09T01:03:09.720Z Reads: 146

```
I am using the Imax B6 V2 Dual Power AC/DC Charger.
```

---
## \#15 Posted by: JdogAwesome Posted at: 2017-01-09T01:04:54.715Z Reads: 142

```
Yeah your voltage meter is hooked up properly. And how do you plan on charging it? I'm guessing in parallel right?
```

---
## \#16 Posted by: Smorto Posted at: 2017-01-09T01:08:52.344Z Reads: 147

```
I was planning on just charging each battery one at a time... but I do have a parallel charging board so I guess I could use that. Although I don't trust it as much in terms of balancing because it takes the average of each of the cells and charges to that if that makes any sense.
```

---
## \#17 Posted by: raxell Posted at: 2017-01-09T01:15:29.337Z Reads: 153

```
Hi!
Have you tried this?
http://www.electric-skateboard.builders/t/miami-electric-boards-diy-charger-how-to/4242
```

---
## \#18 Posted by: JdogAwesome Posted at: 2017-01-09T01:16:08.776Z Reads: 148

```
I guess that would work, but it's just going to make it a pain to charge. Best option would obviously be charging in series at 8S, but then you'd need a different charger so yeah.
```

---
## \#19 Posted by: Smorto Posted at: 2017-01-09T01:22:14.360Z Reads: 150

```
I have seen that yes, and I had thought that it wouldn't really come into play until now! lol. That would make things a little easier I guess but it could always be added later. I never knew I was going to be giving myself so much extra work by creating this thread! But in the end it should make for a better build.
```

---
