# Anyone using/used HTD3M 18/50 or lower and having/had teeth skipping?

### Replies: 17 Views: 1599

## \#1 Posted by: Pedrodemio Posted at: 2016-07-24T23:14:54.418Z Reads: 151

```
Hello guys, the title says all

On my new build no mater how much I tighten, in some situations the belt slip

I already have a mounting for a tensioning bearing to increase tooth in mesh, I just want to know if someone got a similar setup and avoided one more complication somehow

I thought that with 6 tooth I would be fine, guess I was wrong

Cheers
```

---
## \#2 Posted by: Michaelinvegas Posted at: 2016-07-24T23:23:49.899Z Reads: 149

```
Could just be the teeth are too small for your use or the belt itself just sucks

I'd get a different brand belt and see if that helps
```

---
## \#3 Posted by: JLabs Posted at: 2016-07-24T23:50:28.661Z Reads: 146

```
I would recommend switching to HTD5, it seems to be the standard on here, and I have had zero belt slips with a 14/36 gearing ratio..
```

---
## \#4 Posted by: Jinra Posted at: 2016-07-24T23:54:19.886Z Reads: 143

```
try calculating here. it'll tell you if you have too few teeth in mesh

http://www.bbman.com/belt-length-calculator/
```

---
## \#5 Posted by: chuttney1 Posted at: 2016-07-25T00:16:12.925Z Reads: 134

```
Basic rules for having a timing belt skip is tension on belt is not sufficient, few teeth in mesh as Jinra said, or motor is strong causing belt to skip. 

I have used 3M HTD and it worked for the power requirements I designed my eboard, but did it because I had tighter design specifications. 5M can handle more power transfer as this is what the community here uses majority.
```

---
## \#6 Posted by: XIII Posted at: 2016-07-25T00:30:49.710Z Reads: 127

```
is it a 9mm belt? 

I find it slipping on me a lot aswell.. Gonna upgrade to a 15mm.
```

---
## \#7 Posted by: onloop Posted at: 2016-07-25T02:31:43.373Z Reads: 120

```
at a minimum for 3mm pitch you should use 15mm wide belts. if its dual drive maybe 12mm will work.
```

---
## \#8 Posted by: chuttney1 Posted at: 2016-07-25T04:40:56.434Z Reads: 114

```
I used a 9mm belt. At the time of decision my goal was to use to use 2, 320Kv motors for dual motor drive. I changed it to a 149 Kv motor, but kept the 9 mm belt decision. I am going to get increased belt wear as opposed to using 10, 12, or 15 mm belt widths. I like compact and simple design.
```

---
## \#9 Posted by: Pedrodemio Posted at: 2016-07-25T23:05:24.233Z Reads: 104

```
I forgot some details, i'm using 15mm width, will try to find some better belts, but here in Brazil we don't have mane places to choose

I have 6 teeth in mesh, should be okay from my power and torque calculation, maybe i've missed something for low speeds

I chose to go 3mm to get the a bigger gear ratio and climb some steep hill around here, in this i'm good, i have yet to found a hill that i cant climb

I could try to tension even more, but the losses from friction will rise
```

---
## \#10 Posted by: Pedrodemio Posted at: 2016-11-11T19:17:24.174Z Reads: 85

```
Just a update, after looking at various manufacturers catalogs and calculating the the load on the belt, there is no way it was gonna work in my case, the load was on the limit of what the HTD 3M can do, in all the tables i was in the zone of severely reduced operation life, worked for a time and then the belt started to wear until it brooke the internal reinforcements, boosted got way with it because two things in my opinion:

1 - a very well made and centered motor pulley that guarantees a constant belt tension across all motion range 

2 - lower torque being transmitted, some tear down's state that their esc is 30A per channel, that would be, under ideal conditions a max of 0,15 N.m on the motor side, in my case i was trying to transfer 0,28 N.m

Now, using the same belt path with HTD 5M i can use the belt very loose and still have to manage to make it slip

The thing that i miss is that the 3M have a considerably lower drag, in a dual setup and with a lower reduction (lower motor Kv/more teeth in the motor pully) it probably would work
```

---
## \#11 Posted by: mmaner Posted at: 2016-11-11T19:55:33.157Z Reads: 73

```
Thats what I started with, it slipped on every hill.  I went to a 5M and the slipping went away.
```

---
## \#12 Posted by: RenBrant Posted at: 2016-12-19T11:07:14.025Z Reads: 68

```
Hi Pedro,
I'm from Brazil too.
Are you buying parts for esk8 locally or are you importing?
```

---
## \#13 Posted by: Pedrodemio Posted at: 2016-12-19T14:30:35.803Z Reads: 61

```
Depends, I will list what I got here what I imported

Brazil:
-Pulleys/Belts
-Trucks
-Wheels
-Miscelaneous eletronics (arduino/radio module
-Deck
-Hardware
-Some wires, it was cheaper from china but I didn't wanna wait
-Motor mount(I designed and sent to be fabricated)

The rest imported, basically the motor, vesc and batteries, that even if you want you can't find here
```

---
## \#14 Posted by: Guilherme Posted at: 2016-12-21T01:03:20.296Z Reads: 54

```
Hi guys, I'm from Brazil too..
Pedro where did you bought the pulleys and belt?
```

---
## \#15 Posted by: Pedrodemio Posted at: 2016-12-21T02:55:37.526Z Reads: 48

```
I will create a topic for it, probably there's more people arround from here
```

---
## \#16 Posted by: SolidSurfer Posted at: 2016-12-21T03:43:44.908Z Reads: 50

```
I've thought about Boosted getting away with 3M too, and wonder how much it might have to do with supporting the wheel pulley with the bearing on the hanger. The 3M tooth profile is pretty small, and just a little give from being unsupported would lead to slipping IMO.

I'm wanting to go 3M because of the reasons you mentioned, plus you end up with so much more clearance - 3M/50T is so much smaller than 5M/36T.

Planning to support the wheel pulley with a bearing on the hanger.

Will report back...
```

---
## \#17 Posted by: Pedrodemio Posted at: 2016-12-21T03:59:25.642Z Reads: 45

```
I've used a bearing supporting the pulley, good luck, in the near future I plan to go dual motor and will try again, limiting the current on the motors and maybe using 20T on the motor, and more important, sent the pulley to be custom made using wire EDM in steel, aluminum wears to quickly and make the problem worse
```

---
