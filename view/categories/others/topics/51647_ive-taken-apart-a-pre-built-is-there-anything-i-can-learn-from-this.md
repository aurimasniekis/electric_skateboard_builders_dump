# I&rsquo;ve Taken Apart a Pre-Built, Is There Anything I Can Learn From This?

### Replies: 26 Views: 2766

## \#1 Posted by: CHAINMAILLEKID Posted at: 2018-04-09T03:57:37.613Z Reads: 407

```
The story is I was sent a board to review.
I can cover the quality of the skate components well enough, but I was hoping to dig down and figure out if the electronics were decent, more specifically I want to at least make sure that all the things that SHOULD be there are all present.

I know a little bit about electronics in general, but I'm still new enough here that a lot of this is going over my head a little bit, and I certainly don't know what to look for.

I've cleaned it all up so its a lot easier to see whats going on, originally every single connector was glued down, generously, and there was non-conductive cardstock covering the PCB

![IMG_0770|690x460](upload://2cIFrSB7i7DOOpUKkFvQrTTcHWC.JPG)

![IMG_0768|690x460](upload://ogcDKtiMyNXBg6Bt6uZ7B250rQJ.JPG)

![IMG_0769|690x460](upload://qPZgp2c2GXqbWy5MCAbZ0M9A5oF.JPG)

I was actually originally hoping that the components were just knockoffs. If they're cloning something we know is good, well chances are its still pretty good. And that way I also might be able to use the BLDC Tool or something to learn even more. But it doesn't look like it.

The Battery Enclosure is built into the deck, and I need to take off the grip tape in order to get to it.
I plan on doing that and having a look, seeing what cells they're using etc. But I'll need to get some good footage of it before I go messing that up.

Apart from satisfying my own curiosity, the thing I'm trying to get from this is an idea of how recommendable this complete might be. I know there's a lot of other factors, but for context this is a $530 setup.
```

---
## \#2 Posted by: Jedi Posted at: 2018-04-09T04:03:27.702Z Reads: 388

```
What is the name of the board?
```

---
## \#3 Posted by: CHAINMAILLEKID Posted at: 2018-04-09T04:06:00.403Z Reads: 384

```
Its the Teamgee H6

https://www.amazon.com/Electric-skateboard-Solution-Longboard-Companion/dp/B079L5QT7Z

They're new, as far as I can tell brand spanking new.
Haven't even got their English website up yet.
```

---
## \#4 Posted by: TarzanHBK Posted at: 2018-04-09T09:03:26.929Z Reads: 345

```
These boards are all the same asian baords but look a bit different.

The ESC is this one: http://www.diyeboard.com/v11-dual-hub-motors-sine-wave-foc-esc-speed-controller-p-608.html

Hub motors: http://www.diyeboard.com/replaceable-pu-hub-motor-8352mm-450w-for-diy-eboard-p-626.html
```

---
## \#5 Posted by: CHAINMAILLEKID Posted at: 2018-04-09T09:09:24.990Z Reads: 333

```
Nice.
Thats definitely the same board.

I'd already figured the motors were all the same.


That makes it pretty straight forward.
```

---
## \#6 Posted by: b264 Posted at: 2018-04-09T09:12:47.281Z Reads: 317

```
Do you have photos of the battery?  Does it contain cylindrical cells or prismatic pouches?
```

---
## \#7 Posted by: CHAINMAILLEKID Posted at: 2018-04-09T09:13:49.557Z Reads: 306

```
Don't know yet.

Haven't opened the battery enclosure yet as its embeded in the deck, and I'd have to cut open or remove the grip.

But I certainly will be taking a look.
```

---
## \#8 Posted by: esk8thunter Posted at: 2018-05-04T10:18:43.638Z Reads: 266

```
you can find their battery picture at their instagram account.

https://www.instagram.com/teamgeeskateboard/
```

---
## \#9 Posted by: esk8thunter Posted at: 2018-05-04T10:19:14.463Z Reads: 250

```
their site www.teamgee.com.
```

---
## \#10 Posted by: Wilsonliang777 Posted at: 2018-05-21T06:37:47.966Z Reads: 221

```
I really like the teamgee board.  I have 3 diy boards myself.   The simplistic design is what i want in a last smile commute board.
```

---
## \#11 Posted by: CHAINMAILLEKID Posted at: 2018-05-21T06:39:04.471Z Reads: 218

```
Oooh, last mile commute board,I like that.

I'm definitely going to be using that term in the future.
```

---
## \#12 Posted by: Mikenopolis Posted at: 2018-05-21T06:46:40.369Z Reads: 217

```
Definitely prismatic pouch type batteries. 

Watch this video
https://youtu.be/Pf5clVL0GGw

![image|690x387](upload://7mL7t1sBLC6lsemQy3xEPCA2CT6.jpg)
```

---
## \#13 Posted by: lrdesigns Posted at: 2018-05-21T07:35:44.407Z Reads: 201

```
![image|580x315](upload://a2OCGMYc2u575ZUgPGMNS5yovto.jpg)

lols.
```

---
## \#14 Posted by: Exigent Posted at: 2018-05-21T16:03:59.315Z Reads: 192

```
I noticed in the last of the top 3 images you label "Copious amounts of Thermal Paste".

If it is in fact "copious amounts" of thermal paste then that is a VERY BAD thing in any electronic system. The effectiveness of thermal paste is significantly degraded when there is a thick layer of it between the heat generating electronic component (e.g. CPU, MOSFET, etc) and the heatsink. A large quantity of "something" may indicate it's not even "thermal paste" but in fact a binding, electrically insulating, and/or vibration-dampening material of some sort.
```

---
## \#15 Posted by: TowerCrisis Posted at: 2018-05-21T16:18:39.145Z Reads: 187

```
@Exigent That's largely a myth regarding thermal paste. Using too much is far better than too little, as it only increases thermals by 1-2°C. Consistent mounting pressure reduces thermal paste to the same thickness, regardless of how much was applied. IE: open up any stock graphics card, and you'll see thermal paste splooging all over the sides of the die.


Too little on the other hand is very bad.
```

---
## \#16 Posted by: Exigent Posted at: 2018-05-21T23:52:15.973Z Reads: 171

```
Both personal and professional manufacturing long-term experience and empirical lab data show differences in the temperatures of components under potentially high thermal stress can be substantially more than "1 to 2 degC" if there is a "thick" layer of thermal compound between the component and its associated heatsink. It can mean the difference between proper operation, delayed failure or out-of-spec operation, and catastrophic failure of the component. The chemistry of the thermal compound can also make a huge difference.

I do fully agree with the statement that "Too little on the other hand is very bad."
```

---
## \#17 Posted by: TowerCrisis Posted at: 2018-05-22T00:13:33.466Z Reads: 166

```
I also agree with your statement about thick amounts of thermal compound. However in most use cases mounting pressure reduces thickness to a reasonable width. Improper use and thick application is definitely a bad thing.

In this case, seeing excess thermal paste splooging from the sides really is no indication of what thickness is underneath the PCB.
```

---
## \#18 Posted by: Exigent Posted at: 2018-05-24T04:25:35.466Z Reads: 146

```
[quote="TowerCrisis, post:17, topic:51647"]
In this case, seeing excess thermal paste splooging from the sides really is no indication of what thickness is underneath the PCB.
[/quote]

I partially agree with you on that at the base technical level. However, in my experience "splooging" thermal compound reveals a very sloppy manufacturing **or rework/repair** process with low quality control. _Without testing, I would have very low confidence that the compound was properly applied and I would be concerned about a higher probability of latent component failure._
.
.
.
Boring factors for any that might be interested...

Manufacturing Cost Issues...
Generally, good quality thermal compound is not cheap. It can cost $/gram even to OEMs. For comparison, it can cost more than a MOSFET for a single application (although the gunk used by some manufacturers is not very high quality and even manufacturers sometimes get counterfeit or wrong partnumber marked products),

Regardless, all manufacturers that I know try to keep manufacturing costs to a minimum, seeking ways to save even pennies on producing a circuit board. "Splooged" expensive thermal compound is a needless waste of money when you're manufacturing thousands to 100's of thousands of circuit boards. It adds up.

At The Forensic Level...
Such sloppy application can even be a clue indicating an inexperienced worker or DIYer has worked rather invasively on the circuit. Such clues can also indicate a potentially used and repaired circuit-board has been installed in a "new" product or someone is mis-representing an repaired/recycled item as new.
```

---
## \#19 Posted by: Wilsonliang777 Posted at: 2018-06-07T05:37:10.125Z Reads: 128

```
teamgee is About up luanch h9.   it's selling for $450 on indiegogo.   I saw a Facebook link selling this board for $400 too.   I wish I have the extra spending cash now.   

 https://www.indiegogo.com/projects/teamgee-ultrathin-and-lightweight-electric-board#/comments
```

---
## \#20 Posted by: fichelmassbender Posted at: 2019-03-29T09:20:12.431Z Reads: 97

```
Cool!

If i want to extend the cables (motor A and motor B, as seen in the picture), how would i do it? What cable type is it really?

Thanks
```

---
## \#21 Posted by: Mikenopolis Posted at: 2019-04-01T06:52:31.674Z Reads: 86

```
[quote="fichelmassbender, post:20, topic:51647"]
What cable type
[/quote]



You are looking for an MR30 connector
```

---
## \#22 Posted by: Stillshreddin Posted at: 2019-06-01T21:57:06.583Z Reads: 73

```
Question. I have the h5 blade...what can I replace on this board to upgrade the performance? Is it possible to maybe plug in an external battery pack? Maybe change the escape or hub motors?
```

---
## \#23 Posted by: TarzanHBK Posted at: 2019-06-02T07:51:07.919Z Reads: 54

```
Basically these boards have their own setup of parts and your not able to change much.
If you're not satisfied with the performance, you have to get something stronger.
```

---
## \#24 Posted by: albardo Posted at: 2019-06-04T18:43:34.684Z Reads: 38

```
Sorry for offtopic.
Hey Torben, are you still making batterypacks ? How to get in touch with ya. I am from germany too...
```

---
## \#25 Posted by: TarzanHBK Posted at: 2019-06-05T16:10:52.163Z Reads: 33

```
Hi Albardo, yep still rockin´
Pretty bussy with lot´s of Evolve Batteryupgrades lately, but hit me up, I´ll pm you my number
```

---
## \#26 Posted by: Lyricaldiego Posted at: 2019-06-12T20:12:04.960Z Reads: 23

```
Hey would you happen to troubleshoot these computers and motors?
```

---
