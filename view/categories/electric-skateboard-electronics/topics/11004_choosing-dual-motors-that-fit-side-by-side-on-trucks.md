# Choosing dual motors that fit side by side on trucks

### Replies: 15 Views: 1111

## \#1 Posted by: Kaden56 Posted at: 2016-10-12T06:24:10.272Z Reads: 156

```
Newbie here jumping into what seems to be one of the coolest hobbies of all time. 

I've been into longboarding on and off for several years and had a few longboards. The only board I have left now is a 55" sector 9 with an 11" wide deck. I immediately fell in love with the shear size of this board and can't wait to make it electric.  I can only put about $650 into this first build beings that I'm married with a new baby and going to engineering school at the University of Utah. 

My first purchase is going to be the two motors so I can gets going on the motor mounts. I built a CNC over the summer that is capable of milling aluminum and I have aluminum to use for all the mounts and sprockets and things. My problem is that I can't seem to find motors that will fit between my wheels. Measuring from wheel to wheel I have exactly 6.5 inches. I wanted to use the turnigy sk3 245kv or 190kv (another question I have is which would go with my 10s setup better out of those two) but they both seem like they may be impossible to fit. Would the g160 here: http://www.hobbyking.com/hobbyking/store/uh_viewItem.asp?idproduct=44881
be a good motor for this dual set up? It would save a lot of room because it's not as long. Would it still be as powerful as the sk3?
```

---
## \#2 Posted by: rpn314 Posted at: 2016-10-12T06:42:11.101Z Reads: 151

```
Welcome!

Dual setups can be hard to squeeze in there. Which trucks do you have exactly? That will most likely determine what you can fit. I just took a quick measurement and I've got got somewhere between 6.5" and 7" in between my wheels, and I was able to fit in dual 6355 (@torqueboards), but it's definitely really close, so it's hard to say for sure if it'll work with what you've got.

As for the kv rating, I think 190kv is better for 10s than 245kv. 220kv, maybe 230kv is really the max you should do at 10s if you're going to use a VESC. If you're doing a different ESC I will relinquish the floor to someone who knows better than I.

On a side note, I'm just down in Provo doing EE at BYU, so if you want to get together and look at spacing or just try out my board, we can definitely arrange that. I'm up at the U to visit family pretty frequently anyways :slight_smile:
```

---
## \#3 Posted by: chaka Posted at: 2016-10-12T06:42:34.671Z Reads: 141

```
Dual diagonal will give you a better ride. Having all the weight out to the rear will cause you to ice out if you get absent minded while carving. Of course this is just my personal preference, a dual rear can be an equal contender in performance but it will be tail heavy.
```

---
## \#4 Posted by: saul Posted at: 2016-10-12T09:38:05.069Z Reads: 128

```
On a board that size I don't think weight is an issue, and dual diagonal would have crazy long wires...

i think the 190kv would be better on 10s, especially if you use vesc. and you should. :sunglasses:

but i'm more interested in the cnc!
```

---
## \#5 Posted by: Kaden56 Posted at: 2016-10-12T16:54:56.310Z Reads: 106

```
How cool that you live so close! I would love to take you up on that sometime soon. It would be cool to test out a board because I've never ridden one with motors! It would also be a good opportunity to pick your brain and confirm or change some of the plans I have for the build.

I don't know why I said 10s I'm actually making it 9s. Each of the two vescs will have 3 3s 5000mah zippy's in series. I'd like to eventually add 6 more of the same batteries in parrelell with the two sets of batteries to double the mah without increasing the voltage. 

From what I've read 190kv would still give me more torque that the 245kv even with 9s. Does that sound accurate? I weigh 180 and my board certainly won't be light. Also I will often be carrying more than 20lbs with books and a gym bag at the university. I'm way more about torque than top speed. That's why I want to use chain and sprocket as well. As long as my board can reach 20mph I'm perfectly fine because I don't want to be going any faster for safety reasons. I would love for my board to have a crazy amount of torque for going uphill. My biggest question is whether the g160 is a good motor for the vesc on 9s or if I should look into new wider trucks just to fit two 190kv SK3's.
```

---
## \#6 Posted by: Kaden56 Posted at: 2016-10-12T17:01:16.532Z Reads: 102

```
You know? That makes a lot of sense. My only worry is if it would be weird when turning. But I trust you as an expert knowing that you have obviously ridden boards this way a lot. This would solve all problems with making room for the motors too. Because I would be running the motors off of two separate battery packs and two separate esc's the only wire that would need to cross the board is the wire from the controller receiver. I will seriously consider this, thank you Chaka.
```

---
## \#7 Posted by: Kaden56 Posted at: 2016-10-12T17:14:17.955Z Reads: 102

```
Ya I'm certainly not concerned about the board weighing a lot 😂 I can literally lay down on the board.  And I agree I believe I want to go with the 190kv because I'm more concerned about torque than speed. 

If you are interested in my CNC I made a video trying to explain my build to help anyone that may want to build one. They are super easy conceptually, but you can make the build as easy or complex as you want to. Here's a YouTube link if you are interested. https://youtu.be/hoG3FUQ05Fs
And here's another showing it cutting. https://youtu.be/EYHOsZRA4UM
```

---
## \#8 Posted by: saul Posted at: 2016-10-12T17:32:28.102Z Reads: 101

```
cnc looks very clean! i've been wanted to build something similar since i got my 3d printer but i've been building boards instead :money_mouth:

The whole split battery things seems kinda weird, you'd need 2 keyloop or spark switches....but if you are doing this dd drive makes more sense.

if you really want torque you just need the right gearing. my single 6374 149kv has plenty with 14/36t.
```

---
## \#9 Posted by: rpn314 Posted at: 2016-10-12T17:45:03.231Z Reads: 97

```
Of course!

If you're planning on 9s, you'd probably be okay with a 245kv. I assembled the list below when I was deciding what cell count to go with and so I had it in my notes. I just added 9s for you. As for that motor, I think a dual setup with the motors on the same side of the truck are extremely difficult without the truck having a 10" hanger length, thus @chaka's suggestion of a dual diagonal. You probably wouldn't have to use two separate battery packs but you're accurate on everything else.

Motor KV ranges
12s = 170->190kv
10s = 200->225kv
9s = 225->250kv
8s = 260->290kv
6s = 340->380kv

Based on:
Estimates for cells at 4.2v
8570 RPM/50v = 170kv - 12s
8570 RPM/42v = 200kv - 10s
8570 RPM/37.8 = 225 - 9s
8570 RPM/33v = 260kv - 8s
8570 RPM/25v = 340kv - 6s

Estimates for Cells at 3.8v
8570 RPM/45.6v = 188kv - 12s
8570 RPM/38v = 225kv - 10s
8570 RPM/37.8 = 250 - 9s
8570 RPM/30.4v = 282kv - 8s
8570 RPM/22.8v = 376kv - 6s
```

---
## \#10 Posted by: Kaden56 Posted at: 2016-10-12T18:19:50.630Z Reads: 89

```
Ok that makes sense maybe I'll go with the 245kv then with the diagonal set up. Now I'm new on all of this so if you have two esc's can you hook them both up to the same battery pack? Would it be better to hook up 3 of the 3s batteries in series and then another 3 in parrellel rather than giving each motor its own pack? I guess an upside to both esc's going to the the same battery source would be that you wouldn't risk one battery pack getting low before the other one and throwing it off. I just didn't realize that you could hook up two esc's to one battery pack. I planned on getting two 9s bms's for each 3 battery series and then using a 36v 10a charger that would split 5a to each bms. 

That was a lot of just spilling ideas into one sloppy paragraph but I would appreciate any advice or instruction you may have.
```

---
## \#11 Posted by: rpn314 Posted at: 2016-10-12T18:32:26.380Z Reads: 84

```
Yeah. You can very easily split a single battery pack (which can be 9 in series and 3 in parallel. series adds voltage and then parallel adds current and total power stored) between two ESCs. And you can do the same for the bms (a single BMS) as long as the total series number matches the BMS's series number.
```

---
## \#12 Posted by: Luke Posted at: 2016-10-12T19:15:04.575Z Reads: 79

```
[quote="Kaden56, post:10, topic:11004"]
maybe I'll go with the 245kv
[/quote]

Hey :)  I'd still say that you would be better off with the 190 kv motors, as they can provide more torque, which you are looking for.
```

---
## \#13 Posted by: Kaden56 Posted at: 2016-10-12T21:53:37.160Z Reads: 71

```
O wow that would save a lot of wiring and I wouldn't have to buy another bms! Sounds good to me where I don't have $1000+ for this first build! I'll keep in touch with you if you don't mind when it comes to drawing out my wiring diagram and other things I'll have questions on. I also would love to meet up with you if you come up to salt lake some time so you can show me your board and share some knowledge. Thanks for all the help!
```

---
## \#14 Posted by: rpn314 Posted at: 2016-10-13T00:06:53.769Z Reads: 60

```
Of course! I'll be around, feel free to PM me if you need anything, and I'll let you know when I'll be up by the U. Probably won't be this weekend, but maybe the following weekend
```

---
## \#15 Posted by: Kaden56 Posted at: 2016-10-14T01:01:37.191Z Reads: 51

```
Sounds great! Quick question about charging. If I had a 9s bms could I charge all six batteries at once? Like I mentioned I would like to have 6 3s 5000mah batteries wired 3 in series with each one wired to another in parallel. Is it safe to charge like that? Also if they are all rated at 2C batteries then would charging them with a 5a 33V charger be good? This is the bms I am looking to get: http://m.ebay.com/itm/Balance-BMS-PCM-21A-w-Temp-Switch-for-9S-33-3V-Li-ion-Li-Po-battery-9S21W001-/221809130907?nav=SEARCH

And I would charge it with something like this hooked to the bms http://www.ebay.com/itm/like/261871246851?lpid=82&chn=ps&ul_ref=http%253A%252F%252Frover.ebay.com%252Frover%252F1%252F711-117182-37290-0%252F2%253Fmtid%253D1588%2526kwid%253D1%2526crlp%253D53601919689_324272%2526itemid%253D261871246851%2526targetid%253D186358926969%2526rpc%253D0.12%2526rpc_upld_id%253D82514%2526device%253Dm%2526mpre%253Dhttp%25253A%25252F%25252Fwww.ebay.com%25252Fulk%25252Fitm%25252Flike%25252F261871246851%25253Flpid%25253D82%252526chn%25253Dps%2526adtype%253Dpla%2526googleloc%253D9029759%2526poi%253D9029768%2526campaignid%253D239125209%2526adgroupid%253D14978428809%2526rlsatarget%253Dpla-186358926969%2526gclid%253DCj0KEQjw4fy_BRCX7b6rq_WZgI0BEiQAl78nd-pe1adk0NUpBDe-shHoh7pwTtUvqVIBBX8hQ9sUjaIaApfh8P8HAQ%2526srcrot%253D711-117182-37290-0%2526rvr_id%253D1109188633724&ul_noapp=true

Sorry that was a crazy long eBay link. But would that set up work ok?
```

---
