# Will a PLA 3D printer motor mount melt? (and a history lesson)

### Replies: 17 Views: 2263

## \#1 Posted by: Clonkex Posted at: 2017-08-24T04:56:28.017Z Reads: 201

```
Hey all,

I'm a big fan of Corridor Digital, and recently discovered the Sam & Niko channel. After binge-watching a heap of their videos and seeing Wren floating around on his OneWheel (_really_ wish I could afford one of those!) and riding various electric skateboards I became quite interested in the idea of making my own electric board. The hefty $1000+ price tag of most commercial boards made me a bit skeptical that I could make my own on my very limited budget, but after a bit of googling I was quite surprised to find a huge number of DIY builds using cheap, easy-to-get parts.

I watched a tonne of videos to absorb as much information about the subject as possible as quickly as possible, then bought a motor, an ESC, a second 3S 5000mAh lipo (already had one from my [giant custom quadcopter experiment](https://www.rcgroups.com/forums/showthread.php?2330324-Skyduino-X525-Feature-rich-Arduino-based-Custom-FC-Autonomous-FPV-Quad) from a while ago, gonna wire in series for 6S - will probably upgrade to 8S as soon as I can afford it to reduce the current requirement) and the pulleys and belt from [RS online](au.rs-online.com) (which I didn't know was a thing and I freaking LOVE now). I already have a Z-Flex cruiser board (definitely not the nicest board but pretty easy to ride and should work well for this project). Never fear, I have a regular skateboard as well, I'm not a poser :P

The pulleys and belt arrived yesterday and I realised I was a dumb git and didn't measure wheels before buying the pulley. The wheels are 63mm and the pulley is just about exactly the same size. D'oh. I've bought a new, slightly smaller pulley which I'm hoping will be here on Friday so I can get to work over the weekend.

The plan is to use a couple of Arduino Pro Minis (one in the controller and one on the board) to control everything. They'll connect with two HC-05 bluetooth modules. If the bluetooth modules don't get here before the weekend I'll just whip up a test setup with a potentiometer and a wired controller.

Anyway, I'm here to ask a question. Can I make a motor mount out of PLA or will it just melt when the motor gets hot? PLA's glass point is around 60°C, but I don't know how hot the motor is likely to get. I don't have any ABS filament and I've never tried printing with ABS, though my printer should easily handle the temperature. My original plan was to experiment with a wooden clamped motor mount. I still think that'll work fine but if I can make something better I'd like to. I don't have the tools to machine something out of aluminium unfortunately.

Alternatively, if PLA and wood won't work, I did see [this post](http://www.electric-skateboard.builders/t/making-a-motor-mount/2876/62), which seems right up my alley. I reckon with a trip to the hardware store, some hacksawing and some drilling I could make something similar that could be quite solid. We actually do have a working welder but I have no idea what type it is and I've only ever welded once, so I'd rather not learn by attemping to weld something to an aluminium truck :P
```

---
## \#2 Posted by: L3chef Posted at: 2017-08-24T05:02:31.731Z Reads: 186

```
Tl;dr now when I'm at work. But yes pla directly in contact with motor will deform
```

---
## \#3 Posted by: JdogAwesome Posted at: 2017-08-24T05:07:28.165Z Reads: 185

```
Hey David, first off I dont think PLA will hold up at all. To start PLA is very strong though its low "melting" point will make it a bad choice for this. Its also a biodegradable material which means that over time with exposure to water and the elements its going to start to fall apart. I recently tried printing some pulleys for a boosted board to use Kegels and they just ripped apart even at 100% infill. I have seen ones printed in SLS Nylon work though I still wouldn't risk it and id only use ones with bolt running through them or full metal ones. I recently started working with PETG filament which has more heat resistance and is still strong similar to ABS, though its a lot easier to print with. You could try to use that though like I said I wouldn't recommend it, or expect it to last very long. Also about your HC-05 Bluetooth remote, id recommend using something else for communication like an NRF module due to the problems with bluetooth, mainly signal loss as well as power usage.
```

---
## \#4 Posted by: Crossfire Posted at: 2017-08-24T05:27:15.332Z Reads: 172

```
I've printed my mounts out of colorfabb HT, XT-CF20 and Extruder Greentec. All three survived but the best one is without the doubt the xt-cf20. It's printed at about 250-260 degrees, very abrasive filament but when it bonds it's very hard, sturdy and tough. Can only recommend.
Don't use PLA for these applications...maybe for a smaller enclosure but I won't put money on PLA to survive the beatings.
PETG should work just fine too.
```

---
## \#5 Posted by: Boardnamics Posted at: 2017-08-24T05:30:36.462Z Reads: 162

```
Unless you live in a colder area or your motor runs very cool, don't print it in PLA. It's not even because of the whole biodegradable ordeal, it is just like you mentioned, it's glass temperature. Brushless motors we use can go beyond 60C without being damaged. Generally, they can get as hot as 80C (176F) without being permanently damaged. When I made a motor mount in PLA, it deformed more quick than I had thought. It got all bendy, just avoid it.

PETG does do the trick. If your PETG mount deforms, chances are your motor overheated anyways.
```

---
## \#6 Posted by: Clonkex Posted at: 2017-08-24T05:33:45.001Z Reads: 150

```
Ah, that's a good point about PLA being biodegradable, totally forgot about that. Yeah ok, I'll go ahead with my wooden mount experiments (though I'm not convinced it will hold up to the tension since there's a maximum thickness I can make it due to the length of the motor shaft - time and experimentation will tell). I don't have any filament other than PLA unfortunately so I can't experiment with a 3D printed part.

I'm not worried about the power usage of bluetooth but connectivity issues won't be good. I've seen commercial boards that use bluetooth; what could cause a connection issue? I was also considering the NRF modules but assumed bluetooth would be more reliable.
```

---
## \#7 Posted by: Clonkex Posted at: 2017-08-24T05:35:22.019Z Reads: 136

```
Thanks for the suggestions from everyone else. I'll look into other filament types but I've never tried printing with anything except PLA so that will be an adventure on its own. For now I'll see if I can make a sufficiently strong wooden mount, or see what I can find at the hardware store to dodgy up an angle bracket-based mount :P
```

---
## \#8 Posted by: L3chef Posted at: 2017-08-24T05:41:19.105Z Reads: 123

```
Check out armadillo filament
```

---
## \#9 Posted by: JdogAwesome Posted at: 2017-08-24T06:00:43.250Z Reads: 128

```
Personally I just ordered a role of PETG off Amazon gotta love Prime lol. Anyways yeah I'd love to see a wooden mount, I don't think anyone's done that before. On the remote side, the ones that do use Bluetooth tend to have reported connectivity problems, though don't take my word for it I haven't messed with the Bluetooth or NRF modules to much I mainly like the ESP8266.
```

---
## \#10 Posted by: Clonkex Posted at: 2017-08-24T06:10:12.880Z Reads: 125

```
Amazon is almost non-existent in Australia so Prime isn't a thing. eBay is the first stop for the vast majority of the stuff I buy.

Yeah I couldn't find any reference to wooden motor mounts anywhere so I'm pretty interested to see if it can work. I'll be posting a build log when I get all the parts :D

I'm a programmer so I'll be programming my own Arduino-based controller system. I have experience with controlling ESCs with Arduinos (from my quadcopter build) and since I'm programming it myself I can build in good safety systems. Not too worried about that side of things. If I have connectivity issues I can always replace the modules.
```

---
## \#11 Posted by: JdogAwesome Posted at: 2017-08-24T06:32:05.053Z Reads: 111

```
Ahh didn't realize your were an Aussie, they really don't have much Amazon there? It's pretty much my life line lol. You could also try using like an ATiny85 or something similar chip to cut down on size even more cause you don't really need all the other io for something this simple.
```

---
## \#12 Posted by: Clonkex Posted at: 2017-08-24T06:37:20.110Z Reads: 110

```
Pretty much eBay is the equivalent over here; Amazon occasionally has its uses but hardly anything actually ships to Aus from Amazon haha.

Nah I'm a huge fan of Arduinos and I love the Pro Minis. I don't need a smaller board, I'm pretty good at stuffing larger-than-necessary electronics into small 3D-printed handheld devices :P
```

---
## \#13 Posted by: JdogAwesome Posted at: 2017-08-24T06:51:46.255Z Reads: 110

```
Yeah Arduino's and the Arduino IDE are great, use them as my MCU in practically all my projects. Oh and FYI the ATiny uses the Arduino IDE as well so in case you ever need a really small form factor MCU there a good choice.
```

---
## \#14 Posted by: Clonkex Posted at: 2017-08-28T04:56:05.571Z Reads: 89

```
Spent basically all of Saturday working on my build. Got the wheel pulley (which had a lump on one side that got in the way) angle-ground (angle-grinded?) and drilled out (which involved drilling a tonne of smaller holes around the middle and then attempting to file/hacksaw it out to be round; needless to say I'm jealous of anyone with a metal lathe). I also discovered that urethane, while easy enough to drill through, is incredibly difficult to drill _accurately_. It didn't help that the shape of my wheels meant it became an interrupted cut on the other side, so the drill bit decided to go on its own little adventure. Eventually I got the pulley attached to the wheel. It's not perfectly centred but it's close enough for the moment and with a bit of kajiggering I can probably get it perfect.

The next step is the motor mount. This is the hard bit. So far I've only spent about an hour and a half on it, but I believe I've worked out how to do it, and it's going to be made of wood. Since my trucks are very _shaped_ (kind of L-shaped when looking end-on) my plan is to cut out approximately the same shape in the wood so that it just slides on. Then I can araldite it and see how strong that is. If it's too weak I can easily make a brace to slide onto the other side and bolt across the truck. Hmm :thinking:  Maybe I should take a heap of photos and make a build log thread, since this is getting off-topic for this thread.

If only I had the money for some more expensive power tools, like a metal lathe and a decent welder... The way I wield hand tools I'll soon be experiencing death by a thousand cuts :confounded:
```

---
## \#15 Posted by: Toastertato Posted at: 2017-08-29T00:59:21.129Z Reads: 74

```
I have a 3D printed motor mount on my board. It was printed at 5% infill and, generally, has been holding up OK. There wasn't any issue with the motor melting into the plastic, but there has been plenty of other issues. 
The area that connects the mount to the trucks starts to become loose after a while, the rate at which probably depends on the weight of the motor and infill. This is even with some skateboard screws I used as set screws. 
Also, design the mount so that the motor is at a fixed distance. I printed mine with some slack so I could tighten/loosen the belts by about a cm or so when setting it up. The result was that after a few uses the motor would inch closer to the trucks and the belt would start to slip. My mounting screws were also digging into the plastic. I had to solve this by using a lot of hot glue (which **does** start to melt at high enough motor temps). I think much of these problems would be solved if you printed it at a much higher infill and made sure the design was good. Hopefully this helps.
Good luck with your board!
```

---
## \#16 Posted by: Clonkex Posted at: 2017-08-29T01:13:45.152Z Reads: 81

```
Thanks, that's useful information. I've decided to make a wooden motor mount because I think it should work really well and I don't have a lot of tools for working with metal. Although maybe if I printed a mount first I could experiment and then use it as a template for the final wooden mount :thinking:
```

---
## \#17 Posted by: Crossfire Posted at: 2017-08-30T09:40:02.094Z Reads: 69

```
I'm using a 3D printed motor mount out of XT-CF20 filament. Best filament for these applications.
```

---
