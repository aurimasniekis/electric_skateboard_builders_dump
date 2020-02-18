# Battery pack with BMS question - best way to split wires from BMS/batteries?

### Replies: 11 Views: 1565

## \#1 Posted by: Sebike Posted at: 2017-07-11T13:05:21.185Z Reads: 191

```
Dear esk8ers! 
Is there a standard, safe way you guys use for making the wiring/connections from battery /bms when you are splitting up to one charging and one discharging port? 
The battery wires will be coming off a nickel strip on a 18650 build and the other from a BMS where charge and discharge use the same connection P-. 
Couldn't find this explained on here.. 

Any help would be appreciated! 

<img src="/uploads/db1493/original/3X/8/e/8ee86f3b20c7d5d962b5eb6ad04d4b4880b1c48f.jpeg" width="690" height="388">
```

---
## \#2 Posted by: Okami Posted at: 2017-07-11T21:15:33.116Z Reads: 170

```
What u mean by safe? Otherwise.. very nice shematic (style)

U can always make a switch for charging, if you dont like.the idea about exposed "live" wires or just put a plug / cover, if u have one
```

---
## \#3 Posted by: Sebike Posted at: 2017-07-11T21:29:10.401Z Reads: 162

```
Thanks :slight_smile: What I meant was how do you connect two different wires to the same connection of a BMS board or battery etc. Do you just solder the two wires together and then solder them onto the board (P-) and/or nickel strip on battery pack. Or do you solder a single wire to the P-/battery and then use a splitter of some sort to attach the two wires (going to discharge and charge) to?
```

---
## \#4 Posted by: mmaner Posted at: 2017-07-11T21:30:07.871Z Reads: 154

```
Basically, wrap everything the pack and bms in kapton tape and heat shrink the total pack, then hot glue the little beast in place (on the board, not the enclosure) then pad the pack so that its snug against the enclosure.
```

---
## \#5 Posted by: Sebike Posted at: 2017-07-12T08:29:00.057Z Reads: 132

```
Thanks @mmaner. I can see that I was somewhat unclear in my first post, so I tried to be more specific about my question in post #3.
```

---
## \#6 Posted by: Sebike Posted at: 2017-07-12T10:07:45.749Z Reads: 124

```
Sorry about the extensive amount of topic edits. 😂
```

---
## \#7 Posted by: Okami Posted at: 2017-07-12T10:18:09.266Z Reads: 126

```
yeh, I hate the 'edit' mark also :D leaves a 'dirty' reply lol with many edits :D


Anyways.. yes you can add either 2 wires, or split the same wire later on..

Maybe a handy feature would be to install a connector there, so you can later dis-assemble all the modules and cables.. though, this depends on what your final location of these parts will be..

--

I dunno.. you should start assembling in your mind but I assume u havent done much work like this before so you dont know yet what methods might work for the problem / question zone u have right?

And with 'splitting the wire' = this means that you cut the isolation of the wire and make an exposure. Then, you take another cable you position it the same way and solder it onto the previous one, where the exposition is.

It is handy to apply heatshrink (if possible) before you do this.. Otherwise you might need to cover it up just with a tape or something..<img src="/uploads/db1493/original/3X/6/4/642b2820e4748f79686b349cb6f4b5e8eaadd503.jpg" width="690" height="388">

(not my picture) but you can get the concept with bullet connector in the middle.. you basically make 'Y' cable / harness..

I hope this makes it somewhat more easy to understand.. as im not even sure this is the direction you wanted some answers in :D
```

---
## \#8 Posted by: treenutter Posted at: 2017-07-12T10:59:02.839Z Reads: 118

```
[quote="Sebike, post:3, topic:27332"]
Do you just solder the two wires together and then solder them onto the board (P-) and/or nickel strip on battery pack.
[/quote]


@sebike for me, it depends on whether the P- is a contact pad or hole-through. If contact pad, I just solder them next to each other. If hole-through, I twist the exposed wire together and then solder as one connection through the hole.

As @mmaner points out, use kapton tape an heat shrink to cover up everything that's exposed.
```

---
## \#9 Posted by: Sebike Posted at: 2017-07-12T11:15:02.514Z Reads: 118

```
Thanks guys @Okami @treenutter. Those were the kinds of answers I was looking for :slight_smile: :+1:
```

---
## \#10 Posted by: JImmy2 Posted at: 2018-03-09T16:11:38.566Z Reads: 69

```
 hello guys i have 2 6s lithium batteries but i want to make one big 12s battery from them with just one bms , the good thing i think is the balance wires are connected to the of the batteries ( 2 6s bms ) but i dont know how should i connect the wires to the 12s bms . can anyone please help me ?
```

---
## \#11 Posted by: Redfire1 Posted at: 2018-04-23T21:21:35.078Z Reads: 55

```
@Okami ![image|375x500](upload://5DrLOx5jEy5Tf7WWbkhHsYPxEh1.jpeg)![image|375x500](upload://tS423BkwH32by7kLTxzDVeVEvEr.jpeg)![image|375x500](upload://B4GDDptr80b4WI9hDII92Dx4rR.jpeg)![image|666x500](upload://fW1svt2mE6xRfSiLTrUeV2vEwTs.jpeg)![image|374x500](upload://xQmbcPeELyq0xB4YKGCqqaGpYEp.jpeg)hi I don’t know if you could help,I connect my bms for my 2x5s lipo I connect B- to battery,C- to charger - P- to vesc - ,battery + to vesc plus Battery + to charger +,when I connect the vesc they don’t come on the voltage is about 11V so I have to take off the P- and connect it to battery- and then vesc would come on,charging it I am not sure it charge on the charger the light is always yellow.
```

---
