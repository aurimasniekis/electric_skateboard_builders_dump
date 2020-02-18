# Build a 12s5p battery pack for the first time

### Replies: 22 Views: 1436

## \#1 Posted by: Shippo Posted at: 2018-03-23T01:34:09.177Z Reads: 239

```
Hi,
It's my first time to post something here ~ and I'd like to know some suggestions about building my first 12s5p battery pack. 
I want to make this pack as flat as possible. Here's my plan.
![IMG_4077|666x500](upload://lF98vgRjvmPGtKT3h3pMyCE3HyD.JPG)
![IMG_4078|690x387](upload://zyfnGDObB8hBKimCG2KCPUn6n8L.PNG)
First, sorry for my bad drawing skill. 🙈
Will connecting 10 batteries with a single long nickel strip cause any problem?
Is it better to weld multiple layers of nickel strips?
Is this configuration possible to cause any problem like changing with BMS? And the negative cable will be much longer than the positive cable.
Thanks for helping me out🙏. I'm planning to use dual 6374 motors, TB's VESCs and Supower's 100A BMS.
```

---
## \#2 Posted by: b264 Posted at: 2018-03-23T01:40:38.762Z Reads: 229

```
A lot of problems you will have will be caused by HEAVY vibrations.  Think of everything in there as constantly moving around.  Everything rubbing and eating through the thing next to it...
```

---
## \#3 Posted by: myreala Posted at: 2018-03-23T01:42:12.290Z Reads: 226

```
One 10 mm width and 0.15 mm thickness Nickel strip may be fine for parallel groups(but I recommend 2 layers), but won't be enough for series connections. For series connections use 3-4 strips of 10mm width and 0.15 or 0.2 mm thickness Nickel strips. 
To make the pack flexible you can also solder 12Awg wire to connect series groups on the outside(where you marked weak points), this will also help with vibrations and reduce the need to use more than 2 layers of nickel.

Instead of using a single 12 awg wire you can also use two 14 awg wires per connection to make soldering easy on you.
```

---
## \#4 Posted by: Shippo Posted at: 2018-03-23T01:51:02.827Z Reads: 204

```
@b264 Thanks for replying.
Will it be much better after I use wires to replace nickel strip at weak point? And also will make it flexible.
```

---
## \#5 Posted by: b264 Posted at: 2018-03-23T01:54:27.621Z Reads: 203

```
[quote="Shippo, post:4, topic:49891"]
Will it be much better after I use wires to replace nickel strip at weak point? And also will make it flexible.
[/quote]

Yes, 10AWG silcone-insulated high-strand-count
```

---
## \#6 Posted by: Shippo Posted at: 2018-03-23T01:59:25.925Z Reads: 200

```
@myreala Thanks for the suggestions.
 I'm so glad I asked before I built it😊
Can I solder wires between nickel strips at the weak points before welding? I think I will only use wires to replace nickel strips to bridge serial connections. (At weak points)
```

---
## \#7 Posted by: myreala Posted at: 2018-03-23T02:05:14.011Z Reads: 188

```
It could work out as long as you have enough space to still spot weld after applying solder but I am not sure you can be that careful. I think it would be best if you do soldering after the welding. If you have solder hands that would be very handy but I did it without those. 
Also maybe use 10AWG wire instead of single 12AWG as you are looking at 100A, but you will need a very powerful solder to efficiently solder 10AWG. Maybe try two 12AWG wires per connection instead.
```

---
## \#8 Posted by: myreala Posted at: 2018-03-23T02:13:19.718Z Reads: 175

```
Also use sandpaper to sand down nickle surface before you try to solder on it or else it will take forever and use plenty of flux.
```

---
## \#10 Posted by: Shippo Posted at: 2018-03-23T02:21:12.245Z Reads: 172

```
@myreala  Ok!! Thank🙏
I’m worried about soldering after welding will make batteries be too hot.
Or maybe solder wires on double layers(or more) of nickel strips can protect batteries a little bit?
```

---
## \#11 Posted by: myreala Posted at: 2018-03-23T02:33:18.006Z Reads: 167

```
@Shippo  Which spot welder would you be using? If you are using something that can easily do multiple layers of Nickel then just spot weld everything. While using wires is a good idea, its massive headache as well. If you are going to be using the battery with a stiff deck you don't really need the flex anyways. Just leave some room in the enclosure for tiny amounts of flex so your battery doesn't flex when your board does.

And yes Nickel will protect the cells from Solder heat but only for a small time. Try to not leave the solder on for more than 5 seconds or so.
```

---
## \#12 Posted by: Shippo Posted at: 2018-03-23T03:31:13.976Z Reads: 155

```
@myreala I'm going to buy the Chinese one 788H on Amazon because it's faster and more simple to be delivered. I remember it can only deal with one layer of 1.5 mm pure nickel. Can I weld them layer by layer? 
Being flexible is always a good thing though 😊
```

---
## \#13 Posted by: myreala Posted at: 2018-03-23T05:44:02.411Z Reads: 139

```
I got the same one from amazon. I also did it layer by layer. But there is a trick to getting good weld strength. If you do second layer place one electrode on first layer and one on second layer to get a good weld. Placing both on second layer doesn't work well and you can just pull the second layer off. Doing this on positive terminal is very hard because you need to make sure that the weld tips only touch the center part where current can flow through the positive terminals surface or you'll get burn marks on Nickel strip. 
Using the same welder and that trick I did 0.15mm thickness and three layers of 7mm Ni strips.
```

---
## \#14 Posted by: pat.speed Posted at: 2018-03-23T05:47:58.752Z Reads: 121

```
You cannot solder before spotwelding. When you weld the strips the solder can melt.
```

---
## \#15 Posted by: Shippo Posted at: 2018-03-23T06:08:40.808Z Reads: 123

```
@myreala So it's better to weld on electrodes even doing the second and the third layer (since the welding spot is thick enough) ?
Right, it will be a big challenge for me to weld 3 layers on one positive terminal!
May I know your setting of the 788H?
Thanks.
```

---
## \#16 Posted by: Shippo Posted at: 2018-03-23T06:11:41.915Z Reads: 113

```
@pat.speed Thanks for your reminding. It's my first time and I really don't want to mess up
```

---
## \#17 Posted by: myreala Posted at: 2018-03-23T06:13:36.422Z Reads: 123

```
I meant place one weld tip on first layer of Nickel and second tip on second layer of Nickel, do couple welds like this. Always use foot pedal and try to get a weld when tips are touching Nickel at high pressure.
I don't remember my settings but I just got them from a youtube video. My current was around 8 on the knob I think. Don't remember the other one.
```

---
## \#18 Posted by: Shippo Posted at: 2018-03-23T07:01:43.649Z Reads: 124

```
@myreala I got you! Thanks for helping me a lot and sharing these infos. I'm so excited to do this and will share more in the future. It's so nice to meet you 👍
```

---
## \#19 Posted by: Shippo Posted at: 2018-03-24T04:16:31.253Z Reads: 111

```
@myreala This is my first try.
![IMG_4085|666x500](upload://cf8LKhutVMFx8H0n3i5flzBlu5X.JPG)
Should I avoid burn marks? I found out that I can easily pull strips off if current is not strong enough (no burn marks).
```

---
## \#20 Posted by: myreala Posted at: 2018-03-24T05:35:50.269Z Reads: 107

```
That may be bad, I don't know, but the burn marks seem a lot more visible than what I experienced. I would try to increase the pulse time while keeping current around 6-8 A to keep burn marks minimal. 

Take a look at [my pictures.](http://www.electric-skateboard.builders/t/edgerunner-sector-9-meridian-evolve-trucks-5065-140kv-custom-30q-12s4p-dual-focbox-psychotiller-enclosure/48089) 
I would say keep testing your settings and you don't seem to be using that trick I described. Maybe I fumbled it up trying to explain it.
```

---
## \#21 Posted by: Shippo Posted at: 2018-03-24T06:00:51.542Z Reads: 102

```
@myreala
![IMG_4088|690x387](upload://8yd0vZmxp93KlNpMsQwkOQP5ZqE.PNG)![IMG_4087|690x424](upload://p7L7LikQPbN0YmSIv4W0149921n.JPG)

I tried your way and it seems welded very solid. Only one thing I'm considering is sometimes I don't have space to do it. Sometimes under the single layer is the pink film of batteries, I don't want to melt them. 
I set the number to 80, 8A. Seems too high.
```

---
## \#22 Posted by: myreala Posted at: 2018-03-24T06:05:14.501Z Reads: 100

```
Attach the second strip a little sideways so you have room to do welds this way.
```

---
## \#23 Posted by: Acido Posted at: 2018-03-24T09:52:17.545Z Reads: 95

```
I would put 4 strips of nickel on the outer connections because thats where the current flows
```

---
