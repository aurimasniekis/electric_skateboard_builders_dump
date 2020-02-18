# Another bms issue (not charging)

### Replies: 30 Views: 291

## \#1 Posted by: Komamtb Posted at: 2018-09-06T12:15:37.581Z Reads: 76

```
Hey, did I wired my bms incorrectly? It is not charging.![15362360212111198327108721430988|374x500](upload://3E5phdk36e3yVTglKDENpczkJxw.jpg)
```

---
## \#3 Posted by: Trdolan03 Posted at: 2018-09-07T06:59:26.310Z Reads: 57

```
Were all the cells prebalanced?
```

---
## \#4 Posted by: Andy87 Posted at: 2018-09-07T07:12:43.428Z Reads: 54

```
Did you get wiring diagrams with your bms? If yes make a picture please and upload it.
You use lifepo4 cells right?
You charger also the right voltage for them?
Did you check the output voltage?

Stupid question but we have a bit less information till now.

You sure your bms work as charge only bms?
Which bms you use?
```

---
## \#5 Posted by: Komamtb Posted at: 2018-09-07T07:30:12.558Z Reads: 52

```
This is my already used pack, it is a 12s5p battery from 25r cells. The pack is balanced, it did kad a bms on it, I'm only changing to a smaller one. It is for charge only. I have bypass it with push to start switch. Here is the picture of the diagram.![IMG_20180907_102552|666x500](upload://yxoOKG6LbI71Mo833x8aTL2O7Pd.jpg)
```

---
## \#6 Posted by: zaq Posted at: 2018-09-07T12:59:05.175Z Reads: 48

```
IMO you should connect B- from your battery to the B- port on your BMS ( B- isn't used in your picture ).
Connect C- ( BMS port to charger - port ) and the + of the charging port to your B+ ( battery Terminal ).

BTW: I'm not sure about your balancing leads aswell tbh, since there is a gap between those 2 connectors.
Your wiring diagram shows 13 leads. ( B- B1 B2 B3 B4 .. B12 which equals 0V; 4,2V; 8,4V ... )
Check the voltages on those leads and make sure everything is connected as your diagram shows ( there is another B- lead ).
```

---
## \#7 Posted by: Komamtb Posted at: 2018-09-07T13:09:27.293Z Reads: 46

```
The one skipped is number is B10 on this bms the B9 and B10 are soldered together, also there is a gap with no wire in the original pin for those pins. ![41264731_938805256304763_2775310946443198464_n|666x500](upload://g4eTwF3qQHQEjyOcrgoeBbDkj8h.jpg)
```

---
## \#8 Posted by: zaq Posted at: 2018-09-07T13:16:25.129Z Reads: 41

```
Okay, might be a 13s BMS which is modified to work with 12s. I have one of those aswell.
If all those leads are connected correctly you still have 13 balance leads ( i count 13 in your picture, so those might be fine ).

Still, you have to make sure to connect B- port of the BMS to your battery B- port ( this connection isn't there in your picture.
```

---
## \#9 Posted by: Komamtb Posted at: 2018-09-07T13:36:16.113Z Reads: 41

```
Thank you very much, I will try it, once i did plug the wider plug with out skiping the one, a short happened, it was just for a moment, do you think the bms will be okey?
```

---
## \#10 Posted by: zaq Posted at: 2018-09-07T13:41:19.295Z Reads: 40

```
Well, i can't really tell you. Did you charge it without the B- port succesfully before? 
I can't say for sure if it is possible to charge without B- port connected, if there is a B- balance lead attached. 
Might work, might be defective..
```

---
## \#11 Posted by: Komamtb Posted at: 2018-09-07T13:42:13.944Z Reads: 40

```
No, i have only soldered that one lead, I was thinking only one is needed.
```

---
## \#12 Posted by: Komamtb Posted at: 2018-09-09T14:34:13.206Z Reads: 36

```
So I re wired it as you said, doesn't seem to be charging, any ideas maybe?![IMG_20180909_172054|374x500](upload://xC2TIXDjZABgrtTYhzrf4HSp4qX.jpg)
```

---
## \#13 Posted by: Andy87 Posted at: 2018-09-09T14:45:38.156Z Reads: 35

```
Why you measured minus voltage?
You mixed the polarity also on the bms?
```

---
## \#14 Posted by: zaq Posted at: 2018-09-09T14:47:36.381Z Reads: 35

```
Since everything is shrinked i cant tell you if you wired it correctly.
I just tried to explain you what you wiring diagram shows ( so make sure you connect the BMS the way it is shown in the diagram ).

The only difference in your wiring vs the diagram wiring is: you connect your load ( ESC ) directly to battery terminals since you want to bypass it for discharging.

So either you draw a diagram how you wired it or you have to undo the shrink wrap so we can see how you wired it.
```

---
## \#15 Posted by: zaq Posted at: 2018-09-09T15:02:44.616Z Reads: 34

```
![Unbenannt|690x389](upload://jqhq0xLKQ9EIcCzjOTPioQ5ZaL9.png)

This should be your "charging curcuit". Make sure to connect 13 balance leads from 0V/4,2V/8,4V/.../50V
```

---
## \#16 Posted by: hyperIon1 Posted at: 2018-09-09T15:04:13.392Z Reads: 33

```
bypass on bms for direct discharge 
![image|386x499](upload://s875lBmHLE9ZweEOeR8DFIOW1p.jpeg)
```

---
## \#17 Posted by: Komamtb Posted at: 2018-09-09T15:06:36.003Z Reads: 30

```
That is exactly how I wired it, my multimeter leads are just mixed. I was measuring to see if it's charging.
Edit: Maybe this has something to do with it?
![Capture|328x82](upload://bxmqkFDn8fI6A814oe9HEHIKD6b.PNG)
```

---
## \#19 Posted by: hyperIon1 Posted at: 2018-09-09T16:54:30.410Z Reads: 25

```
That’s only when you use the switch. If it’s not connected it shouldn’t stop charging and discharge. I did see something in a pic you posted that could cause issues. 
 This shouldn’t be jumped. 
![image|414x500](upload://4wgKYVkTFKpRoS9yYdaTg1GCv7D.jpeg)
```

---
## \#20 Posted by: hyperIon1 Posted at: 2018-09-09T16:58:37.332Z Reads: 23

```
I see now.  It’s a 13s bms modified to do a 12s set up?
Kinda funny to do that way. usually you  just delete the 13th balance pin. 
You replaced the original bms correct. Where did you get the new one?
```

---
## \#21 Posted by: hyperIon1 Posted at: 2018-09-09T17:02:18.442Z Reads: 23

```
That’s it. It should be all single pins. No jumps. You only delete the 13 balance pin. ![image|313x500](upload://aJ9IeEczaC90Wq5YQZ1FnzHcpuR.jpeg)
```

---
## \#22 Posted by: Komamtb Posted at: 2018-09-09T17:08:25.761Z Reads: 23

```
This pin is jumped on the new plug, it doesn't go anywhere. The wiring is still the same, I have only changed the plug!
```

---
## \#23 Posted by: hyperIon1 Posted at: 2018-09-09T17:43:50.062Z Reads: 22

```
I couldn’t see the pins behind the jst connector. 
If it’s not charging it could be a bad bms. 
If you discover it is. 
I have a replacement you can use. 
Bestech d140 
Set up for discharge directly form pack. 
With charge/ balance
```

---
## \#24 Posted by: Komamtb Posted at: 2018-09-09T17:46:59.968Z Reads: 20

```
Unfortunately the one I have, is the biggest that can fit in my setup.
```

---
## \#25 Posted by: hyperIon1 Posted at: 2018-09-09T17:51:33.459Z Reads: 20

```
I think li tech power sells a bms that size
```

---
## \#26 Posted by: Komamtb Posted at: 2018-09-09T17:52:20.968Z Reads: 19

```
This was bought from them.
```

---
## \#27 Posted by: hyperIon1 Posted at: 2018-09-09T17:55:50.598Z Reads: 20

```
O shit. I’m just no help.
```

---
## \#28 Posted by: hyperIon1 Posted at: 2018-09-09T17:57:36.387Z Reads: 19

```
3/4 inch deep enclosure?
```

---
## \#29 Posted by: Komamtb Posted at: 2018-09-09T18:00:17.356Z Reads: 20

```
It's a 1inch, but all the space is taken, this bms was really a long shot help for my build.
```

---
## \#30 Posted by: hyperIon1 Posted at: 2018-09-09T18:10:24.155Z Reads: 21

```
I don’t think your dead in the water yet. If you could give me a bit more info. The bms we use are olny 1/4 thick. 
If you are able to replace a bms and the pack is from China ( 1 inch thick ) you could brake down your pack to bare minimum and put the bms on top.
```

---
## \#31 Posted by: Komamtb Posted at: 2018-09-09T19:30:24.571Z Reads: 21

```
Sory, my bad, my Eu unit system confused me, my enclouse is only 20mm.
```

---
## \#32 Posted by: hyperIon1 Posted at: 2018-09-09T21:19:52.118Z Reads: 18

```
Yea. You are as flat as you can go at cell size 20mm. 
Sorry I couldn’t help.
```

---
