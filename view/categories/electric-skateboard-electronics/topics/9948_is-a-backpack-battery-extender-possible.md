# Is a Backpack Battery extender possible?

### Replies: 20 Views: 2294

## \#1 Posted by: Monte Posted at: 2016-09-21T18:12:14.497Z Reads: 189

```
Would it be possible to build a second battery pack with a Backpack to double the range?
I could try it if you guys say its possible. I have a Space cell 4 and a 10s2p (With bms) pack. I also got 20 cells from old laptop batterys. So theoretically it should be possible if i solder the 20 cells into the 10s2p pack, Put it into a nice shape for a little backpack and put it in Parralel with my board. I would modify a Anti spark to make it easyer to remove it so if i fall, the battery will be disconnected.
Could it even be possible to use a smaller or larger pack to extend the board?


<img src="/uploads/db1493/original/3X/8/6/86ef0c676b7f93736b5dca89817be3003ba8bbd7.png" width="690" height="328">
```

---
## \#2 Posted by: chinzw Posted at: 2016-09-21T18:19:46.667Z Reads: 184

```
If its parallel you don't need a loop key, since unplugging the extra battery wont open the circuit.
```

---
## \#3 Posted by: Monte Posted at: 2016-09-21T18:20:30.722Z Reads: 178

```
You are right i forgot that :D
```

---
## \#4 Posted by: Hummie Posted at: 2016-09-21T18:28:34.677Z Reads: 177

```
maybe the long battery wires will build too much inductance for the capacitors...maybe add some to the esc if you do this.  but carrying a long wire and likely having to add capacitors...why not just throw the extra pack under the board if you can fit it.
```

---
## \#5 Posted by: Monte Posted at: 2016-09-21T18:34:22.920Z Reads: 171

```
I dont want it under my board because it would increase the weight to much. I dont need that range all the time. I drive only two times a week to school (The rest of the week work ;)) and its not allowed to charge there.. What cappacitors are used with Vesc v4.12?
```

---
## \#6 Posted by: Mrmoonlight Posted at: 2016-09-21T18:41:42.954Z Reads: 161

```
Instead of a backpack with a cable, what about having the battery attach to the top of your board with velcro? You pop it on whenever you need it and store it in your backpack while riding. That will eliminate any need for long wires and the possibility of getting tangled up in them.
```

---
## \#7 Posted by: Monte Posted at: 2016-09-21T18:44:16.396Z Reads: 156

```
Hm that sounds good! I will try it and post the results here in a few days.
```

---
## \#8 Posted by: saul Posted at: 2016-09-22T04:53:51.090Z Reads: 134

```
I think it would be better to disconnect the space cell when you use the external pack. 

discharging two packs with different capacities, different age, different resistance probably wont work out well.

I would put a loop key on the external plug too. so you can disable it. don't want to have another spot that can get shorted.
```

---
## \#9 Posted by: Pathaim Posted at: 2016-09-22T11:54:23.509Z Reads: 113

```
couldn't you buy another space cell, keep it in your backpack and just swap and go when needed?
```

---
## \#10 Posted by: Monte Posted at: 2016-09-22T13:47:55.329Z Reads: 98

```
Swapable would not be good. The space cell is srew mounted under my board and that would be just too much work if im outside. I think will do it like @saul said, I put on on my board, so i dont have to put more resistors on my vesc. If the space cell is empty, i just switch it off and plug the second pack into the board.
```

---
## \#11 Posted by: treenutter Posted at: 2016-09-22T14:41:34.432Z Reads: 88

```
@Monte I'm interested in how you'd use this? A SC4 should get you pretty long range, are you riding in a way where you'll actually exceed it? I still appreciate the ingenuity here!
```

---
## \#12 Posted by: evoheyax Posted at: 2016-09-22T15:57:37.400Z Reads: 78

```
I've thought about this idea before. I would love to see someone try it!

What stopped me is what if you need to bail... Your physically connected to the board (your not getting that backpack off your back) if you gotta jump off. Other wise, I like the idea. My logic is why not build a 12s8p or some massive pack and run it from your backpack. Then, you would only need vescs in your board, and you could even move those to your backpack. hm....
```

---
## \#13 Posted by: chinzw Posted at: 2016-09-22T16:52:28.073Z Reads: 68

```
You would add too much resistance if you put that much wire between the vesc and motor.
```

---
## \#14 Posted by: Monte Posted at: 2016-09-22T17:29:10.770Z Reads: 63

```
Two times a week i drive to my school ~30km. But its not allowed to charge my board there. Dont ask my why.... My Teachers are rly closed minded people (Not my best english sentence :D )... And i ride a bit to aggressiv sometimes^^ Thats why i thinking about to upgrade with another 6374 in front or dual in back. I already have a plan to make them badboys both fit on the back truck ;)
```

---
## \#15 Posted by: Monte Posted at: 2016-09-22T17:30:49.229Z Reads: 67

```
I will build this guys and upload everthing here... But it will need some time because my soldering iron is broken at the moment -.-
```

---
## \#16 Posted by: 2-alex-2 Posted at: 2016-09-22T17:51:57.760Z Reads: 67

```
What I would do is have an extra xt90 plug inbetween the battery and esc but have a male and female on the top of the deck next to watch other and make a loop key out of a male and female. So when using the sp4 you use the loop key and then when you want to use the back pack you take the loop key out and use just the male that on the board leaving the female of the sp4 unplugged. <img src="/uploads/db1493/original/3X/3/c/3c1ddafaf9df0d21699db3e40dd371859bbc87bc.jpg" width="375" height="500"> 

That may help understand but that way they both get disconnected which every you decide to use.
```

---
## \#17 Posted by: treenutter Posted at: 2016-09-22T18:59:17.765Z Reads: 62

```
[quote="2-alex-2, post:16, topic:9948"]
So when using the sp4 you use the loop key and then when you want to use the back pack you take the loop key out and use just the male that on the board leaving the female of the sp4 unplugged.
[/quote]

I think that something is missing here... the loop key would only connect one + and one - connection, but you have it accepting four connections somehow.
```

---
## \#18 Posted by: 2-alex-2 Posted at: 2016-09-22T19:02:27.944Z Reads: 62

```
No like in picture have like a double one but acting like a loop key it's removable so the loop would have a male and female xt90. So in my picture there is 5 xt90 if that makes sense.
```

---
## \#19 Posted by: Hummie Posted at: 2016-09-22T19:09:03.722Z Reads: 63

```
the only thing i like to carry when riding is loose bills (no wallet or change) and the two keys to get back in my house.  no way I'd want to lug around bricks in a backpack.  at worst maybe stack them in the center top of the board.  having a long cord to a backpack, besides the increased inductance and need for more capacitors in parallel there's all the other obvious risks.  long motor wires I see and never heard of resistance problems with them.
```

---
## \#20 Posted by: im-done Posted at: 2016-09-22T20:34:05.306Z Reads: 59

```
I ised to run some 6s 8000 mah zippys in parallel and used a xt60 extention cord hooked you to my back pack worked great! Just every time i got off it would unplug and it was a pain in my ass.
```

---
