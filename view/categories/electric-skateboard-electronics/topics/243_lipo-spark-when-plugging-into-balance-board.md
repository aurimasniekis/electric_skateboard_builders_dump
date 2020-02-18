# Lipo spark when plugging into balance board

### Replies: 33 Views: 7015

## \#1 Posted by: siggs3000 Posted at: 2015-09-27T01:21:45.363Z Reads: 258

```
Well this scared the beejezus out of me. I have an 8s lipo that has two 4s balance connectors to supposedly make charging easier. So I ordered a balance board with two 4s ports (and an 8s wore to the charger. 

Excited that it finally came, I plugged the first 4s wire from my 8s pack into the board and it was a non issue. Then I started to plug the second 4s connector into the board and a pretty damn big spark and a bit of smoke followed. It happened on first contact and I immediately pulled them appart. (Tiny fraction of a second of contact. But it was enough to blacken the plastic on the balance wire and the balance board.

My questions are:

1. Wtf was that about? Is that normal? I was certain that's it was not plugged in backwards. And these batteries have never been used before. They are brand new.

2. Do you think I fried anything beyond repair? 

Pics attached. <img src="/uploads/db1493/original/1X/2a9f9969789b9cbfebf1f30e1eead60b64c2bf03.jpg" width="375" height="500">
```

---
## \#2 Posted by: siggs3000 Posted at: 2015-09-27T01:22:30.400Z Reads: 255

```
<img src="/uploads/db1493/original/1X/00fc01e1f16b1e96bc89bdd9f65f7b440ee57392.jpg" width="375" height="500"> <img src="/uploads/db1493/original/1X/2712d32a7025d272f3f1d703c9aaa6827e2f4c49.jpg" width="375" height="500">
```

---
## \#3 Posted by: psychotiller Posted at: 2015-09-27T01:27:38.849Z Reads: 249

```
So, this is what happened. The battery is wired in series @ 8s. And you tried to balance charge at 4s parallel. Unfortunately, I don't think that's possible.
```

---
## \#4 Posted by: siggs3000 Posted at: 2015-09-27T01:29:14.221Z Reads: 251

```
Interesting... With two 4s balance plugs on the one 8s battery, how do you charge this thing?
```

---
## \#5 Posted by: psychotiller Posted at: 2015-09-27T01:38:04.264Z Reads: 247

```
If you wanted to balance it at 4s it would need to be taken apart and charged as two 4s batteries. 
 The only other way is if you have an 8s charger.
```

---
## \#6 Posted by: siggs3000 Posted at: 2015-09-27T01:41:15.369Z Reads: 241

```
Thanks man. I do have an 8s charger but this battery doesn't have an 8s balance plug... Just the two 4s ones. I'm just a little confused about what type of adapter I would need to connect it to the charger. (My first lipo)
```

---
## \#7 Posted by: psychotiller Posted at: 2015-09-27T01:43:57.009Z Reads: 224

```
Hmmm...someone else chime in here. Could he cut the one red wire on the negative side balance to pull this off?
```

---
## \#8 Posted by: siggs3000 Posted at: 2015-09-27T01:53:01.442Z Reads: 211

```
I found the store listing for this board and it says it's actually made for packs that are wired in series: http://www.hobbyking.com/hobbyking/store/__51405__XH_Multi_Pack_Balance_Board_2_8S.html So I think that should actually be the right thing. Just not sure why there was such a big spark.
```

---
## \#9 Posted by: psychotiller Posted at: 2015-09-27T02:00:02.144Z Reads: 205

```
It shouldn't have sparked or melted the connection. Somethings crooked in Straightesville.
```

---
## \#10 Posted by: siggs3000 Posted at: 2015-09-27T02:01:41.718Z Reads: 207

```
That's what I was afraid of... The only place I could find one of these little boards was from a shop in India! I searched everywhere else in the world for one that allowed for this kind of use for an 8s pack.
```

---
## \#11 Posted by: psychotiller Posted at: 2015-09-27T02:09:40.381Z Reads: 192

```
You should order an 8s jst plug and wire it up 8s.  Make sure the balance lead that sparked isn't melted or needed. It might be the red lead that shouldn't be used.
```

---
## \#12 Posted by: siggs3000 Posted at: 2015-09-27T02:12:51.769Z Reads: 191

```
It was actually the ground wire. 

That's a good idea. I think I should just cut the two 4s plugs off and go with one 8s. That should be an interesting project for a newb though!
```

---
## \#13 Posted by: lowGuido Posted at: 2015-09-27T02:21:05.753Z Reads: 191

```
Did you see my diagram in the cable porn thread? Its for 6s but the theory remains the same for 8s. You need to cut the black wire off the balance lead of the positive pack.  Not doing so or doing so incorrectly can actually blow your charger.
http://www.electric-skateboard.builders/t/cable-porn-ohhhhh-yeahhhh/198/16
```

---
## \#14 Posted by: psychotiller Posted at: 2015-09-27T02:21:58.945Z Reads: 184

```
There you go! Thanks @lowGuido
```

---
## \#15 Posted by: lowGuido Posted at: 2015-09-27T10:49:32.667Z Reads: 185

```
ok so now that I'm out of bed, I'll get a bit more detailed for you.
here is how it works. ... pictures say 1000 words so..
<img src="/uploads/db1493/original/1X/68bfd8e740b4af1090c00587d5efd40f02fa32cd.PNG" width="512" height="500"> 

Left is what you have. Right is what you need.

the important thing to realize here is that the black wire on the left most pack is actually the same as the red wire on the right most pack. which is also the same as the thick red wire in the middle.
so by connecting the small balance lead to that board (I can't see how that board is wired I can only assume logic) if you have your left one and your right one mixed up, the black wire is basically just shorting straight across the positive and negative of one of your series batteries.
make sense? 

in saying that if you were to plug you 2 balance leads into the **opposite** ports, that board you have will still work assuming its not itself fried.

edit: in fact now that I have had time to look at your images in detail I can clearly see that you have plugged the negative balance lead into the positive side of the board. The damage doesn't look too bad so you can probably still use that board. just make sure you connect the leads the correct way. (why would they even sell something so confusing)

TLDR: guessing which balance lead is the more positive and most negative is annoying and potentially dangerous. best solution is the right side of my diagram above with one 8S balance lead.
```

---
## \#16 Posted by: lowGuido Posted at: 2015-09-27T11:16:32.960Z Reads: 174

```
im trying to make this as easy to understand as possible.. sorry if I'm waffling on..
so heres where you went wrong. (again I still don't understand why they sell a product that's so easy to confuse)

<img src="/uploads/db1493/original/1X/24bb47c45c88ed79d6a26211a142451228600456.jpg" width="375" height="500"> 
<img src="/uploads/db1493/original/1X/69d5efc250c7946d4460f7014ba64e232f95cbb9.jpg" width="375" height="500">
```

---
## \#17 Posted by: siggs3000 Posted at: 2015-09-28T01:12:29.154Z Reads: 167

```
Thanks @lowGuido! Amazing detail and amazingly helpful. Last night I also contacted HobbyKing since this is the board that they actually recommended I get for this weirdo battery. They recommended that I cut off the two 4s connectors from the 8s battery and wire up a single 8s connector. I can't imagine why in the world it wouldn't come that way but I instead just initiated a refund process and I'm just going to simplify my life and get a different set of batteries with normal charging leads. That being said, your diagram still comes in handy for wiring the new batteries up together to balance charge down the road. 

Thanks again!
```

---
## \#18 Posted by: Paul Posted at: 2015-12-16T07:50:41.971Z Reads: 160

```
I also connected my balance cables in series and had a massive spark. My batteries were connected in series. Did you have your batties connect in series?

I then speedster the batteries and connected them in series which much more caution and I didn't get a spark. I then connected the batteries in series and had no spark. 

I have not tested this while charging or using a BMS. However I am sure it's just the process that the barriers must be separate at first then connect the balance cables and then connect the batteries in series. 

Anyone else had a similar experience?
```

---
## \#19 Posted by: siggs3000 Posted at: 2015-12-16T08:09:02.895Z Reads: 154

```
As it turned out, I had the wrong balance board for what I was trying to do and since went a different direction with different batteries. I was attempting to connect them in parallel at the time though. Lipo's do spark when you connect them though, especially at the higher S's
```

---
## \#20 Posted by: treenutter Posted at: 2015-12-16T16:20:35.923Z Reads: 158

```
[quote="siggs3000, post:19, topic:243"]
Lipo's do spark when you connect them though, especially at the higher S's
[/quote]

@siggs3000 @Paul There are a few ways to avoid the spark when connecting Lipos; I use a battery arming switch that has a small, temporary resistor. Kinda like this thing below. If the spark is just the normal "connection spark," the danger is that it will wear out or melt your connectors. This thread is about something more complicated, but I thought I'd note that it is possible to mitigate the connection spark.

<img src="/uploads/db1493/original/2X/3/32e05b7e7a8bfac5456e5065afe0e8425d62551f.jpg" width="307" height="229">

There are also xt90 antispark plugs, which are effective but giant:

<img src="/uploads/db1493/original/2X/4/4d386546fa94cb6cd942b8b041b55a767689d201.jpg" width="588" height="500">

@sl33py is working on [builds of Vedder's antispark switch][1] 


  [1]: http://www.electric-skateboard.builders/t/anti-spark-switch-kit-extras-for-sale-vedders-v1-3/384
```

---
## \#21 Posted by: siggs3000 Posted at: 2015-12-16T18:43:08.023Z Reads: 155

```
Actually that's true. I received my new vesc yesterday from @chaka and it has those diesel  XT90 connectors on it with heavy duty 10 gauge wire and it doesn't spark at all when I plug it in. Super nice.
```

---
## \#22 Posted by: Timur Posted at: 2016-06-25T20:26:52.735Z Reads: 128

```
Hello guys! Sorry for posting in an old thread but my problem perfectly fits in here. 
So I plan a build with 2 3s lipo packs wired in series. I bought this serial charging harness - http://www.hobbyking.com/hobbyking/store/__10993__Twin_pack_charge_lead_2_x_3S_6S_w_XT60.html, which has  XT60 plug for charging while my imax b6 charger's cable has a dean plug. today I removed the xt60 from the harness and soldered the dean connector to be able to connect the charger's cable and the harness. Then I thought I'd try to connect the batteries (though there were not used yet, completely new) and the harness together - to check the soldering quality - to see if voltage would be there with a voltmeter. So I connected to batteries in series (as on photo), then I plugged the 1st balance lead into the harness' port - all was good, when i connected the 2nd batteries balance lead - there was a pretty good spark, you can see the damage of one of the pins. could this have damaged the lipo? I measured the voltage afterwards - was fine.  

I am a real newbie. Can someone tell me what did I do wrong? I tried to read the forums and this thread and if i understood well i should cut out the black wire of one of the balancing leads according to @lowGuido's beautiful diagram. But I feel confused because everyone else seems to use my type of harness without any troubles. Thanks in advance.

 
 <img src="/uploads/db1493/original/2X/a/a894f99bc506656498ddce8ece269d0d5f53bf0e.jpg" width="666" height="500">
<img src="/uploads/db1493/original/2X/1/1beaf41e62dee06b7412f23bbd57ebb9f57ff44e.jpg" width="375" height="500">
```

---
## \#23 Posted by: mason Posted at: 2016-06-25T20:33:09.203Z Reads: 117

```
heres what you do:
1. Wire the batteries in series FIRST
2. take your 2x 3s to 6s adapter and cut the black wire closest to the middle ( you will need to cut through the heat shrink)
3. Now you should be able to run this safely
if you plug in the lipo alarm/voltage reader and it shows 3s, switch the two connectors around.

If you do this in any other order expect to get a shit ton of sparks
```

---
## \#24 Posted by: Timur Posted at: 2016-06-25T21:01:57.158Z Reads: 118

```
Hi, thanks a lot for your reply. I uploaded the photo of harness once more - I assume you refer to the thin black wire of the 6 pin balancing lead? 

Does it matter where I cut this wire if I isolate the cut pieces well? I would also appreciate if you could shortly tell me why does this wire cause sparks? And I find it strange that this piece is sold as a plug-n-play product and there are some extra tweaks required.... I also saw other people's reviews on HK - they all seemed happy and noone mentioned cutting wires. :slight_smile:  

Will I actually be fine charging through this harness - I mean using the dean plug I soldered? My plan was to do charge over the harness keeping batteries in the board however with a disconnected circuit (XT90s loop switch).

Thanks a lot!

Edit: BTW, you emphasized the order but you didn't mention the right moment for connecting the batteries to the harness - should it always stay connected or it doesn't matter when you connect them? :)

<img src="/uploads/db1493/original/2X/0/0aa4244082176d6c57915379da791566ab6ef184.png" width="510" height="370">
```

---
## \#25 Posted by: mason Posted at: 2016-06-25T22:01:31.077Z Reads: 117

```
I should also mention I used this exact product, and charging was horrendously slow due to it being charged through balance leads. Instead, wire a xt60/Dean in parallel to the wires feeding to your ESC and plug in through that, it will provide a higher current. 

1. Yes I mean the thin wire on the 6 pin. You should isolate it.
2. It shorts out, thus sparking.
3. you should be fine charging with this harness, though like I said above its not as fast.
4. Connect the batteries after all my steps
```

---
## \#26 Posted by: Timur Posted at: 2016-06-25T23:37:50.004Z Reads: 117

```
Thank you. so you recommend the following wiring (creation of @lowGuido): 
<img src="/uploads/db1493/original/2X/e/e992fcb008e2adb74cbfa50371901c5cf1f34738.png" width="187" height="500">

I have couple of questions:
- I read somewhere that it's not good to have long wires between the battery and esc, I guess it is not true?
- what is the min wire thickness I should stick to for charging wires - I read somewhere that AWG10 is min, is it?
```

---
## \#27 Posted by: mason Posted at: 2016-06-26T00:20:33.502Z Reads: 112

```
Yes that diagram is great. 12 AWG is pushing it, 10AWG is perfect for our use. Wire length shouldn't matter as long as it's not 3+ ft. Though you want to try and keep it as short as possible. If you are using a VESC and FOC, keep it very very short!
```

---
## \#28 Posted by: lowGuido Posted at: 2016-06-26T01:50:27.648Z Reads: 108

```
You need to make sure that your most negative battery has its balance leads plugged into the negative side of the balance connector. Getting this wrong is what causes your short. (Spark)
```

---
## \#29 Posted by: Timur Posted at: 2016-06-26T09:20:58.002Z Reads: 102

```
Thanks for reply. Could you please clarify what means " the most negative battery" - the one with a negative terminal going to ESC? 

And how do to determine which one of two balance slots is negative? Sorry for the "newbie" questions.

Will the method described by  @link5505 - disconnecting  the thin black wire of the harness balance lead will eliminate the necessity of watching for the most negative battery? 

Thanks.
```

---
## \#30 Posted by: Timur Posted at: 2016-06-26T09:29:53.451Z Reads: 100

```
I don't know what's the AWG of the wire I have but it's from the electric kettle - so handles 240v normally, and current of certainly 16A. That should do, right?<img src="/uploads/db1493/original/2X/a/af5868cb9bcc527da5995bd921dc77b7d61abcff.jpg" width="375" height="500">

BTW: is it an idea if I use those wire endings / terminals (donnow how it's called in English) to create parallel wire splittings for charging? I hope you get what I mean ? :blush:
```

---
## \#31 Posted by: Timur Posted at: 2016-06-29T18:33:01.024Z Reads: 87

```
I would love to get a confirmation from someone. Thanks in advance.
```

---
## \#32 Posted by: lowGuido Posted at: 2016-06-29T21:19:29.421Z Reads: 84

```
that kettle wire will not do the job. buy some nice 12 AWG at a MINIMUM.

the "most negative battery" would be the one on the right of my diagram, the one that has the big negative wire to the ESC.
```

---
## \#33 Posted by: Timur Posted at: 2016-07-03T16:22:11.319Z Reads: 79

```
Hi, thanks for your advice, I did get some super thick wires - my colleagues use them for assembling the electric car chargers. AWG  number isn't there but the its a stranded copper wire with a total cross section of certainly more than 3mm.

Will the method described by @link5505 - disconnecting the thin black wire of the harness balance lead will eliminate the necessity of watching for the most negative battery? Thanks.
```

---
