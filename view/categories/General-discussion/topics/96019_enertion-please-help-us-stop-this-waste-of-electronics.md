# Enertion please help us stop this waste of electronics!

### Replies: 17 Views: 708

## \#1 Posted by: seaborder Posted at: 2019-06-06T09:48:40.873Z Reads: 285

```
Hey Enertion Guys @barajabali @EnertionSupport @Deodand 

First time Thanks for the work with the Foxboxes I still love this thing!

But I really have a problem. 

When repairing - every 3 Focbox has a burnt pad for the direct fets. It feels so bad to not be able to use all those broken Focboxes anymore. At first I thought, yes, I can take it for another vesc repair, but there are more defective circuit boards than components that I could ever use. 

On the one side I can understand you guys because its electronics and you never know what people did with it. On the other side the burned directfet pads are clearly a problem that happens to much people and YOU GUYS designed the focbox!

You do not produce the Focbox anymore anyways... Can you please give us the plans to re-create the Pcbs and bring all these good components back to life? Iam not able to reverse engineer the pcb. I understand that you might have a problem with that but it can not be for me that you sell partly OPEN SOURCE stuff for Diyer but then you do not really support us! That's a double game for me and the plans are not for a new top secret airplane.

I may have a compromise - can you make at least a few focbox pcbs for us if you do not want to publish the plans? I think many people would be interested in it.

I really want to stop that waste of electronics!
I hope you understand my / our concerns.

Thank you for everything!

![0|374x500](upload://dlMd7zajDAZoikXGQBAWEt1jaCJ.jpeg)
```

---
## \#2 Posted by: ARetardedPillow Posted at: 2019-06-06T10:37:24.844Z Reads: 252

```
+1 on this topic
```

---
## \#3 Posted by: dareno Posted at: 2019-06-06T10:44:39.570Z Reads: 246

```
Thought the design was open now?  No?
```

---
## \#4 Posted by: seaborder Posted at: 2019-06-06T10:50:41.394Z Reads: 240

```
I dont think so, if thats correct I take everything back. But I dont think so
```

---
## \#5 Posted by: ARetardedPillow Posted at: 2019-06-06T10:50:55.365Z Reads: 240

```
Yeah but I have no idea where the files are and I can only find 1.3 files
```

---
## \#6 Posted by: seaborder Posted at: 2019-06-06T10:54:17.413Z Reads: 231

```
schematics are online sure they are open source, but cant find the file for the pcb manufacturer dont think there even is one, thats why I started that post :expressionless:
```

---
## \#7 Posted by: dareno Posted at: 2019-06-06T10:55:29.556Z Reads: 228

```
I would like to say that surprises me but sadly it doesn't.    Abuse of open source design is a habit of enertion.
```

---
## \#8 Posted by: banjaxxed Posted at: 2019-06-06T11:19:56.469Z Reads: 213

```
Allow me to be devil's advocate for this

1) The actual gerber files are not required to be published in order to meet VESC O/S requirements. In fact VESC simply have a diagram with paths, a pdf I think. From that you have to design your own schematic as Stewii did against the VESC6, this results in a gerber that you can have produced.

Enertion also did this with the VESC 4.12 and made some changes to the power stage to make it DirectFET I believe if you dig hard enough you can find a schematic, but unless you are willing to redeign/transfer the pdf into Eagle/KiCAD or one of those other programs then you will never get a resulting gerber file to have made as an end-user.

Even Stewii did not release his for the VESC6-based ESCape. He simply sold on the ready made PCBs to those who really wanted to make themselves. But now he disappeared without trace(!) and this is sad.

Chaka did something similar to Enertion for the 4.12. The pcb was not released or was then pulled and leaked a little. No point in Ohlin boards making ESCs if there is a pcb released to compete with...mostly people are cheap, I include myself in that sweeping statement.

2) If you were still in the business of producing ESCs, why would you release a gerber to cannibalise your sales?

Why would you even sell a PCB? Removing all the still ok components for reuse is a huge overhead & challenge to the end-user & opens the maker to competition on their own product from those with production skills & access to cheap components aka China or nefarious individuals.

So I can still understand wanting to sell you a new ESC if you are not covered by warranty and you have blown a hole through the PCB under the FETs sometime after warranty. At some point it has to be a case of 'tough shit'.

A business has to be able to sell product in fairness, otherwise what's the point? Different if you are an individual with another primary source of income with a deep love of O/S, but it's challenging to put food on the table solely dependant on O/S.

My advice if you have the skills and equipment & desire is to cannibalise what you want when you have a repairable one.

Or get creative
https://www.electric-skateboard.builders/t/updated-with-location-california-santa-monica-meet-up/6994/16?u=banjaxxed

https://www.electric-skateboard.builders/t/fried-my-focbox/34287/5?u=banjaxxed

but sometimes as may be the case in the picture up there ^
https://www.electric-skateboard.builders/t/focbox-mosfet-explosion/46309/3?u=banjaxxed

Or to design your own PCB.. And certainly consider dialling back your setting if using a stock heatsink

Until one of the E.E. clever folks puts out a truly O/S design, then this is the current state of things in VESC-based controllers. Watch Shamen, he is not putting food on the table off it (yet) and others who are, would be understandably be a little nervous & possibly rightly so. 

There is no VESC6 derived gerber out there to print off a few PCBs, but it won't be long I feel, that's where it's going to get to -  unless a vendor can produce at FlipSky prices which undercuts a home effort they are in trouble without also added value features which not in Vedder's core design & you better be price-competitive.

That is why there is a huge propriety design added value touch to anything coming out from the big boys regarding controllers/BLE/dohickys = features & forks. 

It's difficult to close fences around Vedder's top-level O/S, but it's the only way if you want to mass manufacture & sell end-product. 

Business Vs Ideology
```

---
## \#9 Posted by: seaborder Posted at: 2019-06-06T12:31:15.413Z Reads: 162

```
I'm just more than creative,

please do not get me wrong, of course it's not about the end user. If someone lets fix his focbox it's not about the end user also. But where and when do you make the difference? Or do you think everyone with a broken fetpad was like "ah today Iam going to brake the pad because thats fun" WTF

But I still did not realize why enertion is such a big problem to collect some money from us and make a few pcbs to get your devices up and running again. Or would like to tell me again enertion "no, we do not help because we are doing so big business so please buy the unity". People already build their own Vescs for that very reason, but then at least open the plans or point out in advance that such things can break. But you act as if you sell the perfect vesc and if something breaks you are not responsible. If at 100 cars produced, 20 cars in the engine begin to burn, then it is the driver or the car with missing protection mechanisms?
    

[quote="banjaxxed, post:8, topic:96019"]
If you were still in the business of producing ESCs, why would you release a gerber to cannibalise your sales?
[/quote]

What's so bad about that? I've even suggested you a compromise without her out the plans.
You can even earn easy money with it ...


[quote="banjaxxed, post:8, topic:96019"]
Even Stewii did not release his for the VESC6-based ESCape. He simply sold on the ready made PCBs to those who really wanted to make themselves. But now he disappeared without trace(!) and this is sad.
[/quote]


Yeah sure, but he does not do youtube videos where he says about 100 times how great it all is for diy like "build your own board with our parts" and "THE BEST SPEED CONTROLLER EVER" blabla right? And at least he made some pcbs.

 Sorry but that pisses me off, many people could make vescs or electronic skateboards, but these people also know that this hardware is unfortunately prone to errors and then let it. And I ask for no replacement or something like that. Just for a few PCBS for which we would pay!!

I really dont want to be a dighead or sth like that, I think iam even a nice guy. I just thought you can help us here with some pcbs. Enertion sells electronics for diyer not iphones..

Its not Business Vs Ideology. Its getting both together or you customer wont stay.

So please just think about it to produce some pcbs in china and send them to us it isnt that hard.
```

---
## \#10 Posted by: banjaxxed Posted at: 2019-06-06T12:40:52.455Z Reads: 142

```
[quote="seaborder, post:9, topic:96019"]
Or would like to tell me again enertion “no, we do not help because we are doing so big business so please buy the unity
[/quote]

They stopped making it as both products would compete against each other, you could not make the foxbox cheap enough to have it as a product & pricepoint differentiation, despite the different H/W design, they do kind of the same thing...drive brushless motors. A single Untiy is almost certainly cheaper to manufacturer over two focboxs

Selling you a pcb is risky for the reasons I went over in the last post, that and if you mangled it they could get additional problems from that such as liability.

Find me a maker who will sell you a pcb outside of stewii who vamoosed...

What may work for you is to wait for @shaman's designs and transfer viable components onto his design. I think he plans to sell kits, but not DirectFET package, also MCU is different? I think.

Or buy old broken repairable focboxes and harvest your good components for them.

Companies can't sell blank pcbs without destroying their market line. Even if you're sure it's someone who bought a valid product a year or two ago. It's not Enertion...nobody does it
```

---
## \#11 Posted by: seaborder Posted at: 2019-06-06T12:53:15.973Z Reads: 137

```
Yeah but what acutally is the market line? Diy or finished builded boards? They mix it up for me. I can understand that totaly from the bsiness side. I understand you cant produce both. Totaly fine. But in my opinion when you reach out to diyers so also try to help them. And I was just asking for some of the pcbs I pay for np - not a new focbox. Iam not into that Business maybe I would understand if I would be. But I think it wouldnt be that difficult at all to produce some old pcbs. 

Dunno, but thank you anyways for your concerns and the info :)

I dont think some pcbs will affect enertion. And also I thought we are a community and you guys are a part of it. The last thing I want is to harm someone. :)
```

---
## \#12 Posted by: shaman Posted at: 2019-06-06T17:03:18.970Z Reads: 97

```
[quote="banjaxxed, post:10, topic:96019"]
also MCU is different? I think.
[/quote]

Nope. Different DRV but same MCU.
```

---
## \#13 Posted by: seaborder Posted at: 2019-06-06T17:09:28.881Z Reads: 94

```
Yeah cant wait for your vescs, awesome work 👌
```

---
## \#14 Posted by: Blasto Posted at: 2019-06-06T17:27:38.306Z Reads: 90

```
i have some bare pcb's if you feel like transferring the components, just cover postage
```

---
## \#15 Posted by: seaborder Posted at: 2019-06-06T18:07:58.718Z Reads: 78

```
what how :D
```

---
## \#16 Posted by: Blasto Posted at: 2019-06-06T18:13:25.078Z Reads: 77

```
i need to confirm, pretty sure I do, the shop underwent a purge last week... unlikely those got tossed, but you never know
```

---
## \#17 Posted by: torqueboards Posted at: 2019-06-06T18:19:17.650Z Reads: 75

```
Blasto is the man. @seaborder
```

---
