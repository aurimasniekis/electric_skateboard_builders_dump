# Thoughts on my PCB holder for 18650

### Replies: 16 Views: 1171

## \#1 Posted by: RazzleDazzle Posted at: 2018-05-02T13:12:45.589Z Reads: 200

```
Hey Guys,

I was wondering if you could give me some feedback on my PCB and whether you think it will work well.  I wanted to use the LiOn holders I bought on amazon so i could hot swap batteries if they fail.  I wanted to make it modular so that the overall battery cell could flex across the PCB array.

https://www.amazon.com/gp/product/B071K5FCM1/ref=oh_aui_detailpage_o01_s00?ie=UTF8&psc=1

the PCB is meant two hold 2x 4pack batteries to create a 4P cell, which then feeds to the adjacent one.  SO in a sense is 2S4P per PCB, then i'd use 12AWG wire to interconnect 5 PCB's to create a 10S4P pack.  I put a connector for the BMS, two per PCB.

![final|690x346](upload://nFOt1g9Kt5p3NDDnn69QhqW1V7w.PNG)

Hopefully my explanation made sense.  Thoughts?
```

---
## \#2 Posted by: Ronny_CTS Posted at: 2018-05-02T13:20:25.702Z Reads: 184

```
I don't think those battery holders will be able to deliver the full amperage that the batteries are capable. Do you know the max amp rating for those holder?
```

---
## \#3 Posted by: akhlut Posted at: 2018-05-02T13:21:39.651Z Reads: 174

```
Save space and elminiate the inteconnection terminals and the balance terminals.  Have one side of the PCB be positive and the other side be negative and use the opposite side of the PCB for the series connection.

And skip the battery holders.
```

---
## \#4 Posted by: RazzleDazzle Posted at: 2018-05-02T13:23:26.564Z Reads: 176

```
So basically scrap the idea... :frowning:

Whats wrong with the battery holders? I've seen them used in other battery pack builds and it doesnt seem like there were issues with them
```

---
## \#5 Posted by: akhlut Posted at: 2018-05-02T13:31:39.438Z Reads: 165

```
If you're going to go the PCB route they're superfluous.  Just use hotglue to secure the cells and fishpaper to insulate.

Think about this layout:

![image|690x425](upload://dY1F09q4v4RhKw1mogkWaT2cfXy.png)

No through-holes to solder, and you can achieve a higher cell density.  just make your connections on the exposed bus.

Check this out:
https://www.electric-skateboard.builders/t/no-words-just-pictures-delete-words-use-pm/2992/3036

Same idea, just a single P-group.
```

---
## \#6 Posted by: RazzleDazzle Posted at: 2018-05-02T13:36:33.934Z Reads: 140

```
I see... I dont want to get a spot welder though...  I thought my route would be easier and only requires the tools I have
```

---
## \#7 Posted by: akhlut Posted at: 2018-05-02T13:45:32.868Z Reads: 138

```
Gotcha.

Honestly, I wouldn't try this approach.  It's going to cost you a good amount of time and money to try and get a usable pack that may or may not work and may or may not be reliable.  It sucks, but bite the bullet and get a spot welder.
```

---
## \#8 Posted by: pakue Posted at: 2018-05-02T14:15:28.220Z Reads: 133

```
You can also use the backside copper layer for current handling. What I usually do with high current traces is to remove the solder mask on top and add solder manually. That way you can get much more power from a trace than the copper is rated for.
```

---
## \#9 Posted by: RazzleDazzle Posted at: 2018-05-02T14:17:51.365Z Reads: 133

```
hmm thats an interesting idea, im not sure how to remove the solder mask on the traces...  Have you done something similar to what I'm doing?
```

---
## \#10 Posted by: Ronny_CTS Posted at: 2018-05-02T14:28:07.674Z Reads: 129

```
The terminals on those holder are probably made of misture of steel to maintain springiness. Steel is a poor electric conductor and heats up. So if you have 18650 cells capable of delivering 15 amp  continuously you need to have good conductivity of else you will bottle neck you batteries. Thats why people use nickel or copper to build batteries, allowing a complete battery pack to deliver 60 amp and more. 

However, from what i know, there are two main attempts to build 18650 pressure battery holders:

* [Vruzend kit 2.0](https://vruzend.com/product/vruzend-battery-kit-v2-0/) capable of delivering 15 amp per cell continuously

* [N.E.S.E Modules](https://www.electric-skateboard.builders/t/n-e-s-e-no-solder-module-battery-packs/36847) which were tested at 6P delivering 200 amp (30 amp per cell)

These kits are made of copper connections and allow for high amp conductivity. However, add size and cost.
```

---
## \#11 Posted by: RazzleDazzle Posted at: 2018-05-02T14:32:15.021Z Reads: 121

```
I've seen those options you linked, i read that the pressure holders over time can come loose if there's too much jarring happening... seems like everything has a trade off.

I guess i can try it out and see how it works, the one good thign about this is that I can take the batteries out and try a different approach
```

---
## \#12 Posted by: deucesdown Posted at: 2018-05-02T15:20:39.744Z Reads: 121

```
[quote="RazzleDazzle, post:11, topic:54127"]
too much jarring happening
[/quote]

NESE is well tested for vibration

http://18650.lt/index.php/2017/05/01/vibrotion-test-results-of-compression-pad/

https://www.youtube.com/watch?v=93JBo87LJiU

He's on the forum if you have questions.
```

---
## \#13 Posted by: Mikenopolis Posted at: 2018-05-02T20:54:38.572Z Reads: 106

```
[quote="RazzleDazzle, post:11, topic:54127"]
read that the pressure holders over time can come loose
[/quote]

I wonder if using these systems and adding a shrink wrap over it would help with the issue, but then you could potentially get a loose nut rattling around within the wrap once it come loose
```

---
## \#14 Posted by: pakue Posted at: 2018-05-03T00:46:33.771Z Reads: 92

```
Depends on what design software you are using. Usually you have to draw the same trace on the f.stop/b.stop layer. 
I used it for a connector board of a 2000W supply before.
```

---
## \#15 Posted by: RazzleDazzle Posted at: 2018-05-23T01:17:49.665Z Reads: 87

```
Wanted to post an update since I got my boards back and soldered two "packs" together.  I tested the voltage across both connected packs and make sure  it came out to 13.68v (4*3.42v).  Sure enough, it's all good.![20180522_210829|250x500](upload://8YN5Euxd3MYQGefETWhafCEPftD.jpg)![20180522_210848|250x500](upload://QaDrmL4qpnL6mI9gFw7m6Xx6WD.jpg)![20180522_211000|690x345](upload://5tfT4IzPvX6kkCpmTMNJvs6KSo8.jpg)![20180522_211014|690x345](upload://u1BA3mnjHjymi1QEpybAMQAeJMW.jpg)
```

---
## \#16 Posted by: TheMrLarin Posted at: 2018-07-06T12:47:49.068Z Reads: 64

```
I like your 2S pcb design, great idea! I'll probably do something similar pcb wise when the time comes :wink:
```

---
