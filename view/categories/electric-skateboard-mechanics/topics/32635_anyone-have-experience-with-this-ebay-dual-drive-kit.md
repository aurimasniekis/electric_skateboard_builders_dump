# Anyone have experience with this eBay dual drive kit?

### Replies: 14 Views: 1464

## \#1 Posted by: NickTheDude Posted at: 2017-09-08T16:55:03.126Z Reads: 167

```
http://www.ebay.ca/itm/DIY-dual-1500W-electric-longboard-drive-kit-83MM-wheel-7-trucks-CNC-mounts-/322549102279?hash=item4b196cb6c7:g:I0UAAOSwbtVZOttQ

Since it's so cheap I figured I'd buy it to test some stuff out. Plan was to try and rewind them to lower the kV, hook them up to VESCs on 10S and slap some Abec11s on em.

If you've got these, what is the gear ratio and belt width? Also is the wheel pulley removable? In the description it says "wheel pulleys are enbeded with theels" not entirely sure what that means...
```

---
## \#2 Posted by: Rinzler Posted at: 2017-09-08T17:02:05.532Z Reads: 161

```
The riptide electric skateboard uses it, so they should be good. https://www.google.hr/imgres?imgurl=https%3A%2F%2Fs.aolcdn.com%2Fhss%2Fstorage%2Fmidas%2Fe8b5e254aee3df1fccdebf71437bd025%2F205615245%2Feng-riptide-5JT.jpg&imgrefurl=https%3A%2F%2Fwww.engadget.com%2F2017%2F08%2F30%2Friptide-power-packed-electric-skateboard%2F&docid=Vyq4SjGG1ncJkM&tbnid=9v0AqoaRk0nijM%3A&vet=10ahUKEwju1_7Gh5bWAhVHPBoKHd4eAr8QMwg4KBAwEA..i&w=1600&h=978&bih=735&biw=1517&q=riptide%20electric%20skateboard&ved=0ahUKEwju1_7Gh5bWAhVHPBoKHd4eAr8QMwg4KBAwEA&iact=mrc&uact=8
Riptide has abec wheels, so they should fit.Maybe you dont need to rewind, just connect it so it is star aka delta.Drops the kv by 1.7, more Torque.
```

---
## \#3 Posted by: NickTheDude Posted at: 2017-09-08T17:34:03.804Z Reads: 147

```
Yeah I figured it was the same kit as the one on the Riptide. So I guess that answers the question about switching wheels.

[quote="Rinzler, post:2, topic:32635"]
just connect it so it is star aka delta.
[/quote]

Could you elaborate on that? I thought you had to rewind the entire motor to switch it from delta to wye.
```

---
## \#4 Posted by: Rinzler Posted at: 2017-09-08T18:24:45.617Z Reads: 132

```
<img src="/uploads/db1493/original/3X/b/c/bc52f5fa882696913bf196f6cc67a0f5f6a50f8b.png" width="620" height="315">
This picture explains everything, i didnt try to do this but apperently it is really easy.
"The three end wires can be soldered together for a Y configuration for the most torque and less rpm, or attach each end wire to one of the other two starting wires for a high speed low torque setup."
```

---
## \#5 Posted by: Rinzler Posted at: 2017-09-08T18:37:45.123Z Reads: 124

```
I mean, if you want to rewind the motors you could do that but this should work so you have nothing to lose i guess. I need to rewind my burned out 5065 270kv and i cant get the stator off the motor screw plate, and it is proving to be a pain..
```

---
## \#6 Posted by: NickTheDude Posted at: 2017-09-08T19:59:26.697Z Reads: 112

```
Sounds good, I'll probably give that a shot at some point, thanks!

And if anyone was wondering, I got a response from the seller and the wheel pulleys can be removed, the belts and pulleys are 15mm wide and gear ratio is 12:36.
```

---
## \#7 Posted by: Cobber Posted at: 2017-09-08T20:33:23.245Z Reads: 102

```
I haven't seen it done like that before LMT put 6 electrical binding posts on some of their motors so you can either use their pre made saddles or [solder them up with wire](http://www.lehner-motoren.com/doc/man_30_series_en_11_2013.pdf) to get either config... pretty cool :sunglasses:

http://www.lehner-shop.com/images/product_images/info_images/7_4.jpg

http://www.lehner-shop.com/images/product_images/info_images/60_0.jpg

I wish my motors had solid posts to attach flexible wire to rather than inflexible wire :(
```

---
## \#8 Posted by: Rinzler Posted at: 2017-09-08T21:12:49.679Z Reads: 95

```
 @NickTheDude Great, china is taking over. Bad news for eu suppliers, i hope this forum wont be for fixing china eboards that rookies buy. Make sure to update us on the kit.
 @Cobber  Soo cool, so it should work as the three delta wires are split and bridged into wye on the same side, leaving three thinner wires as A, B, C.
```

---
## \#9 Posted by: Greenie Posted at: 2017-09-18T11:44:51.012Z Reads: 74

```
I ordered it, just trying to figure out which VESC to get. But I can let you know how it runs if you want.
```

---
## \#10 Posted by: NickTheDude Posted at: 2017-09-18T12:21:09.429Z Reads: 74

```
Same, I should have a set coming soon. I got 2 TB VESCs. Their not the best in the world but I'd imagine you'd run into a bottleneck at the motor before the VESC so they shouldn't be working too hard.
```

---
## \#11 Posted by: pat.speed Posted at: 2017-09-18T12:28:51.919Z Reads: 72

```
Hey man this is a bit off topic but if I want to change my motors stator from delta to wye how would I do this? I though I new but then your LMT post and the picture the other person posted look different and I got confused. Could you help me out with a quick pick or something, thank you
```

---
## \#12 Posted by: Cobber Posted at: 2017-09-18T12:45:34.399Z Reads: 67

```
hit the link on the post pat, did you scroll down? I found [this calc](http://www.bavaria-direct.co.za/scheme/calculator/) great for me visualizing the wind and what connected with what.

edit: not sure on your motor but try 12 slot 14 pole 2 layer Y... then D
```

---
## \#13 Posted by: Greenie Posted at: 2017-09-18T12:49:55.914Z Reads: 65

```
Not sure what you mean, can you explain? I understand the TB are very good.
```

---
## \#14 Posted by: NickTheDude Posted at: 2017-09-18T12:58:07.255Z Reads: 64

```
Yeah, his VESCs are pretty good, not on the same level as a ollinboards heatsunk vesc or a focbox though.
```

---
