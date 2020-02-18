# Carbon fiber electrical conductivity

### Replies: 16 Views: 971

## \#1 Posted by: krloz Posted at: 2017-08-25T10:24:36.965Z Reads: 195

```
Hello fellow board neards.
I have a question for the carbon fiber gurus. 
I have some experience working with fiberglass add I AGM planning on doing my first carbon battery enclosure.  But I have a bit of concern about having electricity conducting walls. 
My question is what do you people do about this issue
I have thought about aging a first layer (I am using a male mold with ghetto vacuum so the first layer would be in contact with the contents) of maybe fiberglass or cloth of some type but I'm not sure if this would affect the strength of the enclosure
Or maybe adding Some  cheap adhesive car sound proofing inside

Thoughts?   Thanks!!!!
```

---
## \#2 Posted by: Jinra Posted at: 2017-08-25T10:43:48.093Z Reads: 189

```
Calling @MasterCho!
```

---
## \#3 Posted by: itsmikeholland Posted at: 2017-08-25T10:57:26.707Z Reads: 185

```
i cant contribute much to your original question but just make sure you actually need carbonfiber vs fiberglass. Im not sure how well cf takes to flex stressing so just keep that in mind!
```

---
## \#4 Posted by: krloz Posted at: 2017-08-25T11:03:11.260Z Reads: 178

```
Flex and stress was my reason to try carbon instead of fg. And that is after reading carbon posts in the forum. 
New question any reason for fiberglass over carbon?
```

---
## \#5 Posted by: Cobber Posted at: 2017-08-25T11:24:04.006Z Reads: 166

```
depending on how the fibers are laid CF will or will not be flexy... if your'e good (know the fiber) you should be able to tune the flex to what you want. I haven't had a CF eSk8, but I've had paddles, bikes and wheels. Some have had no flex and some like the paddle was stiff in the butt but like a spring towards the blade that returned the energy in the second half of the stroke.
I have seen some of the builds here insulate the CF enclosure, I _think_ I have seen _whitepony_ use felt. Try searching some builds, I'm sure you will find several tested solutions.
```

---
## \#6 Posted by: pakue Posted at: 2017-08-25T11:34:39.819Z Reads: 154

```
I just checked the resistance on a CF strand (300mm length; roughly 30mg of mass) and it had around 50Ohm resistance, so its definitely conductive enough to cause quite a current flow in a mesh if connected to the battery. However in a case you've got multiple layers of epoxy resin above the CF, so I doubt it could cause any realistic issue.
```

---
## \#7 Posted by: krloz Posted at: 2017-08-25T11:41:55.080Z Reads: 147

```
Not above.  Layers of resin between the cf. And i can't be sure the first layer of carbon will suck enough resin to be isolated from the contents of the case

By the way.  I'm only doing a battery enclosure.  Not a full deck.  I'm going to look into builds and see if I find something
```

---
## \#8 Posted by: pakue Posted at: 2017-08-25T11:51:45.982Z Reads: 142

```
Don't you usually coat it again with another layer of resin after it has hardened? Otherwise you'll damage the fibers while sanding.

If I poke through the surface of my enclosure with the multimeter probes I sometimes get a reading, but its not very consistent. Are you planning on having the contacts of the battery open inside the enclosure?
```

---
## \#9 Posted by: i2oadsweepei2 Posted at: 2017-08-25T12:18:36.229Z Reads: 139

```
I built my entire enclosure out of fibreglass and used carbon fibre only around the flange where it gets bolted down. The enclosure is very strong with a layer of mat and a layer of cloth using west systems epoxy. You get the flexibility all over and the strength where you bolt it down. It's the second time I built an enclosure this way. If you are going for looks then you can't beat the awesomeness of CF. Maybe just insulate the insides with sound proofing as you suggested or maybe a few coats of paint. If you want a thing of beauty then you may just want to buy a master cho enclosure. I couldn't build one cheaper than he makes them. I would totally paint the inside though. It can also block the signals from your transmitter to your receiver. We learned this in our RC boats. It's why I wouldn't use a full CF enclosure. just my 2 cents. Good luck.
```

---
## \#10 Posted by: onepunchboard Posted at: 2017-08-25T16:32:48.366Z Reads: 126

```
I ve seen issue with cf using on drons racers. sometimes motor wire get loose and touches body where esc is bolted on. it can fry thing if not careful
```

---
## \#11 Posted by: i2oadsweepei2 Posted at: 2017-08-25T17:59:28.576Z Reads: 121

```
That's true. We had to use plastic standoffs and plastic screws when we mounted our flight controllers to a cf frame. I learned that the hard way with my flip32 foc. Thankfully they are only $30.
```

---
## \#12 Posted by: MasterCho Posted at: 2017-08-26T01:45:26.172Z Reads: 115

```
I would shrink wrap all the component and use thick Fiberglass as the last layer.

<img src="/uploads/db1493/original/3X/8/6/86cb338d642d19133cb0dde1f09a51d0ab788569.png" width="690" height="388">
```

---
## \#13 Posted by: krloz Posted at: 2017-08-26T11:53:27.270Z Reads: 86

```
Obviously the guru @MasterCho had what I wanted to hear.
 Inside layer of non conducting and the rest of the layers of carbon fiber.
Still digging the car soundproofing as it is still self adhesive and add padding. Still not puncture resistant which is what I didn't like

Just as an aclaration. This is an enclosure for under the board 10S lipo made of 2S packs and my vescs and receiver are above the board so not very worried about the signal blocking.  Still worth mentioning for anyone investigating carbon fiber in the forum.
On another side note. When I solder thick risky wires like the ones between lipo packs, I like to add a layer of abs sludge between  the solder and the heatshrink. For those of you who 3dprint you know what I'm talking about.  You dissolve abs plastic in acetone and get a marmalade like sludge. You apply it around the solder and when the acetone evaporates you get a solid layer of plastic around the solder
```

---
## \#14 Posted by: visnu777 Posted at: 2018-07-27T23:18:15.655Z Reads: 49

```
Just an example of what can happen: Today I rode around a bit with my new board, when I came home I wanted to check the voltage and when I plugged in my antispark plug the area around the usb port of one VESC started to smoke and glow. I immediately unplugged the antispark plug but the USB port was already burned and the nearby can cable melted to the socket. Of course they didn't work any more, not even one of them, i guess the death came through can :) The cause for this mayhem: During the testride the shrinktube on the cable connecting both 5s3p packs was damaged, it touched the case. This resulted in the Case being plus pole. Since the regular minus pole had the vescs connected, the contact of the USB port with the case closed the circuit. I'm actually glad this happened since I wasn't aware of the danger, I knew about the conductivity of CF but underestimated it. Now I lost some money but I have the chance to apply my newly acquired knowledge and make it even more safe. Since I took the train with it today and went to work it could have been way worse so I'm grateful that it happened right under my nose :smiley:
```

---
## \#15 Posted by: visnu777 Posted at: 2018-09-07T10:52:59.450Z Reads: 31

```
I have to pull this up again. I just found out by accident that there is 34.8 Volts on my deck/integrated enclosure against my plus pole. During charging I touched one of the screws holding my enclosure lid with still humid hands from washing and it tickled a bit. I did some detective work and found out that it seems to come from the motors. When i put the minus pin of the voltmeter on the truck its even closer to the real voltage 40.6V. Its only happening when the VESCs are plugged in without Antispark-Plug even there. The CF is connected by the truck mount screws I guess. Is this normal? Does everybody have electricity on the trucks?
Both trucks show this when I connect their VESC, alone and together. One has less Voltage than the other :crazy_face:

edit: I just connected the Antispark and pulled the trigger for some time, now the strange behaviour voltage dropped to 26V. Could it be that the motor became wet?
```

---
## \#16 Posted by: Cobber Posted at: 2018-09-07T12:11:32.703Z Reads: 27

```
You have some issues dude. 
The motor wires/windings should be insulated, Vedder has done some of his vesc motor tests with the motor in a tub of water...
```

---
