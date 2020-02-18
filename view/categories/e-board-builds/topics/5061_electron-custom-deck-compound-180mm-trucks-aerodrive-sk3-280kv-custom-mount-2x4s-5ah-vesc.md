# Electron &#124; Custom Deck &#124; Compound 180mm Trucks &#124; Aerodrive SK3 280kv &#124; Custom mount &#124; 2x4s 5Ah &#124; VESC

### Replies: 18 Views: 2861

## \#1 Posted by: Monstercrunch Posted at: 2016-06-23T21:41:15.577Z Reads: 256

```
Hi all !

It's time, I'm building my electric board ! :slight_smile:

About me (shortly): french maker, new to riding stuff (I own a penny like since last month but felt in love with the way we move with those things :heart_eyes: )

About the board:

It's my first one, here is the stuff I plan to use. Feel free to comment and give advices :slight_smile:

- **The board** : I'm going to make a custom board, with this kind of shape
![Deck photo](http://i35.servimg.com/u/f35/13/84/06/30/planch10.jpg)

- **The trucks** : Compound 180mm Trucks
![Trucks](http://i35.servimg.com/u/f35/13/84/06/30/trucks10.jpg)

- **The wheels** : 72 mm D-Street longboard Wheels Fly 78A
![Wheel](http://i35.servimg.com/u/f35/13/84/06/30/wheel10.jpg)

- Motor: Turnigy Aerodrive SK3 - 5055-280kv
![Motor](http://i35.servimg.com/u/f35/13/84/06/30/1817510.jpg)

- **Batteries** : 2x ZIPPY Flightmax 5000mAh 4S1P 20C in series (8s equivalent)
![Battery](http://i35.servimg.com/u/f35/13/84/06/30/batter10.jpg)

- **Pulley and belt** :
 Pulleys will be 3D printed (15 and 36 teeth), and I choosed a 265mm HTB belt for an approximative 65mm C.

- **Battery charger** :
   Not chosed yet. If you have a reference for good 6s one (I read that I can charge my two 4s in parallel that way), not too expensive :)

- **Motor controller** : 
I'd like to start with an normal ESC for budget reasons... Is it a bad idea or is it ok to start with ? It's less than half the price of an homemade VESC, but is it really half the quality ?

- **Remote** : probably a nunchunk hack. Any comment on the reliability of this method ?

I'll update the topic as I build it, with a lot of pics of course ! Feel free to comment my choices :wink:

Monster.
```

---
## \#2 Posted by: Maxid Posted at: 2016-06-23T21:47:39.348Z Reads: 241

```
1) don't print the motor pulley
2) There are basically no ESCs for 8S that are cheaper than a VESC. If you want to go 8S you will need a VESC or you go for 6S and use a normal car ESC.
3) discharging as 8S and charging as 4S in parallel is also not easily done.
4) Nunchuck hacks are bad - use a GT2B with mad munkey mod instead
5) The wheels will be hard to mount the pulley on
6) same for the trucks - everyone uses caliber trucks to mount the motor on.
```

---
## \#3 Posted by: shred Posted at: 2016-06-24T17:52:06.462Z Reads: 213

```
[url=http://www.ebay.fr/itm/HTD-5M-15T-16W-5-6-6-35-8-10mm-Bore-Pitch-5mm-Timing-Belt-Drive-Pulley-15-Tooth/252402866384?_trksid=p2045573.c100033.m2042&_trkparms=aid%3D111001%26algo%3DREC.SEED%26ao%3D1%26asc%3D20140423084956%26meid%3D0d728cddd6e24b55a1edae3aa9b49abb%26pid%3D100033%26rk%3D2%26rkt%3D8%26sd%3D262150819891"]Motor Pulley: you can order these on ebay.fr[/url]
```

---
## \#4 Posted by: Monstercrunch Posted at: 2016-06-25T11:53:26.713Z Reads: 205

```
Thanks for the advice :)

1) I'll buy a metal one for the motor pulley, but I'll try the 3D print anyway, just to test
2) Ok, didn't know you couldn't find ESC for 8s...
3) Is it that complicated ? I thought I just needed to have a series connexion on the board and a parallel on the charger. Maybe I'm missing something ?
4) Noted !
5) It's just 4 holes... ;)
6) I'll make a custom fixation

I know I didn't choose the easiest way to build my board, but for me the interesting part in this project is the "making" part. Where is the fun when you buy plug and play kits ? :p

Any idea for the lipo charger ?

Thanks again for those tips :)
```

---
## \#5 Posted by: Monstercrunch Posted at: 2016-06-25T14:47:19.580Z Reads: 193

```
For the charger, I've been looking around and that's what I understood:

- if I want to charge my two 4s batteries in series (ie I don't have to change my wiring from when I use them in series), I need a 8s charger (more expensive, but with 150w I'll charge my batteries faster) : [44€ Turnigy Accucel-8 (150w)](http://www.hobbyking.com/hobbyking/store/uh_viewitem.asp?idproduct=31867)
- if I charge my two 4s in parallel, I need to change the wiring to parallel and I can use a 4s charger like this: [16€ Imax B6 (50w)](http://www.ebay.fr/itm/Neuf-iMax-B6-LCD-LiPo-NiMh-LiFe-Balance-Batterie-Chargeur-Battery-Charger-/300879515979?hash=item460dd1114b:g:zSgAAOxy14VRTDGR)
- or use 2 Imax B6 to charge my two batteries at the same time :p (still cheaper than the Accucel-8)

Am I right ? I guess you would consider buying the Accucel-8, even if it isn't wallet friendly :(

If you have other charger references just let me know !

[EDIT] For the records, I read this very good article on parallel charging : http://www.rchelicopterfun.com/parallel-lipo-charging.html
```

---
## \#6 Posted by: Monstercrunch Posted at: 2016-07-01T17:20:09.796Z Reads: 181

```
Hi, little update :slight_smile:

Almost ordered everything, waiting to receive the parts.

I have a question about flat wires, cause I'd like to  separate batteries and VESC/Motor space like on the boosted board.

The question is:  : which dimensions should I choose ?
And this lead to my second question: how many amps usually flow out of the batteries ?

My motor (which is a turnigy aerodrive sk3 280kv) says "Max Loading: 60A". Should I use this information to choose my wire ?

Thanks in advance :slight_smile:
```

---
## \#7 Posted by: Monstercrunch Posted at: 2016-07-03T22:04:02.254Z Reads: 169

```
Little update, the deck is drying : 

![Deck](http://i35.servimg.com/u/f35/13/84/06/30/deck10.jpg)

My last question still accept answers ;)
```

---
## \#8 Posted by: Stevemk14ebr Posted at: 2016-07-03T22:18:08.490Z Reads: 163

```
Most people here use 12awg wire. This is what my 80a 230kv from torqueboards came with so i imagine you would be good with that.
```

---
## \#9 Posted by: lox897 Posted at: 2016-07-03T22:32:07.869Z Reads: 167

```
Changing the SK3 wire is a PITA. It has an enamel coating around it.
```

---
## \#10 Posted by: Monstercrunch Posted at: 2016-08-01T23:32:25.407Z Reads: 154

```
Hi there ! :slight_smile:

I've been working on my board without uploading updates here, time to catch it up a little bit:

**The board**
![The board 1](http://i35.servimg.com/u/f35/13/84/06/30/receiv10.jpg)
![The board 2](http://i35.servimg.com/u/f35/13/84/06/30/receiv11.jpg)
![The board 2](http://i35.servimg.com/u/f35/13/84/06/30/receiv12.jpg)

**Homemade VESC** <- pretty proud of the result, not tested yet ^^'
![VESC](http://i35.servimg.com/u/f35/13/84/06/30/img_2010.jpg)

Also, I'm actually making an adapter to wire my two 4s lipo in series. I made a pcb to create a 9pin connector from the two 5 pin connectors, however one of the trace has melted when I plugged it to my charger :X How many amps are going through those balance wires ? I'm pretty sure my wirering was good, I don't think I made any short cut :/ I guess the current was to high...

If you want to check the typon:
![Typon](http://i35.servimg.com/u/f35/13/84/06/30/captur10.png)

Any idea why it melted ? (I'll add pics tomorrow)
```

---
## \#11 Posted by: Maxid Posted at: 2016-08-02T06:45:11.820Z Reads: 139

```
how were your main lines connected?
<img src="/uploads/db1493/original/2X/5/5f3ab1f4619b97759d4beabe1917fe9ca6a25db1.png" width="574" height="265">
```

---
## \#12 Posted by: Monstercrunch Posted at: 2016-08-02T17:33:21.081Z Reads: 141

```
I may have connected it wrong... I don't remember but I may have kept the 9pin connector with red on the right side and black on the left (with your picture as a reference).

Here the short (on the left). 

![Shortcut](http://i35.servimg.com/u/f35/13/84/06/30/shortc10.jpg)

As you can see I already had fixed it one time cause the trace melted when I tested connexions with my ohmmeter  u_u

I'll make a second version of the pcb and test it again, I'll keep you informed, thanks for your help :)
```

---
## \#13 Posted by: Monstercrunch Posted at: 2016-08-04T06:22:42.131Z Reads: 122

```
Well it works :) I pprobbly connected it wrong last time. Didn't change anything.

Now I'm trying to flash my vesc with an st link V2 but the thing can't talk to the target :'( Openocd is telling me that the target voltage is at 0,8V which I think is abnormal. And when I plug the vesc usb to power it (that's what I think it would do), it becomes 0V. I'll dig a little that way, check my soldering etc..
```

---
## \#14 Posted by: Monstercrunch Posted at: 2016-08-21T19:35:33.873Z Reads: 120

```
Hi, little update :slight_smile:
Just mounted the motor on the truck. It was a pain in the a** !!  :rage: The truck has a weird shape... At least now I know I'll never go again for something similar ^^

Also my wheels seem to be a little bit short, the structure can easily touch the ground :/ I'll probably change it for bigger ones or modify the structure. 

Some pics, enjoy :slight_smile:

http://i35.servimg.com/u/f35/13/84/06/30/motor_11.jpg

http://i35.servimg.com/u/f35/13/84/06/30/motor_10.jpg

http://i35.servimg.com/u/f35/13/84/06/30/motor_12.jpg
```

---
## \#15 Posted by: whitepony Posted at: 2016-08-21T19:40:09.679Z Reads: 117

```
couldnt you mount the mount the otherway round? hey, that rhymes! :smile: like this you got this aweful long motor pulley construction that puts a lot of lateral load on your mount (and to be frank: your mount doesnt look like it could take that lateral load at all) and also a lot of extra torque on your motor shaft and motor bearings because of that really long lever.
```

---
## \#16 Posted by: Monstercrunch Posted at: 2016-08-21T21:15:20.957Z Reads: 113

```
Well, the thing is that the motor pulley's hole is too big for the motor axe. I've used an adapter given with the motor which fits perfectly in the pulley. But I agree I've a big lever here... I'll make some tests, will see if it holds :confused:
```

---
## \#17 Posted by: jujukrollou Posted at: 2016-10-11T19:23:56.594Z Reads: 67

```
Any update on your board ? I use the same motor than you but I am not sure on how to connect everything
```

---
## \#18 Posted by: Stefanowich Posted at: 2016-10-12T19:11:34.624Z Reads: 57

```
Update? :D
```

---
