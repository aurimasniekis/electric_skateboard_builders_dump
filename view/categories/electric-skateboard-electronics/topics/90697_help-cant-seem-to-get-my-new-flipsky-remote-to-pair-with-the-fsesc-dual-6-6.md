# Help! Cant seem to get my new flipsky remote to pair with the FSESC dual 6.6

### Replies: 34 Views: 927

## \#1 Posted by: Skyart15 Posted at: 2019-04-16T02:48:46.333Z Reads: 163

```
Hey guys, need some help. Cant seem to get my New flipsky remote to pair with my FSESC 6.6. The motor set up seems to work but when i get to the input set up, i go into the PPM option and the remote doesnt seem to work, am i missing a step or two? This is the first time im programing any VESC, any help would be appriciated! Thanks guys!![20190415_194327|375x500](upload://rV8r2KglV9mAsV3rN4ZtSXLgBr0.jpeg)
```

---
## \#2 Posted by: Andy87 Posted at: 2019-04-16T05:35:54.553Z Reads: 152

```
Is the remote connected to the receiver?

Is the ppm cable pluged in in the right order?
```

---
## \#3 Posted by: ARetardedPillow Posted at: 2019-04-16T06:14:08.336Z Reads: 148

```
That remote is connected via UART.
Please read the description 
https://flipsky.net/collections/accessories/products/flipsky-remote-vx1?variant=22002887262268
```

---
## \#4 Posted by: Skyart15 Posted at: 2019-04-16T12:27:13.931Z Reads: 136

```
Ok so i tried that and maybe i am doing something wrong. I had it connected like the diagram shows, and still nothing would happen when i pushed or pulled the scroll wheel. Is there a diffrent way to program it in the vesc tool?
```

---
## \#5 Posted by: JohnnyMeduse Posted at: 2019-04-16T12:35:10.545Z Reads: 134

```
it won't work with the PPM setting if you are plug-in UART. You need to configure the UART not the PPM.
```

---
## \#6 Posted by: Skyart15 Posted at: 2019-04-16T12:41:02.339Z Reads: 128

```
Gotcha. Thanks. I will try that tonight and see how it goes. Also does anyone know how i can program my fsesc dual to have one vesc as master and the other as slave? The video that flipsky has on their website shows the proccess as being more intuative then it is with the vest tool. For example in that video after the guy finishes programing one vesc and does the settings for one of his motors, he plugs into the other one and clicks the app settings button and it basicly asks him if he wants to set the other vesc as slave. This does not happen on my vesc tool. Not sure if maybe i have a different version or what is up.
```

---
## \#7 Posted by: defyent Posted at: 2019-05-01T03:34:04.836Z Reads: 108

```
Did you ever get this resolved with ppm?
```

---
## \#8 Posted by: Skyart15 Posted at: 2019-05-01T04:11:11.835Z Reads: 104

```
No, but i did get UART to work, the UART jacks had the orange and green wires reversed once i fixed that it started working like a dream
```

---
## \#9 Posted by: defyent Posted at: 2019-05-01T04:30:36.095Z Reads: 104

```
What did you change in the vesc tool to make the uart work? I've changed "App to use" to UART but still no go. Made sure the cabling was correct too. Both UART and ppm don't work for me. Old receiver works fine so I know it's not my vesc.
```

---
## \#10 Posted by: Skyart15 Posted at: 2019-05-01T04:33:52.987Z Reads: 104

```
Make sure your wires look exactly like this ![Screenshot_20190430-213246_Samsung%20Internet|243x500](upload://ilzvel9OxQhfnd3KVVA7Mprx2FK.jpeg)
```

---
## \#11 Posted by: Skyart15 Posted at: 2019-05-01T04:35:40.074Z Reads: 102

```
Orange, green, black, red. And the other side green, orange and plugged in exactly like that. After you rogram your motors, the remote is plug and play, doesnt need any programing, but i hear on thsi forum that you can adjust the settings in the nunchuck app
```

---
## \#12 Posted by: defyent Posted at: 2019-05-01T04:37:31.390Z Reads: 97

```
So the motors need to be programmed again afterwards? I didn't realize that. My wiring is all correct, but hadn't done that step yet. I'll give it another go. Cheers.
```

---
## \#13 Posted by: Skyart15 Posted at: 2019-05-01T04:37:40.061Z Reads: 91

```
Make sure the white wire is connectex to your battery also
```

---
## \#14 Posted by: Skyart15 Posted at: 2019-05-01T04:38:48.328Z Reads: 89

```
No no, you have to program motors first, and make sure the renote is unplugged from the UART ports, flipsky website says it will mess with your programming
```

---
## \#15 Posted by: Skyart15 Posted at: 2019-05-01T04:39:57.343Z Reads: 87

```
Had this issues also when i programmed with the remote plugged in, but after i unplugged it and reprogrammed, then plugged the remote in, it worked good
```

---
## \#16 Posted by: defyent Posted at: 2019-05-01T04:40:10.754Z Reads: 82

```
okay, well thats essentially what I've done then, also my voltage reading is always blinking, so I think maybe my receiver is dead. (It's definitely paired)
```

---
## \#17 Posted by: Skyart15 Posted at: 2019-05-01T04:41:02.279Z Reads: 80

```
If its low on battery it will vibrate, is the blue led on the transmiter blinking?
```

---
## \#18 Posted by: defyent Posted at: 2019-05-01T04:42:48.016Z Reads: 83

```
connection led is solid, and is the color of the mode I've selected. Remote battery indicator is solid green, and board battery indicator is indicating 1 bar, and it's blinking, which tells me my board is less than 10% battery, which it isn't.
```

---
## \#19 Posted by: Skyart15 Posted at: 2019-05-01T04:43:41.911Z Reads: 81

```
Weird. You running the dual fsesc 6.6?
```

---
## \#20 Posted by: defyent Posted at: 2019-05-01T04:44:00.783Z Reads: 75

```
yeah i am .
```

---
## \#21 Posted by: Skyart15 Posted at: 2019-05-01T04:45:21.328Z Reads: 73

```
Is your white wire connected to the battery?
```

---
## \#22 Posted by: Skyart15 Posted at: 2019-05-01T04:45:52.942Z Reads: 73

```
The possitive side of your battery
```

---
## \#23 Posted by: defyent Posted at: 2019-05-01T04:47:43.539Z Reads: 75

```
It's connected to the positive side of the input into the ESC, which is coming from my no spark switch. Reading the voltage with a multimeter gives me the correct voltage going into the receiver's V pin
```

---
## \#24 Posted by: Skyart15 Posted at: 2019-05-01T04:49:46.617Z Reads: 70

```
Not sure what could be up bro :/ double check all the cables and connections, and if you can't find anything, i would contact flipsky. Or get help from someone local, where about do you live?
```

---
## \#25 Posted by: defyent Posted at: 2019-05-01T04:58:11.372Z Reads: 74

```
Thanks for the info :) I'll keep trying. I've put a message into flipsky so just waiting to hear back. I'm in NZ
```

---
## \#26 Posted by: defyent Posted at: 2019-05-01T05:03:10.375Z Reads: 75

```
https://www.youtube.com/watch?v=poW8DE0H-Vs

in case i've missed something stupidly obvious here's a video
```

---
## \#27 Posted by: Skyart15 Posted at: 2019-05-01T05:12:25.934Z Reads: 74

```
If you are saying that your skateboard battery is more then 10% charged, the only problem i can think of is that the small white wire is not reading the possite voltage properly, have you tried soldering it direcly to the battery possitive? Or atleast hold it to the battery possitive, for a second to see if your remote will start reading the board correctly.
```

---
## \#28 Posted by: defyent Posted at: 2019-05-01T05:17:50.312Z Reads: 73

```
Well when i test the voltage of the V pin on the receiver, against the ground pin on the receiver, it reads my correct voltage. just tried though, same result. I'll wait for flipskys response. Thanks again.
```

---
## \#29 Posted by: Skyart15 Posted at: 2019-05-02T19:09:35.650Z Reads: 71

```
Hey did you ever get it to work?
```

---
## \#30 Posted by: defyent Posted at: 2019-05-02T22:22:05.382Z Reads: 69

```
Unfortunately not. Flipsky repomnded and said they would look into it but I have not heard back
```

---
## \#31 Posted by: karrotboi Posted at: 2019-09-27T22:44:57.235Z Reads: 37

```
I apologize to revive this thread but I think I may have found a solution! I opened up my remote and turns out that the white wire was detached. Also for your voltage indicator, it should be that the wire soldered to your positive battery had come off from the receiver or the positive battery wire. Hope this helps :slight_smile:
```

---
## \#32 Posted by: itsrow Posted at: 2019-10-30T15:19:38.790Z Reads: 25

```
Is the white wire necessary for the remote to function I thought it was optional.
```

---
## \#33 Posted by: karrotboi Posted at: 2019-10-30T15:31:33.430Z Reads: 21

```
I meant the wires solder inside the remote broke off. The white wire with the reciever should be for the battery indication and is not required for the remote to function as mine recently broke off and I just don't have a boards battery indication anymore
```

---
## \#34 Posted by: itsrow Posted at: 2019-10-30T15:34:48.112Z Reads: 22

```
Ah thank you, I think my receiver is fried but I'm going to try UART after PPM didn't work.
```

---
