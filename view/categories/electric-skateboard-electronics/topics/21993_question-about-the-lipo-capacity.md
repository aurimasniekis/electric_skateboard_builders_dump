# Question about the lipo capacity

### Replies: 15 Views: 574

## \#1 Posted by: domfeng123 Posted at: 2017-04-28T22:29:47.951Z Reads: 65

```
Hi I just built my first DIY skateboard, using an cute old school santacruze deck.
I have a question about the battery I am using. it is this one:
ZIPPY Compact 5000mAh 6S 25C Lipo Pack

I found article online say that you can only use 80% of your battery capacity,
so every time, i will left 1000mAh in my battery, so when i charge it, it will only
need about 4000mah to get fully charged?

Is this the right way? or should i just can use all 5000mAh ?
```

---
## \#2 Posted by: Michaelinvegas Posted at: 2017-04-28T23:14:12.895Z Reads: 61

```
Just easier to look at it in terms of voltage. Gonna drive yourself nuts.
```

---
## \#3 Posted by: Okami Posted at: 2017-04-28T23:21:58.331Z Reads: 60

```
@domfeng123 Just dont charge up till 4.2v, kiddo

Choose Li-ion setting when charging.. thus you will spare your pack some cycles..

If you dont want to compromise on capacity, set it to 4.15v.. thus you will be in between ;)

(that is if your charger allows you to change current)

--
Plus, I think it is hard to ''pull'' all 5000mah out of the pack.. you usually just end up using 4800mah or so anyways.. if you do get 5000mah .. hands down to your lipo pack!
```

---
## \#4 Posted by: domfeng123 Posted at: 2017-04-28T23:29:16.916Z Reads: 53

```
@Okami
Thanks a lot for your reply

i found this article online:
https://goo.gl/1z3odI

do you think it is good practice to just leave 1000+mah in battery for every time i use ?
```

---
## \#5 Posted by: lowGuido Posted at: 2017-04-28T23:30:12.148Z Reads: 50

```
it all depends on the quality of the pack. I have pulled 5100mAh from a 5000mAh pack before it reached 3.00V per cell before, but on the flipside I have also had packs drop to 3.00V on a cell before 5000mAh has been used.

a good quality pack should deliver what it advertises, just be aware that some companies lie about their mAh ratings.. 9000mAh from an 18650 is probably a lie.

its probably also worth nothing that battery voltage percentage is not the percentage of the battery used. so when my battery meter on my board reads 70% I have actually used about HALF of my capacity.. so.. stay woke LOL.
```

---
## \#6 Posted by: domfeng123 Posted at: 2017-04-28T23:32:33.974Z Reads: 49

```
@lowGuido Oh, kind of heard about that, lol, thanks.
So what you mean is how many mah you use is not accurate,
just not let the battery v  below  3v never is enough ?
```

---
## \#7 Posted by: lowGuido Posted at: 2017-04-28T23:38:31.155Z Reads: 45

```
actually what Im saying is the mAh you use is MORE accurate that the battery voltage..

say for a 5000mAh battery when you have used 2500mAh you have used 50% of you battery capacity, but if you look at the voltage meter it might still read close to full..
the battery voltage stays high for longer, once it starts to drop it drops rapidly..

so when I ride my voltage stays around 90%+ for a say the first 45 mins but then once it hits 60% it will drop to nothing within 10mins.
```

---
## \#8 Posted by: Okami Posted at: 2017-04-28T23:43:42.187Z Reads: 41

```
@domfeng123 for you.. better staying in 3.4v-3.5v per cell would be best..

I think lowest you want to go for lipo is 3.3v..

They need to be a bit higher in voltage than regular li-ions..

If im wrong.. just say @lowGuido
```

---
## \#9 Posted by: domfeng123 Posted at: 2017-04-28T23:45:46.676Z Reads: 36

```
Thanks a lot, i will test that and see what is max mah i can use :slight_smile:
```

---
## \#10 Posted by: Okami Posted at: 2017-04-28T23:48:02.443Z Reads: 36

```
It might be close to 4ah you mention.. but I think you can aswell use 90%.. just dont use it all the time.. only occasionaly

It is a recommendation.. not a rule you have to obey for all costs.. Your skateboard will just get slower.. and as lowguido says.. in the last 10% or so.. the drop in voltage / power might be a bit drastic, so it is wise not to use your board beyong this point..at least that is what I would do .. not to destroy the balance of the cells a lot.
```

---
## \#11 Posted by: lowGuido Posted at: 2017-04-28T23:48:13.019Z Reads: 35

```
don't forget voltage sag! so when you are riding you might drop down as low as 2.9V or even lower under load and when you take it off load you are still at 3.2v-3.3v so I set my alarm at about 3.0

having said that its always best to never fully discharge all the way so.. learn your range and never go too far.
```

---
## \#12 Posted by: Okami Posted at: 2017-04-28T23:49:12.742Z Reads: 32

```
@lowGuido  So do you finish discharging batteries at 3.2-3.3v?

I heard in the other topic you said you barely discharge more than 50%.. is that true also?
```

---
## \#13 Posted by: lowGuido Posted at: 2017-04-28T23:53:10.023Z Reads: 33

```
my pack is 10000mAh and most of my skates are about 7km which uses around 3000mah 
so I re charge after every skate. I almost never go lower than 3.8V per cell
unless Im doing a full range test when I will purposely drain the batteries down to 3.0v per cell to see how far i can push it.
```

---
## \#14 Posted by: Okami Posted at: 2017-04-28T23:54:41.278Z Reads: 33

```
Good ''economy'' on battery life, that''s for sure :D

curious how many kilometers can you do.. drawing only 3ah for 7km does sound good..
```

---
## \#15 Posted by: lowGuido Posted at: 2017-04-28T23:56:40.019Z Reads: 32

```
interestingly enough a 7km skate with a 3000mAh drain still reads 85% on my battery...
 longest ride I have done is 22km till cells at 3.00v
```

---
