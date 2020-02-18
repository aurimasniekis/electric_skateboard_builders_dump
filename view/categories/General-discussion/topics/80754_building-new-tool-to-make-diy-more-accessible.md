# Building new tool to make DIY More accessible

### Replies: 15 Views: 429

## \#1 Posted by: Anubis Posted at: 2019-01-13T15:05:13.546Z Reads: 150

```
Hey all,
So I am a huge advocate of DIY, and I want to have as many people building rather than buying prebuilt. We all know its better value, a fulfilling achievement and good fun, but a lot of folks are intimidated by it and I've been working on a small webapp that might help people to get into DIY for their first board.

This tool isn't necessarily directly targeted towards people already active on the forum but It should still be useful to everyone here, and I wanted to ask about what features I should go about implementing to improve upon what I'm going for already.

Here's what the tool looks like currently:
![image|690x450](upload://eDfn8M6PDxvPrdUBQ3U7lY9VD2z.jpeg) 

Currently, each option (Each deck, each truck, each mount) Needs data that looks like this:
![image|644x500](upload://dXYmw2dYzXBCJNWXM9XmKWldhY9.png) 
I was going to use a database, but as its entirely open source and could work as an offline app, the data for each component will just be directly stored.


The features I'm building into it are currently:
- Picking each component for your build in dual or single 
- Attempts to spot compatibility errors between parts
- Allows easy browsing through lots of available parts with filters, tags and sorting
- Gives links to each product selected
- Approximates price based on US Shipped Prices for each item

Complications:
- Detecting compatibility issues takes a long time. For example, choosing a certain truck will implicate which Mounts, motors and pulleys are possible, while a deck implicates the trucks, risers, battery and enclosure. Currently, the tool will not take into account things like diagonal/zigzag mounting and not allow dual 6374 on caliber II, because there is a transistive dependancy on their not being a split enclosure that comes with that etc etc. The tool will be for people who want to DIY easier. 
- Gathering data on the options. Getting 1 deck can take 15 minutes alone when I have to approximate the actual wheelbase space, width, gather data on ply, colours, and price. The same goes for a lot of the other things
- Skipping certain parts of the builder when certain component are selected. E.g gear drive means no pulleys or belts, and direct drive must skip mounts, pulleys, motor and belts all together.

What features should I add to make this tool even better? Here are my planned features:
- Adding in MTB components. They're not there right now because its just so much more data to gather
- API based price fetching on each item, although this is a difficult one to do and won't be added for some time. Most items don't change price much, except enertion and flipsky who both have a sale every 5 minutes.
- Exporting your build via a sharable link

I hope to have it online within the next couple days, when it is I'll need people to try and break it to find bugs :slight_smile:
```

---
## \#2 Posted by: Indiangummy Posted at: 2019-01-13T15:17:41.277Z Reads: 128

```
So a pc part picker but for esk8s?
```

---
## \#3 Posted by: Anubis Posted at: 2019-01-13T15:18:41.438Z Reads: 130

```
Yea that's what I was going for, its going to be much harder to build in compatibility stuff though
```

---
## \#4 Posted by: ZachTetra Posted at: 2019-01-13T15:18:45.669Z Reads: 124

```
This is super cool...I like what you're trying to do!
```

---
## \#5 Posted by: sami Posted at: 2019-01-13T15:20:30.685Z Reads: 125

```
Suggestions for belt length might be a good idea especially if you are new to this hobby but it might be hard to implement
```

---
## \#6 Posted by: Indiangummy Posted at: 2019-01-13T15:21:08.227Z Reads: 120

```
Yeah that's going to be hard unless you limit it to only certain decks.
```

---
## \#7 Posted by: Anubis Posted at: 2019-01-13T15:28:45.524Z Reads: 112

```
I don't think thats realistically possible, because any pulley + any mount = like thousands of possible belt lengths, and then you also need to take into account if they're using idlers or not etc etc. I kind of intend for someone to make a partlist and juggle around the prices of stuff, then come here and work out the few small details
```

---
## \#8 Posted by: Anubis Posted at: 2019-01-13T15:30:17.989Z Reads: 102

```
The deck options should be unlimited, but I do need to know things like clearance, width and actual wheelbase for each one. Then I can figure out if something *should* be compatible. Its not something you should use to actually order all your parts with, just get a good idea of the price of what you're building/get ideas as to what can be on your build
```

---
## \#9 Posted by: Anubis Posted at: 2019-01-16T16:57:04.635Z Reads: 70

```
Added up to the wheels so far! I keep finding more complexity in everything I have to add. This project will be open source if anyone wants to read through the code.

![image|690x450](upload://eDfn8M6PDxvPrdUBQ3U7lY9VD2z.jpeg)
```

---
## \#10 Posted by: mmaner Posted at: 2019-01-16T17:00:16.776Z Reads: 68

```
FYI, this has already been done by one of the most experienced builders on the forum, in the world actually...

https://www.electric-skateboard.builders/t/what-if-you-could-just-go-to-a-site-and-build-your-next-electric-skateboard/21768
```

---
## \#11 Posted by: longhairedboy Posted at: 2019-01-16T17:06:05.812Z Reads: 64

```
yeah, and people just kept ordering the same thing.... so i stopped using it and started asking what they wanted different on theirs.
```

---
## \#12 Posted by: Anubis Posted at: 2019-01-16T17:07:46.111Z Reads: 62

```
But how limited were the parts that could be chosen? Its not easy to develop with compatibility detection and allow for a ton of parts to be used interchangeably. 

I wish I could have seen his system
```

---
## \#13 Posted by: Anubis Posted at: 2019-01-16T17:08:23.365Z Reads: 58

```
Well I mean this won't be commercial its just for people who want to make a DIY but don't know where to start to look at. How restricted were the options on your builder?
```

---
## \#14 Posted by: longhairedboy Posted at: 2019-01-16T17:13:04.726Z Reads: 58

```
it was extensible and the parts list was constantly updated based on availability and compatibility. 

The real monster in a sytstem like this is compatibility mapping. With every choice you have to check all of the other choices and either make a decision or prompt the user for a decision in order to resolve conflicts. 

Ultimately i found it easier to remove some choices from the user, but that only applied to my use case. Your use case seems like it should cover every option available.
```

---
## \#15 Posted by: Anubis Posted at: 2019-01-16T17:19:26.861Z Reads: 56

```
Yea, its really difficult to think of compatibility issues. For example, when the user is shown what trucks they can have, as this includes options for Hub motors etc, this places limitations on the type of ESC, as well as changes the fact that they never choose motors, pulleys, or wheels. 

You can kind of guess how I'm doing it currently based on the data in the original thread, but I hope to have a tool that allows people to get a general idea of how much a "Dual motor hub board with x range and y top speed could cost compared to the prebuilt I was going to buy".

 Also I *assume* your tool was limited in some respects to components you made yourself, e.g could you order a board with a landyachtz deck, boa wheels, torque boards trucks and boardnamics mounts. It would be near impossible to make a system that detects price changes and availability for all of those, because a lot of them are made by companies/people not searchable on any marketplace.

It kind of defeats the purpose of a builder if the options for 6x2 pnumatics are limited to just ones 1 vendor sells. I'm hoping to aggregate all parts that are at least of decent quality into 1 builder
```

---
