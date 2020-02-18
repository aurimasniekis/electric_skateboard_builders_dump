# Will this battery work

### Replies: 21 Views: 381

## \#1 Posted by: marshal Posted at: 2019-05-29T21:20:07.599Z Reads: 128

```
I was watching a video by skatemetric where they build an all terrain electric longboard and they use these batteries:

https://hobbyking.com/en_us/turnigy-high-capacity-battery-12000mah-6s-12c-drone-lipo-pack-xt90.html

I want to use 1 of these batteries to power a 6s electric longboard.
Will this battery have good enough output to power my board.
```

---
## \#2 Posted by: barajabali Posted at: 2019-05-29T21:56:14.247Z Reads: 119

```
It will work but it’s not ideal. You should really consider a lithium ion pack, more investment but will work much better for you
```

---
## \#3 Posted by: marshal Posted at: 2019-05-29T21:59:02.532Z Reads: 115

```
Can I ask what you mean by not ideal.
```

---
## \#4 Posted by: barajabali Posted at: 2019-05-29T22:02:36.763Z Reads: 109

```
There are a few topics on lipo vs lion, check them out and let me know if you have questions
```

---
## \#5 Posted by: bartroosen12 Posted at: 2019-05-29T22:06:52.621Z Reads: 103

```
What esc are planning to use?

I also think you can make a better battery for just a bit more money with 18650 cells, go for the samsung 30Q (like a 10S4P)

If you can't make it by yourself, buy at least 2 of these lipo's and put them in series to make a 12S pack.
```

---
## \#6 Posted by: Halbj613 Posted at: 2019-05-30T09:07:33.765Z Reads: 74

```
there only 12c so there amp output wont be much
```

---
## \#7 Posted by: marshal Posted at: 2019-05-30T09:51:09.413Z Reads: 70

```
Im planning to use this esc:

https://www.ebay.co.uk/itm/Dual-motors-longboard-skateboard-controller-with-remote-ESC-Substitute/302812941839?var=601709105318

With two of these motors:

https://www.ebay.co.uk/itm/1X-6354-Brushless-motor-for-scooters-180kv-1920W-8S-Lipo-for-electric-skate-L4B1/233193082373
```

---
## \#8 Posted by: marshal Posted at: 2019-05-30T09:56:56.426Z Reads: 57

```
I did the calculations and this lipo should be able to output continuous 144 amps
```

---
## \#9 Posted by: JulianS Posted at: 2019-05-30T10:09:38.788Z Reads: 57

```
From an engineering standpoint there's not much to say against the pouch cells. They might have slightly worse lifetime, but they are probably much cheaper. You could consider taking 2 of the yellow turnigy 6200 in parallel, they usually have a higher C ratings. You need to protect those a bit better then 18650 or 21700 though.
```

---
## \#10 Posted by: marshal Posted at: 2019-05-30T10:21:40.910Z Reads: 54

```
Thanks Ill have a look at those batteries
```

---
## \#11 Posted by: Andy87 Posted at: 2019-05-30T10:22:16.843Z Reads: 56

```
[quote="marshal, post:8, topic:95431"]
output continuous 144 amps
[/quote]

unfortunately the C rating is not a norm, so the rule capacity * C-Rating is max amp output is not really right. the cheaper the lipos the more it will not fit. the multistart 12Ah lipos are rated for 12C as well but in real life measurements they came out to be only able to supply 3-4C.

If you look for a relatively cheap and good option I would look at the Heavy duty line from Hobbyking. they not bad and hold up pretty good with there 60C.
```

---
## \#12 Posted by: Andy87 Posted at: 2019-05-30T10:24:22.989Z Reads: 50

```
If you non the less want to go with the high capacity lipos the hobbyking graphene 8Ah and 12Ah are a very good choice as well.
```

---
## \#13 Posted by: bartroosen12 Posted at: 2019-05-30T11:23:39.850Z Reads: 44

```
The esc is only like 40A max.
I think the 6S 12Ah lipo won't be a problem to deliver that power.
```

---
## \#14 Posted by: marshal Posted at: 2019-05-30T13:47:28.188Z Reads: 37

```
Thanks for some actual information everyone else is just telling me to spend more money
```

---
## \#15 Posted by: bartroosen12 Posted at: 2019-05-30T14:27:03.821Z Reads: 34

```
I should actually not buy the 6S version
The 10S version would be much more efficiënt and for a AT build 10S would be much better, because it will require to pull more amps than a normal esk8.

I think you are better of with buying 2 of these batteries and putting them in series:
https://hobbyking.com/en_us/turnigy-5000mah-5s-30c-lipo-pack-xt-90.html?gclid=Cj0KCQjw_r3nBRDxARIsAJljleHBnUZ3LCfwxhi-23yG-sG7ctGksMMNtJldaWaU6W_UV-SibhEx_BAaApTGEALw_wcB&gclsrc=aw.ds

It will cost you the same and it will be healthier for the battery.
```

---
## \#16 Posted by: infiniteoffset Posted at: 2019-05-30T14:41:11.659Z Reads: 31

```
12C means 12 times it's capacity. Since this lipo is 12Ah, total current will be 144A which is more than enough.
```

---
## \#17 Posted by: infiniteoffset Posted at: 2019-05-30T14:48:43.610Z Reads: 30

```
Tried to search for some info here on forum, two disadvanteges of lipos seem to be energy density and form factor. Are there any other reasons to go for a liion?
```

---
## \#18 Posted by: bartroosen12 Posted at: 2019-05-30T15:21:25.900Z Reads: 28

```
Like @Andy87 said the C-rating is not always correct.
If you try to find a max 'safe' current for a lipo you can better devide the C-rating by 2.

I made a 6S2P battery with 20C 5Ah cells. So it should be able to handle 20C*10Ah=200A I tought first. My esc only pulled max 100A.

After riding 5min on fullspeed (40-45km/h), I have no idea how many amps I pulled but it must be for sure below 100A. Some of my batteries were swollen and pretty hot, so I rode back home and they cell voltages were very unbalanced (3,4V - 3,7V).
So just to say this battery was even not strong enough, while I thought it would be absolutely no problem according to their C-rating.
```

---
## \#19 Posted by: wafflejock Posted at: 2019-05-30T15:21:33.383Z Reads: 28

```
No issue with using lipo really.  Would take Max C rating with a grain of salt though, the higher internal resistance of a battery and the larger the load or current draw the more voltage will dip until the load is reduced.  That said in our case there is usually only a brief period of high amp draw during acceleration and relatively high charge current when using regen braking (assuming you aren't a large rider or in a very hilly area).  I've also read some things about the lithium ion 18650 package stopping the expansion when gas builds in the cell which can apparently help with cycle life, on the other hand much cheaper and generally easier to replace lipos.
```

---
## \#20 Posted by: Wilsonliang777 Posted at: 2019-05-30T15:32:35.918Z Reads: 27

```
I have been using these for a while and I found it to be pretty good.  I hooked 4 of the 3s together to make a 12s pack.  I also did a 9s pack on these too.    It's rated at 25c but I dont trust the c rating.  I set my vesc to battery  to 50amp only.  $20 a pack is super cheap
![Screenshot_20190530_082636|233x500](upload://u6TuoFBdFbnFIkQUZtTfnAYcGLx.jpeg)
```

---
## \#21 Posted by: infiniteoffset Posted at: 2019-05-30T15:55:17.416Z Reads: 23

```
I agree that C-rating is not correct, but it should still have high current.

It's strange that you were able to pull only 100A out of your lipo. I don't think that the lipo was limiting factor, because if you short the battery, even small 1500mAh lipo will give you over 200A. Of couse pulling this current will permanently damage the battery, but it is possible.

Thanks for sharing your experience, I though that lipos can handle high current without a problem. Discharging battery in 5 minutes means that you were pulling 12C on average, meaning 120A on average. That battery was most definitely false labeled. Lot of cases where there are different specs written on the wrap than on the cells when you take the wrap off.
```

---
