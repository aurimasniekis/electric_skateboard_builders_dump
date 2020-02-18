# What are the real details of the VESC 6?

### Replies: 29 Views: 1986

## \#1 Posted by: SkateYS Posted at: 2018-06-03T20:05:00.399Z Reads: 318

```
Hi everyone! I have been searching through Trampa web site for more info about the VESC 6. They just mentioned every detail except the ones I'm looking for! What is the Hardware version and what is the firmware version!?
```

---
## \#2 Posted by: linsus Posted at: 2018-06-03T20:08:19.050Z Reads: 320

```
Firmware is updated every month or so via vesctool. Not sure what verision comes on it but you'll update it when pluggin in either way. Hw is 6.4
```

---
## \#3 Posted by: SkateYS Posted at: 2018-06-03T20:09:41.994Z Reads: 309

```
cool! thanks for the info!
```

---
## \#4 Posted by: b264 Posted at: 2018-06-03T20:22:37.542Z Reads: 290

```
[Hardware](https://github.com/b264/bldc-hardware/blob/master/VESC_6.pdf)

[Software](https://github.com/vedderb/bldc)

Also since it's GPL, you can ask the manufacturer (@trampa) and they will provide this information per law
```

---
## \#5 Posted by: trampa Posted at: 2018-06-04T04:58:05.594Z Reads: 253

```
HW6.41, 
FW3.38

We try to always flash the lates FW.
And you don't loose your warranty when updating your device to the latest Vedder FW.
```

---
## \#6 Posted by: trampa Posted at: 2018-06-04T07:38:29.144Z Reads: 227

```
We want our users to always run the latest FW, so it might be that Benjamin made an update while our VESCs sit on the shelf waiting to be sold. VESC-Tool will tell you that the FW is outdated, when that is the case. In that case you need to do an update of the FW through VESC-Tool. The FW will then be up to date, resembling the files you find on Benjamin's GitHub. 

HW revsion: Some vendors decided to call their HW e.g. rev.6.6. That doesn't mean it more up to date. It's probably totally different Hardware.
It is like with Cars. An Audi A6 is not more up to date than a BMW 3.25.
We use our own revision number system. So should others. I know it can be confusing for the customer.

Frank
```

---
## \#7 Posted by: Minim Posted at: 2018-06-04T08:57:37.331Z Reads: 208

```
And some «decided» to not use the VESC name at all Even if its the same thing just to make the confusion complete.

You can go and buy a ESCApe vesc6.4 here on this forum for a major discount and it’s basically the same stuff as the high priced trampa stuff. They only trademarked the vesc name to squeeze dollars from us and tramp is going after everyone that tries to make vesc with the TM bullshit. You will see it in the reply to this post also (coming soon from tramp) that there will be a response on how good TM is for everyone but in reality it’s just to increase confusion and hope that more people buy vesc6.4 from trampa instead of other identical suppliers.
```

---
## \#8 Posted by: trampa Posted at: 2018-06-04T11:45:17.521Z Reads: 189

```
And everyone calling different products and qualities the same helps customers a lot to differentiate between all the products available in the market now and in future LOL. Poor customer!

The ESCApe is definitely not of the same quality. 
- Different supplier
- Different manufacturer and assembly line. How consistent and precise do they work?
- Is the PCB wired up exactly the same? Trace lengths, positions of parts towards another etc.
- Quality Inspections and testing?
- Same components used?
- Internal silicone parts missing that are essential for a long product life and best thermal conductivity.
- gets hotter faster, can't push as many Amps.
- external silicone sleeve missing
- Warranties? 
- same service offered?
- same product availability guaranteed, or is it a pre-order product with months of patience involved?
- same VESC-project support, invest into future Innovations and R&D?

Sorry @Minim, its not the same and should have its own name, so that customers can differentiate. 
And it the device fails, it doesn't affect our reputation. It affects the manufacturers reputation in that case.
I can see a lot of design flaws already and I know what the outcome will be with regards to reliability.  

When I want to buy a Canon Camera, I want it to be made by Canon and not someone else who thinks he can make Canons, not using the same material and precision and not performing same quality inspections and not offering the same service. And Canon will therefore make sure that they are the only ones using their TM. Brands stand for a certain quality and people trust brands to deliver a certain standard.
```

---
## \#9 Posted by: Jc06505n Posted at: 2018-06-04T12:03:22.468Z Reads: 178

```
So I’m not an ESC expert by any means but..

[quote="trampa, post:8, topic:57701"]
Different supplier
[/quote]

Different doesn’t mean worse nor better , it just means different. Having a different supplier is not a valid argument in the terms of whether or not something Is of the same quality. 


[quote="trampa, post:8, topic:57701"]
Different manufacturer and assembly line
[/quote]

Same point as the point above

[quote="trampa, post:8, topic:57701"]
How consistent and precise do they work?
[/quote]

That’s a valid point/question, the other two above are not. The next few points you list are valid. 

[quote="trampa, post:8, topic:57701"]
Warranties
[/quote]

Doesn’t make a product cost $200 more. We’ll also disregard the fact that Trampa offers a 6 month warranty instead of the Legally mandated 2. Whatever. 

The next few points are valid. 



[quote="trampa, post:8, topic:57701"]
same VESC-project support, invest into future Innovations and R&D?
[/quote]

Since the VESC project is opened source, any updates you push out also benefits Escape , as well as any other software like Ackmaniac. Unless you were to push out an update that would only work for the Trampa VESC6, which you would still have to provide and would be noticed. But I doubt you would do that. The main point is: the ESCape goes wherever the community goes. And if it can do the bare minimum that your VESC6 can do without the $200+ price tag , then your VESC6 is essentially dead to future sales from this community. 

[quote="trampa, post:8, topic:57701"]
Sorry @Minim, its not the same and should have its own name, so that customers can differentiate.
[/quote]

I agree with this, don’t like how you go about it, but I agree. 

[quote="trampa, post:8, topic:57701"]
I can see a lot of design flaws already and I know what the outcome will be with regards to reliability.
[/quote]

Then it’s a good thing that we have an entire community willing to test the shit out do this thing until it’s perfect. Here’s the thing frank , even if this fails 100 times , there’s no way his community is going to retreat back to that $300 price tag. We’ll contribute as much as we can to ensure that @stewii makes a VESC6 killer product.
```

---
## \#10 Posted by: trampa Posted at: 2018-06-04T12:37:04.897Z Reads: 164

```
It's not 200 more! Some vendors here advertise their products without taxes to make things look cheaper.
If you buy a VESC 6 together with one of our board you pay a lot less! 
The price depends on where you live and how high taxation is. 

If a ESCape is 185 GBP with housing, that is for a European customer 222 Pound including the applicable British VAT of 20%. That is more than our customers pay when they buy a board from us with VESC 6 included.
```

---
## \#11 Posted by: Cobber Posted at: 2018-06-04T13:43:29.773Z Reads: 155

```
I have bought a deck from you Frank, I missed this VESC 6 deal that is cheaper than a ESCape...
Rebate?
```

---
## \#12 Posted by: hexakopter Posted at: 2018-06-04T13:52:34.991Z Reads: 146

```
I think Frank is talking about their complete boards where the VESC 6 is included. Not their single decks.
```

---
## \#13 Posted by: Cobber Posted at: 2018-06-04T13:55:19.482Z Reads: 147

```
Rebate?...
```

---
## \#14 Posted by: trampa Posted at: 2018-06-04T14:41:55.923Z Reads: 147

```
Completes...
```

---
## \#15 Posted by: FredrikHems Posted at: 2018-06-04T14:46:24.278Z Reads: 148

```
Not many on this forum buy trampa’s completes though..
```

---
## \#16 Posted by: bevilacqua Posted at: 2018-06-04T14:59:44.033Z Reads: 152

```
**DIY** :) 
10char
```

---
## \#17 Posted by: trampa Posted at: 2018-06-04T15:14:43.506Z Reads: 172

```
That's your guess.
```

---
## \#18 Posted by: Jc06505n Posted at: 2018-06-04T15:50:15.280Z Reads: 179

```
[quote="trampa, post:10, topic:57701"]
It’s not 200 more!
[/quote]

My Fault, $100 was an exaggeration, it's closer to $100-$50. But understand that $50 is a major difference when buying a ESC as that's the difference between a Focbox and a Maytech. See how many people opt over saving 50. Now how this applies to a $100-$50 difference.

[quote="trampa, post:10, topic:57701"]
If you buy a VESC 6 together with one of our board you pay a lot less!
[/quote]

Frank, please excuse my French here, but *who the fuck*, on a *builders* forum is buying a complete tampa complete to save some bucks on a VESC? Deck? Maybe, Trucks? Sure Complete Drivetrain? Even I considered it. That's like buying a Banshee or an Arcboard for the goddanm ESCs they use!

Lets be real Frank, there's no saving at all. It's like walking into a shop for one thing and walking out with a whole shopping cart of shit cause of the "sales". You don't save shit, you just end up spending more.

[quote="trampa, post:10, topic:57701"]
If a ESCape is 185 GBP
[/quote]

The latest Price i can find is:

[quote="stewii, post:1, topic:49720"]
£113-120
[/quote]

[quote="trampa, post:10, topic:57701"]
with housing
[/quote]

The Latest Pricing Details i can find is: 

[quote="stewii, post:1, topic:49720"]
Dual will look like this:  (note: dual might have an increased value of £10 per housing.)
[/quote]

but @LukePL & @stewii should be able to clarify.

But that's a max of **£130 without VAX**, or **£156 with VAX** , which is **€179.93 or $172.99** (The US don't get charged VAT from what I've seen, please correct me if I'm wrong in that regard). 

**That's a €150.07 difference(€330 - €179.93) a $177.01 difference ($350 - 172.99).** 

@stewii @trampa @LukePL Any corrections I gotta make?
```

---
## \#19 Posted by: LukePL Posted at: 2018-06-04T16:43:39.355Z Reads: 158

```
As for complete ESCape it is up to @stewii I'm just a guy that makes enclosure the best price I can. Your calculations are correct and I have no idea from where this 185GBP Frank got. Thing is that I believe that Trampa cost of producing VESC 6 is higher than stewii's ESCape but does it mean that we have to pay for that? @onloop has managed to make great controller for good price so it's can be done by a company. 
This discussion is kind of pointless as we will never know the cost structure and Trampa sales policy regarding Vesc 6 and even more pointless when after all what happen it seems that they are not willing to change that. 

Hey @trampa maybe I can make you an enclosure that is much cheaper that what you currently have :D ?
```

---
## \#20 Posted by: FredrikHems Posted at: 2018-06-04T17:38:22.542Z Reads: 151

```
![image|220x147](upload://bB2dOdSaE6NvY491wW6G4ruJ3te.gif)
```

---
## \#21 Posted by: thepiano Posted at: 2018-06-05T07:21:07.403Z Reads: 139

```
You are assumming that new people joining this forum are similar to the existing ones. 

I see nothing wrong buying trampa's complete, it's high quality and support at a cost. I also see nothing wrong with DYI-ing your way around and milking every $. To each its own. Maybe you're in your 20's and have time and no money, maybe you're 45 and it's the other way around. 

Trampa will always have a sales pitch. Good for them I say, whatever it takes to make quality shit available and iterate until it gets better. Market and time will tell. But seems to me people are having an issue with the idea of it, not the end game.
```

---
## \#22 Posted by: FredrikHems Posted at: 2018-06-05T11:08:57.460Z Reads: 135

```
We all know that newcomers arent the ones that spend the most on their first build too, compared to the ones that have been in the game for several years. Trampas are expenisve either way.

[quote="thepiano, post:21, topic:57701"]
milking every $
[/quote]
I guess you can build a less expensive emtb if you want to, but the majority of diy emtb`s here cost more than a pre-built trampa. In many cases- way more.
```

---
## \#23 Posted by: Jc06505n Posted at: 2018-06-05T12:03:07.610Z Reads: 137

```
[quote="thepiano, post:21, topic:57701"]
I see nothing wrong buying trampa’s complete
[/quote]

There’s nothing wrong with it, but buying a Trampa complete just to save in a VESC? Lol no 

[quote="thepiano, post:21, topic:57701"]
I see nothing wrong buying trampa’s complete
[/quote]

No one saying it’s wrong , no one cares about a Trampa complete. But saying buying one *saves* you money on a builders forum ? Fuck out of here, and this is coming from the guy willing to spend endless amount of money just so he doesn’t have to solder a single joint on a build. 

[quote="thepiano, post:21, topic:57701"]
Trampa will always have a sales pitch. Good for them I say, whatever it takes to make quality shit available and iterate until it gets better. Market and time will tell. But seems to me people are having an issue with the idea of it, not the end game.
[/quote]

Trampa sales pitch and how they go about is another matter for another time, but ain’t no way they’re going to come on here and have the audacity to say that ESCape is going to cost more with their own overpriced esc *by buying a complete Drive Train*.
```

---
## \#24 Posted by: trampa Posted at: 2018-06-05T12:51:06.583Z Reads: 124

```
1300 for a unbreakable custom spec board with VESC 6 and deck integrated cables and Carbon Monster Box for 1Kwh of LiPo Battery incl. Remote and Bluetooth module, LCD Battery indicator, bindings and all cables and connectors is not expensive. We are actually offering to cheap.

![Trampa_Monster%20BOX%20V2_electric%20skateboard_battery%20box|690x308](upload://rU0Xe1nYK8S4h5leUEViW90HKgU.jpg)

Frank
```

---
## \#25 Posted by: FredrikHems Posted at: 2018-06-05T13:14:40.567Z Reads: 121

```
But you’ll have to buy a $300-700 battery too. Also I guess the 1300 is In pounds?
```

---
## \#26 Posted by: trampa Posted at: 2018-06-05T14:03:48.980Z Reads: 119

```
You have to buy the battery you want. If you are DIY, you can make a nice pack yourself. 
Sure Pound, we are a British company. Still a deal and a lot better in value than all other commercial boards out there. Quality to the buck is still unmatched.
Trampa stocks all the stuff, we are no cash upfront and deliver 6 months later company.
All of our boards are custom made to spec and usually delivered within 4-5 days after purchase.
Just had a customer from California, who could not believe that the postman knocked on his door on Friday. He ordered on Tuesday.  Someone has to build the board and this guy gets a salary. 

I sometimes have the feeling that people compare apples to oranges. You can't compare the prices a no profit group buy to prices that companies offer. Running a company is expensive. There is more involved than the price of the raw materials. Staff, pensions, health insurance, rent for warehouse, tools and machines, electricity and heating, truck and trailer, travel expenses, website, sourcing, product design, taxes and warranties and product returns and financing costs, and computers and furniture and and and. This all needs to be priced in. Otherwise you don't make profits and if that is the case, you don't have a business for long. 

Most small companies like us struggle these days to survive. The mid class society is shrinking rapidly, with all the bad consequences for our society. The more people struggle, the more they are willing buy from big, cheap mass market sources to compensate low incomes and the more pressure there will be on society in general. Companies like us are the ones offering the jobs everyone wants and they are the ones paying the taxes. If you want everything for cheap, you should not complain if you don't find a job. Economy is sending money in circles.
```

---
## \#27 Posted by: Ackmaniac Posted at: 2018-06-05T17:40:45.779Z Reads: 107

```
Motor mounts, Motors? Can't really see the offer where i only need to add batteries. These seem to start at 1700 pounds or 1900 pounds.
```

---
## \#28 Posted by: trampa Posted at: 2018-06-05T18:34:00.431Z Reads: 106

```
http://www.trampaboards.com/single-motor-urban-electric-mountainboard-on-electric-deck-with-vertigo-trucks--8-inch-superstar-wheels-ratchet-bindings-monster-box-vesc-p-24729.html
```

---
## \#29 Posted by: Ackmaniac Posted at: 2018-06-05T18:38:31.115Z Reads: 104

```
Ok my fault. So this is a single drive and the once i have seen are dual drive.
```

---
