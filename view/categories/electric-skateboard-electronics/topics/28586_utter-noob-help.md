# Utter noob help

### Replies: 18 Views: 1263

## \#1 Posted by: Gynpe Posted at: 2017-07-25T12:19:04.480Z Reads: 141

```
Hey guys new builder here, with lots of confusion regarding batteries.

I'm currently waiting on my deck and trucks to arrive on the mail, and should have a FOCBOX inbound sometime in August thanks to @monkey32 props to him.

However I'm in serious doubt regarding batteries, because I simply do not know what to buy. But I do know that I want to make the actual battery packs with 18650's to get the whole experience of building, instead of buying Lipos from HobbyKing.

So my build will have a FOCBOX speed controller, and was thinking of this motor https://www.horizonhobby.de/en/p/dymond-gtx-6374.htm?a=article&ProdNr=03121773&p=43793 in particular because of a Trampa build I saw on YouTube by Jens Kappel which made me fall in love (if i enjoy the experience I plan to get another motor and a trampa board for a similar build).

This first build however will be a single motor build on a normal longboard with 90mm wheels. I've read the Battery Build Guide post, but I still don't get it.

Just how many batteries do I need? With how many mAH? And is 30A too much? Also, how do I determine the BMS needed... If I even need it?

Anyway, thanks for your patience in advance. 

Oh, and as far as range and speed 25-30km and 25-30 kph is good with me.
```

---
## \#2 Posted by: aigenic Posted at: 2017-07-25T16:43:17.234Z Reads: 124

```
10S4P Samsung 25R cells...3,7*10*2,5*4=370Wh That should give you more than 25 kms
10S4P LG 30Q cells...3,7*10*3*4=444Wh Even more range :O and the 30W 18650's are better but more expensive...

You need the BMS...I cant give many advices about this one, but if you use 80A 10S BMS with intergrated switch you should be ok :)

I do not recommend you to try 12S battery pack, because the motor is 200kv and you would exceed the ERPM limit of the VESC...
```

---
## \#3 Posted by: psychotiller Posted at: 2017-07-25T17:50:07.734Z Reads: 105

```
If you've already bought the FOCBOX you should buy a motor that is sensored. Not sure if the one you linked here is. It would be a shame to not use the functions available to you with an unsensored motor.
```

---
## \#4 Posted by: Jedi Posted at: 2017-07-25T19:35:51.112Z Reads: 93

```
As a new builder with lots of confusion, do yourself a favor and buy a premade 18650 pack. There are members who will build you one at a fair price. Building your own would be a rich learning experience, but mistakes can have serious consequences. Any new builder should leave the battery building to the pros.
```

---
## \#5 Posted by: Gynpe Posted at: 2017-07-29T04:21:31.419Z Reads: 79

```
Hey guys, sorry for the late reply and thank you for your help

@aigenic will this do https://eu.nkon.nl/rechargeable/18650-size/samsung-inr-18650-30q-3000mah.html ?? 

and this http://bestechpower.com/37v10spcmbmspcbforli-ionli-polymerbatterypack/PCM-D223V1.html ?

@psychotiller I wrote the guys that sell the motor I mentioned and waiting for a reply regarding the matter. If it its not sensored, do you have any recomendations? I ask this in case there is a more optimal option. I'm in EU by the way.

@Jedi I know I'm a padawan right now, but I'm determined to do this... It just looks too fun. I do appreciate your advice however. At any rate, can you point me towards someone willing to build me one just in case I change my mind? 

Thanks all!
```

---
## \#6 Posted by: Jedi Posted at: 2017-07-29T05:11:49.617Z Reads: 76

```
Go for it. All the info you need is here or elsewhere online. May need a spot welder. 

@barajabali has been building some impressive packs.
```

---
## \#7 Posted by: aigenic Posted at: 2017-07-29T05:26:26.677Z Reads: 71

```


@Gynpe Get a higher discharge cells :) 15A is quite a lot, but with higher higher discharge rating the batteries wont sag that much :) I dont use LiIons so i cant advice you much, but from what I have read, higher discharge is always better :)
```

---
## \#8 Posted by: Jinra Posted at: 2017-07-29T05:29:10.188Z Reads: 66

```
30Q's are very well regarded here and are a favorite of li-ion users. they will be fine. They can handle 20A continuous despite their specified rating.
```

---
## \#9 Posted by: Gynpe Posted at: 2017-08-02T14:56:08.644Z Reads: 52

```
Hey guys, 

Been reading quite a few these days, and all there is left to purchase is the battery pack and the motor. I've decided to go with the Alien Power System 6473 170kv Sensored motor. 

I guess I'm just looking for confirmation from your guys to see if its a good choice to go with 10S4P pack and FOCBOX controller.

Thanks!!
```

---
## \#10 Posted by: Jinra Posted at: 2017-08-02T15:03:46.788Z Reads: 50

```
Yep, that'll work fine. Just be aware that the sensor labeling on the FOCBOX is wrong so be sure not to hook them up wrong.
```

---
## \#11 Posted by: Sebike Posted at: 2017-08-02T15:17:30.995Z Reads: 49

```
Just a heads-up.. That motor has a 10mm shaft that will require a similar sized bore on the motor pulley. You will find those pulleys on APS and/or Esk8.de, but 8mm bore pulleys are more common.
```

---
## \#12 Posted by: Gynpe Posted at: 2017-08-02T20:19:44.503Z Reads: 44

```
Just placed the order... I'm psyched here!

Thanks all!

Now on to further reading...
```

---
## \#13 Posted by: sl33py Posted at: 2017-08-02T21:00:22.070Z Reads: 45

```
FOCBOX and 10s4p will work great.

Also second @Sebike - make sure you get a 10mm motor gear from APS when you get the motor.  THey can be a PITA to find otherwise and usually steer folks to 8mm shaft motors.

I'd also suggest (if you haven't already grabbed trucks and motor mounts) - to get Caliber II trucks and mounts vs Paris or any round mount.  Save yourself some frustration.

Still make sure you Loctite all your wheel gear bolts and bolts securing the motor mount!

GL!
```

---
## \#14 Posted by: Gynpe Posted at: 2017-09-04T09:18:39.465Z Reads: 42

```
I never replied @sl33py, but I ordered as you advised. Thanks man!

Also, I'm not going to be able to do the battery pack just yet... Perhaps later this month, and I happen to have all the components except for the battery.

I'm really thinking of getting a couple lipos from hobbyking or amazon, or whoever sells the cheapest, and going parallel.

I was thinking 3x 5000 mAh 20c lipos, but I haven't read about how they work or what I need, or if they are sufficient for my build (APS 6374 170KV and FocBox).

I also I have an Imax b6 charger... Will it do to charge the three packs? 

Can someone shed some wisdom on the matter?

Thanks!
```

---
## \#15 Posted by: darkkevind Posted at: 2017-09-04T11:08:00.185Z Reads: 39

```
Do yourself a favour and use my handy tool to find the best Li-ion for your needs.

http://kevindark.co.uk/PublicServices/NkonFilter

And build yourself a DIY battery spot welder (like this one I built) for a pinch and weld up your own li-ion pack ;)

https://www.youtube.com/watch?v=o4NaDMoEHxU
```

---
## \#16 Posted by: hornet90 Posted at: 2017-09-04T12:55:50.519Z Reads: 35

```
Look at this set up 
http://www.electric-skateboard.builders/t/high-power-10s-lipo-battery-pack-with-bms/10014?u=hornet90
```

---
## \#17 Posted by: hornet90 Posted at: 2017-09-04T12:57:54.609Z Reads: 35

```
http://www.electric-skateboard.builders/t/irish-shamrock-build-no2/23997/29?u=hornet90
```

---
## \#18 Posted by: sl33py Posted at: 2017-09-04T22:10:11.210Z Reads: 31

```
[quote="Gynpe, post:14, topic:28586"]
I also I have an Imax b6 charger... Will it do to charge the three packs?
[/quote]

iMax b6 (B6ACv2?) - will work great.  It will only charge up to 6s, so you'll need to likely charge individually, or in parallel.  If you do charge in parallel i would periodically charge individually to make sure none of the cells get out of whack (too far voltage delta from the rest).  Good inexpensive charger to get started.

If you are "thinking" of those batteries - i'd suggest you get their slightly "beefier" big brothers - the 5000mAh 30c cells, or similar - higher output capacity, so less sag under heavy load.

GL!
```

---
