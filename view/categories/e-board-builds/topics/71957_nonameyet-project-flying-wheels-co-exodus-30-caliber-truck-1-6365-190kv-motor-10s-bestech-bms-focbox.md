# Nonameyet project &#124; Flying wheels co Exodus 30&rsquo;&#124; caliber truck 1 &#124; 6365 190Kv motor &#124; 10S &#124; Bestech BMS &#124; FOCBOX

### Replies: 11 Views: 390

## \#1 Posted by: Kev06 Posted at: 2018-10-22T14:12:32.933Z Reads: 144

```
Hi everyone !

I spend a lot of time on this forum and it's been a lot of inspiration and learning!

Leaving in south east of France, we have a lot of up and downhill, when you just wanna drop your car and ride the rest of you travel by skate well, early in the morning you don't really think of warming up you legs and fews month later you get hurt.. So it was a good motivation to start building an esk8 !
5 years ago I made a very cheap and unpowerfull esk8. only flat grounds and no brake only motor brake => pretty useless!

Few years later I want something powerfull and secure!
So I went ahead with this new setup.

Everything is now designed assembled and ready to test.

My only problem is a mistake when wiring up the BMS. Instead of wiring the wire of the cell 5 I wired the cell 10. 18,5V instead of 3.7V and the serie of resistors began to melt. I immediatly unplug it but the mistake was done.
![wiring|690x287](upload://4chzrrzN6WOjDB0CrwxuyafXNxi.jpeg) 
![20181016_123735|281x500](upload://9yNZTnPk5qXVxak26bPgaFB4YPo.jpeg) 
So I decided to contact bestech so they could tell me the exact reference of the smd resistor. 1week later I received them and started to remplace the burned ones.
But now my BMS is warming up a bit when the cells are connected to it.
Warming = current going through the BMS = batteries that will slowly discharge when the board is stored. Worse, cells are going to disbalance each other. 
I don't want that. 

Maybe somebody can help me with this? If you need more informations feel free to ask;)
Also when I'm tryig to charge the batterie with a 42V charger, it doesn't seems to charge anything, the green led on the charger is on and nothing is happening.
I know I'm not the only one who got this problem so if you solved it some advice are welcome  :slight_smile: 

Here come the picture of the project !
I'd love to have you feebacks ;) !!

![20181015_100957|690x365](upload://5EAv3jq8uD0JsjVO7mid3B9YqmF.jpeg) ![20181015_115715|690x388](upload://rKX3ECZlJ7XKloAnsOTmAhFeXZP.jpeg) ![20181016_123735|281x500](upload://9yNZTnPk5qXVxak26bPgaFB4YPo.jpeg) ![20181018_085007|690x388](upload://vCnnwZzc7oSHWMEANw0LIHo82Da.jpeg) !
![20181018_221333|473x500](upload://zJDGtg1wAJ47Xa7Y0vXHIWDcBgx.jpeg) ![20181019_102932|690x388](upload://8A8wv9VnBBxvyU09bjsQoFQdegE.jpeg) ![20181020_100323|281x500](upload://vMp59A4YY7EF53CmUxZtZLIorfT.jpeg) ![20181020_133853|690x388](upload://d9cZYOH9CHWgIQalw9zCnXFbwUp.jpeg) ![20181020_134119|690x388](upload://c53LzeiLSn1LemPwxTEMjKZ2Y0c.jpeg)
```

---
## \#2 Posted by: Grozniy Posted at: 2018-10-22T14:24:27.600Z Reads: 114

```
Why not get yourself a charge only bms? It would be 1/4 of the size and maybe cheaper
```

---
## \#3 Posted by: Kev06 Posted at: 2018-10-22T14:57:55.610Z Reads: 111

```
I don't know actualy, I never used a BMS before and I only know that it's protecting my batteries from overdischarge (The focbox does it), but also over current over temperature and short circuit.

But I'd like to have your point on view about that ;)
```

---
## \#4 Posted by: nuttyjeff Posted at: 2018-10-22T15:01:24.196Z Reads: 113

```
1. The BMS is huge! a charge only BMS can really help with that.
2. The casing will break. It will. ><. Unless you're strengthening it somehow?
```

---
## \#5 Posted by: Kev06 Posted at: 2018-10-23T09:57:13.649Z Reads: 76

```
YEah it's huge...
Do you have a brand to advice?

And for the enclosure, yeah maybe it's gonna break, but not sure I wanna give it a try ;)  it seems pretty strong for me ^^

For now I'm gonna let down the BMS and connect directly the batteries with the focbox. I hope they will keep a good balance with the time...
What do you think ?
```

---
## \#6 Posted by: pat.speed Posted at: 2018-10-23T11:13:56.861Z Reads: 69

```
Generally the cells stay reasonably balance when new. I would get a cheap charge only bms on eBay. They cost about $10 and super simple. The problem I’ve found with lipos is that the over discharge is pointless as it only trips at 2.5v at which point your batteries are already destroyed. Therefore you might as well use a charge only one
```

---
## \#7 Posted by: Grozniy Posted at: 2018-10-23T15:02:52.163Z Reads: 61

```
http://www.bestechpower.com/37v10spcmbmspcbforli-ionli-polymerbatterypack/BMS-D141.html
This one might work
```

---
## \#8 Posted by: Kev06 Posted at: 2018-11-22T08:36:21.903Z Reads: 45

```
Sorry for no answering so long! The fact is without BMS my batteries work just fine. I just want to charge them without open the case everytime. So a cheap BMS will do the work indeed. I found one on amazon (with prime^^) that looks exactly the same as an ebay&apos;s one. What do you think of it?

https://www.amazon.fr/Protection-Equilibrage-Surcharge-Surintensit%C3%A9-Court-circuit/dp/B075MFBB23/ref=pd_aw_sim_23_1?_encoding=UTF8&amp;pd_rd_i=B075MFBB23&amp;pd_rd_r=c4873911-ee2f-11e8-8f7c-734f98c58a09&amp;pd_rd_w=CtdKS&amp;pd_rd_wg=i2Yh4&amp;pf_rd_i=mobile-dp-sims&amp;pf_rd_m=A1X6FK5RDHNB96&amp;pf_rd_p=4b7b81c8-113c-4bed-b8e0-946ac958e96d&amp;pf_rd_r=7VH6CAWQNKV7KE1YFRTM&amp;pf_rd_s=mobile-dp-sims&amp;pf_rd_t=40701&amp;psc=1&amp;refRID=7VH6CAWQNKV7KE1YFRTM
```

---
## \#9 Posted by: pat.speed Posted at: 2018-11-22T11:41:36.776Z Reads: 38

```
Looks fine, I've got a similar variant on my 12s lipo board

Edit: it's got a bad review, I did translate it to english and seems just like the guy couldn't figure out the wiring but I'd be wary
```

---
## \#10 Posted by: Kev06 Posted at: 2018-11-22T13:16:50.653Z Reads: 34

```
Yep I saw. But this guy didn't see all the pictures. I found this.![_AC_SY400_|326x400](upload://4WrNTa6E4G5kXEnrHuX4gfLZo3L.jpeg)

I will receive it tomorow.
Maybe I will need some advise with the wiring for charge only but it should be ok ;)
```

---
## \#11 Posted by: Kev06 Posted at: 2018-11-24T16:21:52.331Z Reads: 26

```
Hi !

So I receive it today. I made a wiring sketch so I don't get confused.
Since I only use the BMS as a charger, I think I'm good with the wiring. Anyone who can confirm :) ?
Also Can somebody tell me why there is this wire ( in the blue arrow) and should I not wire it ?!

Thanks for your help !!

![_SL1001_%20-%20Copy|690x346](upload://iDxfP8eYFyAavJKciV2hFyrj00P.jpeg)
```

---
