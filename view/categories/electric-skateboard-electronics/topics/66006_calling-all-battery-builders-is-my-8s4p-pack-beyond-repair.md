# Calling all battery builders - is my 8S4P pack beyond repair?

### Replies: 31 Views: 834

## \#1 Posted by: DaFunkyMonkey Posted at: 2018-08-25T07:27:42.553Z Reads: 301

```
I managed to break my Alien Power Pack (8S4P) this morning :( 

I was at the last stage of an All Terrain dual motor setup, when I had incorrectly soldered an XT connector to my vesc the wrong way around, which fried the battery when i turned it on.

The battery now has 4 burn marks up the side where the cells have melted the plastic cover, and the level indictor is only reading 5%. My main worry right now is that the battery will not turn off. I just left it outside the house hoping the battery will eventually drain itself to 0%.

Does anyone know if the battery pack is fixable or it any of the parts of it salvageable? If not, does anyone know how to dispose of the battery in the UK?
```

---
## \#2 Posted by: BigBrit Posted at: 2018-08-25T07:52:56.214Z Reads: 288

```
I'm sorry to say it's most likely dead now.  Take it to a tip, they have a battery thing there.

The Antispark is dead for sure, the fets are now fused open which is why it won't "turn off". Have you taken the shrink wrap off and measured the battery voltage into the Antispark?

  You could have even destroyed the VESC's too, could be an expensive mistake!
```

---
## \#3 Posted by: DaFunkyMonkey Posted at: 2018-08-25T08:13:29.844Z Reads: 276

```
Thanks for the reply and advice.

Unfortunately I have a busy day out of the house today so will not be able to work on it. 

Do you know if it's safe to leave it in the shed or is it likely to burst into flames any second?

Thankfully the vesc was a cheap flipky
```

---
## \#4 Posted by: BigBrit Posted at: 2018-08-25T08:22:54.250Z Reads: 250

```
I would say (although hard to know until you open it up and have a look) that it will be ok.  The Antispark is dead for sure, hopefully the pack hasn't somehow shorted itself
```

---
## \#5 Posted by: DaFunkyMonkey Posted at: 2018-08-25T08:35:12.292Z Reads: 243

```
Cool, thanks for all your help.

This might be a good excuse to upgrade to a 10S4P as I was a bit concerned that my 8S might have been a bit weak and possibly sagged for my new setup (dual 5065 200kv on evolve AT wheels).
```

---
## \#6 Posted by: DaFunkyMonkey Posted at: 2018-08-25T08:44:11.257Z Reads: 240

```
![20180805_095213|690x414](upload://593fNxv6W8a4Bp5IYPy0WnNqfcm.jpg)

it was so close to completion :(
```

---
## \#7 Posted by: DaFunkyMonkey Posted at: 2018-08-25T08:46:52.571Z Reads: 230

```
And such a stupid mistake.
```

---
## \#8 Posted by: xilw3r Posted at: 2018-08-25T09:04:00.524Z Reads: 227

```
I think the battery should be ok. If its not, hey, you have plenty cells for a beefy power bank :slight_smile:

Be happy that you didnt start a lithium fire. That would suck much much more.
```

---
## \#9 Posted by: DaFunkyMonkey Posted at: 2018-08-25T09:38:50.430Z Reads: 214

```
Absolutely, that went through my mind straight after cursing my own stupidity.
```

---
## \#10 Posted by: DaFunkyMonkey Posted at: 2018-08-25T09:42:01.325Z Reads: 207

```
Does anyone know or a battery repair service near Liverpool?
```

---
## \#11 Posted by: BigBrit Posted at: 2018-08-25T09:43:20.869Z Reads: 203

```
It could be quite easy to diagnose yourself mate.  Take the shrink wrap off and look at the wiring with a multimeter.
```

---
## \#12 Posted by: DaFunkyMonkey Posted at: 2018-08-25T10:10:35.083Z Reads: 199

```
I just opened it up to take a look:

![IMG_20180825_110526955|375x500](upload://cJSzixiFf66As6z9A8T7WC92cFo.jpg)

And I haven't got a clue what should be connected to what
```

---
## \#13 Posted by: xilw3r Posted at: 2018-08-25T10:11:25.604Z Reads: 191

```
Mate i think your picture did not upload :D
```

---
## \#14 Posted by: dareno Posted at: 2018-08-25T18:52:50.846Z Reads: 168

```
What bms does it have?
```

---
## \#15 Posted by: DaFunkyMonkey Posted at: 2018-08-25T21:17:59.633Z Reads: 158

```
Not sure, possibly from SmarTec. The number on it is pcm-l16s50-985(b).
```

---
## \#16 Posted by: pat.speed Posted at: 2018-08-26T11:11:48.651Z Reads: 130

```
First off please move some of the foam to check for damaged cells. Next in plug the bms balance leads and check with a voltage meter each cell group to confirm which ones may or may not be damaged. If they are all at the right voltage I would try and charge in a steel can outside. If not try pulling it apart and seeing where it’s broken or contact aps and see if they will service it for you. 

I’m thinking the bms should have cut off the power to not damage the battery
```

---
## \#17 Posted by: DaFunkyMonkey Posted at: 2018-08-27T11:06:01.767Z Reads: 97

```
Thanks for all the advise.
I removed the foam and found that a couple of the batteries appear to have cosmetic damage (burn marks) and the +ve connection between the BMS and the cells has disintegrated. I measured the voltage across the cells and it looks like they are ok 😁  However the BMS is a goner 😔
```

---
## \#18 Posted by: pat.speed Posted at: 2018-08-27T11:26:24.770Z Reads: 93

```
If there are burn marks on the cells this could not be good for the cells. I would ask Alien power systems about a repair, or contract @psychotiller if he would inspect it for you
```

---
## \#19 Posted by: DaFunkyMonkey Posted at: 2018-09-07T19:40:47.493Z Reads: 90

```
I asked APS  about battery pack repairs and unfortunately it's not a service they provide. However they can send me an identical replacement BMS. So, to any experienced battery builders out there, would you recommend that I try and replace the BMS on this pack, or is it beyond repair?

![IMG_20180827_143154955|375x500](upload://9nKJCudho3xkJ3tcjnXr9Y5HgRn.jpg)
![IMG_20180827_143322045_HDR|666x500](upload://AktzUxXFEu6ZnBzxUXbAZiOMfdt.jpg)![IMG_20180827_143258464|666x500](upload://tGmJaX8RTaGndBdNK9yDXwv1MM8.jpg)![IMG_20180827_143344756_HDR|666x500](upload://jbF4k0C7MhO9bxjgpRFmt1zyhbh.jpg)![IMG_20180827_143415533_HDR|666x500](upload://cBmVEahClfsVTIWgXnT3b9SO4G4.jpg)![IMG_20180827_143425328_HDR|375x500](upload://1hRK1KfeJQdeEijLBstJWgJJADD.jpg)![IMG_20180827_143354671_HDR|666x500](upload://swRigIXHSmu4Zr930Q3fANUSxwM.jpg)
```

---
## \#20 Posted by: myreala Posted at: 2018-09-07T20:28:34.339Z Reads: 79

```
Looks like all your series connections burned out and opened the circuit. It looks like AlienPower systems only used single layer of Nickel this might have saved you as those series acted like a fuse. You should be extremely happy and thankful that you avoided a massive fire. Some of those cells might still be okay but I would not attempt a repair on the whole pack as there are bound to be some bad cells in there.
```

---
## \#21 Posted by: Brdchris Posted at: 2018-09-07T20:40:08.008Z Reads: 74

```
I’m crazy. But I would just check the voltage of each p group. If they are all similar, I would reweld the connections and run with it. I agree that the s connections acted like a fuse.
```

---
## \#22 Posted by: DaFunkyMonkey Posted at: 2018-09-08T09:14:58.603Z Reads: 67

```
Yep, super thankful that it didn't burn the house down, but still cannot help feeling bummed that this has happened right at the end of the build. I have spent a ton of cash in getting to this point and I've been building  it for an eternity (slowly buy piece by piece). Plus the timing sucks as currently in the process of changing job and moving house so will not be able to spend much time or money on it for awhile. Anyhow I must keep telling my self it could have been a million times worse. Sorry rant over.

Although there are burn marks on the series connections, they all seem to be intact. The only nickel strip to break was the one connecting the BMS to the pack (first picture above). 

I think the battery pack  is ok as one my colleagues at work was able to charge the pack by bypassing the dead BMS using A PSU.

Unfortunately I don't have a spot welder and will not be able to get one anytime soon. So I was thinking that I'll probably take a risk and replace just the BMS.

Do you know of anyway to attach the BMS to the battery pack without spot welding it (first pic above)?
```

---
## \#23 Posted by: Andy87 Posted at: 2018-09-08T14:59:28.041Z Reads: 50

```
Like it was made before by soldering it on it.
Get a 10awg and solder it on the bms and on the nickel on the batterie.
You sure there is nobody around you who could remake the Batterie?
You already had once luck, wouldn’t risk it once more. Better save than sorry with batteries. Especially if you just moved...take care about your new home...200-300$ are less then thousands for rebuilding 😉
```

---
## \#24 Posted by: TowerCrisis Posted at: 2018-09-08T18:24:55.777Z Reads: 50

```
You need to scrap that BMS.

There's an issue with them, where if there is a load connected to the battery (like it's shorted) and a series connection within the battery breaks, then the balance cable portion of the BMS will break.

This is because normally the BMS only sees a Max of 4.2V difference between balance cables. When you short the battery and break a series connection, the new voltage differential between the two balance cables on either side of the series connection break jump to your full battery voltage. This almost certainly fries the balancing function.

BUT this is only the case if the nickel tabs fused out. If there's still continuity within the pack then you might be lucky.


This is also why I'm not a fan of cell level fusing, because in the case of a fuse out scenario it might set the BMS on fire.
```

---
## \#25 Posted by: Brdchris Posted at: 2018-09-08T18:59:22.824Z Reads: 46

```
See I think I like cell level fuses and don’t like bms’s. Mine is bestech and seems to be nothing but trouble. I would rather just drop the deck once a month or so and check/charge with a hobby charger to manually balance
```

---
## \#26 Posted by: TowerCrisis Posted at: 2018-09-08T19:19:51.071Z Reads: 44

```
They're definitely opposing solutions to one problem.
```

---
## \#27 Posted by: Brdchris Posted at: 2018-09-08T20:19:36.539Z Reads: 45

```
Agreed. Bms makes it a lot like a factory build, out of sight out of mind, but we diy so I don’t mind opening it up to check things out every now and then
```

---
## \#28 Posted by: hyperIon1 Posted at: 2018-09-09T04:12:54.214Z Reads: 37

```
if you get a chance bypass the discharge function and run charge balance only.
we have seen so many packs with good cells in them and bad bms units. 
we will soon start taking request to rework factory battery packs. 
we can't rework every battery pack but the majority of them can be fixed.....
```

---
## \#29 Posted by: DaFunkyMonkey Posted at: 2018-09-12T19:20:49.018Z Reads: 33

```
I decided to go the simplest route for now and just replace the dead BMS with an identical one. That way I can just plug the existing balance wires into the new BMS and copy the soldering of the power button, display, charge port, usb port and any other wires from the old BMS onto the new BMS. Hopefully that will get it up and running again with little effort. If it works I'll continue to keep the battery pack in the shed.

Can anyone tell me if I need to reconnect the wires to the new BMS in any particular order?
```

---
## \#30 Posted by: Andy87 Posted at: 2018-09-12T19:45:26.285Z Reads: 26

```
Yes, in the same way it was before 😅
Just take a picture, or take the pictures you already made and connect the wires like they where before
```

---
## \#31 Posted by: DaFunkyMonkey Posted at: 2018-09-12T20:15:19.138Z Reads: 22

```
Do I need to connect the balance wires after soldering the -ve and/or +be wires, or does it not matter which wires are soldered to the BMS first?
```

---
