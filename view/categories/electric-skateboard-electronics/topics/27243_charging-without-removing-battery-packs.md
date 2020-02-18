# Charging without removing battery packs

### Replies: 23 Views: 1778

## \#1 Posted by: florensvb Posted at: 2017-07-10T12:42:13.715Z Reads: 160

```
Hey guys,

I am about to build my first electric longboard for which I have order 2 x 4S 8000mAh batteries, as well as an SKYRC e8 100w LiPo balance charger.

My question is how can I achieve to charge the batteries without taking them out every time. I already looked at the BMS solution and decided that it's not the way to go for me, since I already have a Balance charger. Basically I need to expose the lead wires as well as  the balance ports, right? But if I do that, how can I switch between ON Mode and CHARGING mode without physically re-plugging the cables every time? 

Thanks for the help!
```

---
## \#2 Posted by: cricrithezar Posted at: 2017-07-10T12:58:15.298Z Reads: 153

```
If they're in series, you need an 8s charger or BMS,. If you want to charge them as 4s you need to disconnect them or you'll short things somewhere. Can explain when I'm not in class.
```

---
## \#3 Posted by: TarzanHBK Posted at: 2017-07-10T13:04:02.527Z Reads: 148

```
http://www.electric-skateboard.builders/t/miami-electric-boards-diy-charger-how-to/4242
```

---
## \#4 Posted by: scrapheap Posted at: 2017-07-10T13:08:32.233Z Reads: 140

```
[http://www.electric-skateboard.builders/t/how-to-charge-12s-with-imax-b6/24660](http://www.electric-skateboard.builders/t/how-to-charge-12s-with-imax-b6/24660)
```

---
## \#5 Posted by: florensvb Posted at: 2017-07-10T13:29:18.508Z Reads: 134

```
Yes they are in series. [This is the charger i intend to use](https://www.tomtop.com/charger-adaptor-1226/p-rm3758eu.html?_ga=2.266025295.1375015153.1499633257-1299444626.1499432448)
```

---
## \#6 Posted by: cricrithezar Posted at: 2017-07-10T14:22:41.017Z Reads: 129

```
Then you can treat your 4s packs the same as an 8s pack, just know that you'll have a redundant balance lead where your packs are connected. If you need schematics you can probably find some around here (or Ivan draw some later)
```

---
## \#7 Posted by: florensvb Posted at: 2017-07-10T15:26:29.203Z Reads: 117

```
Yes thats what i am intending to do: put the two 4s in series so it gives me an 8s pack. 
so youre saying that i can only connect the 4s balance lead from one of the two packs and leave the other disconnected? dont i have to somehow make the 2 4s balance leads into one 8s lead, either by buying an adapter or a balance board?
```

---
## \#8 Posted by: cricrithezar Posted at: 2017-07-10T16:28:47.828Z Reads: 109

```
I guess I didn't explain correctly, you need both leads, but one of the wires is redundant. You need 5 wires for 4s, and 9 wires for 8s. So you'll have one redundant wire if you combine your two 4s Balance leads. I can send you a schematic if you want
```

---
## \#9 Posted by: florensvb Posted at: 2017-07-10T16:29:49.855Z Reads: 107

```
Yeah thatd be so nice! thanks a bunch
```

---
## \#10 Posted by: florensvb Posted at: 2017-07-10T16:30:58.414Z Reads: 110

```
Also in order to combine the two balance leads into one 9-pin balance lead- do i need to buy some 9pin plug or can i somehow combine the two without buying something else?
```

---
## \#11 Posted by: cricrithezar Posted at: 2017-07-10T16:55:03.591Z Reads: 103

```
Here's a quick paint.net drawing.
<img src="/uploads/db1493/original/3X/2/e/2e8e7870aff7b04ec64e14f5029346a10a8f12e8.png" width="666" height="500">
You might not want to connect all 10 wires coming out but only 9 (leave out one of the redundant ones, less risk of shorting your balance leads, though I don't know how a balance charger would handle funky voltages, just try and not mess up). You probably want to keep the connectors on your battery, just create a series adapter, you might even be able to find one online (something like [this](https://www.alibaba.com/product-detail/2-x-4s-to-8s-Splitter_60083961379.html)) Also don't ever put the wrong balance lead in the wrong connector if you do that, you'll short the entire battery through that small wire which is definitely not good.
Feel free to ask any questions, it's best to be well informed when it comes to batteries because they can be scary things.
```

---
## \#12 Posted by: Okami Posted at: 2017-07-10T17:43:08.929Z Reads: 92

```
[quote="florensvb, post:1, topic:27243"]
But if I do that, how can I switch between ON Mode and CHARGING mode without physically re-plugging the cables every time?
[/quote]

You can make a switch for this or just make the port not 'visible' to the outside (by inserting a cap or a plug, for example!)

A good solution is the one @TarzanHBK referenced to:

By getting VGA port, you can sort of make a one cable solution - you would just plug in this one cable and would not need to mess with balance cables and main cables.. 

Though, you need to check whenever 8s is possible at higher currents, as each pin has a current limit I think it can withstand, so sometimes 4pins might be needed just for power alone.
```

---
## \#13 Posted by: florensvb Posted at: 2017-07-11T09:29:38.522Z Reads: 85

```
@cricrithezar thank you so much for taking the time to explain this. I think i feel comfortable now to make my own 8s battery pack in series :) 

I never need the balance leads until I wanna charge it, right? The ESC does not need them? 

But what the ESC and the Charger both need are the + and - leads, correct?

So the next question is how I can build a good setup for achieving that. I am gonna re-watch the videos you guys posted earlier. I think one guy was using a parallel XT90 connector for this purpose..
```

---
## \#14 Posted by: florensvb Posted at: 2017-07-11T09:35:45.626Z Reads: 87

```
[quote="Okami, post:12, topic:27243"]
You can make a switch for this or just make the port not 'visible' to the outside (by inserting a cap or a plug, for example!)

A good solution is the one @TarzanHBK referenced to:

By getting VGA port, you can sort of make a one cable solution - you would just plug in this one cable and would not need to mess with balance cables and main cables.. 

Though, you need to check whenever 8s is possible at higher currents, as each pin has a current limit I think it can withstand, so sometimes 4pins might be needed just for power alone.
[/quote]

I think this is what I am gonna go do actually. A VGA port sounds like an elegant solution. 

You said that I might need more of the pins because I am using 8s. @TarzanHBK said that the port has 15 pins. My battery balance leads would have 9 pins, leaving me with 6. So I could use 3 for - and 3 for +. That should definitely be enough, no? My charger can charge up to 6A, although I think i'll select the lower options, so that my batteries last longer.
```

---
## \#15 Posted by: Okami Posted at: 2017-07-11T09:40:14.245Z Reads: 77

```
yeh 15pins should be way enough :slight_smile:

More problems would be, if you wanted to run 10s/12s and then charge at something like 8amps probably.

So you, with 8s, should have plenty of current ability, I think for 6amps even 2 pins for + or - would be enough.

--

And yes, both esc and charger needs +/- leads, + charger will need also balanace cables which you gonna incorporate into the vga cable/port.

You basically need 2 +/- leads, you can do this by getting a parallel cable for your existing battery connection and then installing a switch on one of the charge cables for example.

One other solution I have seen is, xt90 connector, like you mentioned but then you need to search a bit around to find how exactly to install it.
```

---
## \#16 Posted by: florensvb Posted at: 2017-07-11T09:42:28.159Z Reads: 70

```
[quote="TarzanHBK, post:3, topic:27243"]
Split the battery cable into 2 pins (2 for Red and 2 for Black) 4 Total. This will allow you to charge up too 6amps.
[/quote]

Just because I am a noob at soldering: Do I literally split the fibers inside the cable in two, or do you somewhat put the whole cable in between the two pins and use a lot of solder to combine it? :D
```

---
## \#17 Posted by: florensvb Posted at: 2017-07-11T10:00:03.306Z Reads: 76

```
[quote="scrapheap, post:4, topic:27243"]
I made this video on how to one plug charge 6S and 12S (two plug) with cheap and readily available b6 chargers. the question comes up often enough..  with one (or 2) simple to make charging lead you can easily charge your batteries without removing them from the board. 
[/quote]

Looks like you simply soldered the charging leads from the balance charger to the + and - of the balance leads? I thought the balance leads aren't quite capable of handling all that voltage? That also seems like an easy solution. So you just have the balance lead plug and that's it? :D
```

---
## \#18 Posted by: Okami Posted at: 2017-07-11T10:05:43.413Z Reads: 75

```
A while ago, I had such cable:

https://hobbyking.com/en_us/twin-pack-charge-lead-2-x-3s-6s-w-xt60.html

It looks it makes it possible to charge through only balance leads, as it makes an xt60 connection from the balance leads.

I suspect it is enough for low amperage, something like 4amps probably is fine, though Im not sure does it matter related to amps per one cable on how you charge (balance mode or charge mode)
```

---
## \#19 Posted by: TarzanHBK Posted at: 2017-07-11T12:42:58.555Z Reads: 70

```
You can split the cable in two - one for each pin, or solder 2 smaller cables on the pins and solder them to the bigger battery cable.
```

---
## \#20 Posted by: TarzanHBK Posted at: 2017-07-11T12:46:08.644Z Reads: 67

```
This charger is capable of 100W max, so you won´t reach 6amps on 8s:
100W : 8S : 3,7V = 3,38A max.
So your two cables are enough (although you could wire 3 cables each for pos and neg to charge on a higher rate with a more powerfull charger later on)
```

---
## \#21 Posted by: florensvb Posted at: 2017-07-11T12:48:34.706Z Reads: 62

```
Ok combining all these amazing answers, I think this is what I will do:

First I will need to combine my 2 3S Packs in series by either buying a harness or simply soldering them together correctly.

Then I'll use the VGA port as an one plug solution by soldering it to the + and - leads from the balance plug, as it can be used for charging as well, like @Okami suggested. 

That should work as a good solution, right?

Thanks so much guys
```

---
## \#22 Posted by: scrapheap Posted at: 2017-07-11T13:23:29.907Z Reads: 57

```
You have to ask @lowGuido, it's his video.  Maybe he can chime in with his input on this, because I have no idea.
```

---
## \#23 Posted by: lowGuido Posted at: 2017-07-11T23:57:11.494Z Reads: 57

```
[quote="florensvb, post:17, topic:27243"]
Looks like you simply soldered the charging leads from the balance charger to the + and - of the balance leads? I thought the balance leads aren't quite capable of handling all that voltage? That also seems like an easy solution. So you just have the balance lead plug and that's it? :smiley:
[/quote]

yes thats exactly what I did. no need to worry about the balance leads, they are rated much higher than the B6 can put out. I think from memory the balance leads are 22AWG which is about 7A max and the B6 can only put out 5A max which in practice is 2.4A max @ 6S.  TLDR: don't worry about it.
```

---
