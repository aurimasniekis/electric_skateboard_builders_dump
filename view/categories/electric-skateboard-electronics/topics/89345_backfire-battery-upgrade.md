# Backfire battery upgrade

### Replies: 10 Views: 514

## \#1 Posted by: Gisop Posted at: 2019-04-04T15:32:35.990Z Reads: 82

```
Hello,
I'm new to the e-board building. Right now I'm not doing any e-board build but I just want to upgrade my Backfire. I'm planning to connect one of these batteries (pictures) to my Backfire Galaxy G2s in parallel. My question is if it is possible without any damage to my board. The battery that is included in the orig. board is the first one.
Thanks for suggestions.

![Sn%C3%ADmek%20obrazovky%20(31)|690x225](upload://fqL5htXv47AVYwhnWrQppdwMWZU.png) ![Sn%C3%ADmek%20obrazovky%20(33)|690x228](upload://eL3GXRkc2iQN1yfhKstzo8cj2e3.png)
```

---
## \#2 Posted by: olestra Posted at: 2019-04-04T15:51:52.213Z Reads: 76

```
mixing old and new batteries is generally a poor idea even in a parallel setup, mixing different capacities and types -- I would only do that with stuff that was free.

In an extreme example, the reason is that in a parallel set up, even new, you wouldn't really have a capacity of 180WH + 216WH, you would have 180wh+180WH, yet the voltage would show still having capacity left, you would end up over-discharging the weaker battery leading to it failing sooner.

If you strapped on the 2nd battery, and just switched connections from one to the other when the first ran low (like a truck with two gas tanks) -- you could do that with no damage. 

However, by asking this question, I'm guessing that you don't have much electrical experience -- if that's the case, it's unlikely you would setup a safe method to switch between them. If you go for it, find a makerspace, or a friend you can visit in person to help set it up.
```

---
## \#3 Posted by: Gisop Posted at: 2019-04-04T15:56:46.190Z Reads: 72

```
Thanks for explanation :+1:
```

---
## \#4 Posted by: Sn4pz Posted at: 2019-04-04T16:03:22.711Z Reads: 65

```
[quote="olestra, post:2, topic:89345"]
you could do that with damage.
[/quote]

I think you meant to type no damage

That is probably the best way to use both packs, especially considering you have the ESC that comes with it. Just make sure to have somewhere to store the loose power cables, you don't want a short as it dangles in some puddle 😂😂

And to please turn it off before switching... I feel like that doesn't need to be said though 😂
```

---
## \#5 Posted by: olestra Posted at: 2019-04-04T16:15:56.125Z Reads: 57

```
Thanks for the catch! you're right, "no damage"  I'll fix my post
```

---
## \#6 Posted by: skatardude10 Posted at: 2019-04-04T17:24:17.371Z Reads: 56

```
Whenever parallel packs come up for extra range, I've got to mention boost converting a smaller pack to charge voltage and charging on the go.

It's relatively compact, can be in a backpack, on your board, stored away for a quick charge on the road during breaks, whatever you want. 

You can use a range of smaller or larger batteries. I use power tool batteries. When I ride, I click in a power tool battery that extends my range significantly. Set the boost converter to charge voltage and set amp limits, connect battery to input, connect output to charge port. 

After 12 miles of charging on the go I'm usually sitting at 85-90% charge when riding hard, carry as many extra batteries as I think I'll need. Otherwise I'm usually around 30% without the boost converter.
```

---
## \#7 Posted by: morrisxyz Posted at: 2019-04-04T20:14:04.287Z Reads: 49

```
This is what you're looking for

https://www.youtube.com/watch?v=QfYvA-OaAds

Edit: It's an example, I'm not saying this is how you _should_ do it.
```

---
## \#8 Posted by: Mikenopolis Posted at: 2019-04-04T22:09:17.847Z Reads: 45

```
Are there battery builder here from Czech Republic - Prague? that can help?

I would highly suggest just building a larger single battery pack with flex as to not mix the old and new cells.
```

---
## \#9 Posted by: meesie Posted at: 2019-04-05T14:38:41.809Z Reads: 38

```
@ElectricPacks

he might be able to help you increase your range.
```

---
## \#10 Posted by: janpom Posted at: 2019-04-05T14:57:28.909Z Reads: 32

```
There's a [Czech esk8 group](https://www.facebook.com/groups/esk8cz/) on FB. There are at least a few people from Prague who have built their battery packs. There's also Štěpán from Wattboards (Brno based company) who distributes the Backfire boards. You may find some help there.
```

---
