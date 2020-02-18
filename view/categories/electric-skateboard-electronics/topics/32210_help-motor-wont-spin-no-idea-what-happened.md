# Help/Motor wont spin, no idea what happened

### Replies: 23 Views: 957

## \#1 Posted by: ARetardedPillow Posted at: 2017-09-04T04:57:30.758Z Reads: 82

```
I went for a little ride today but hit a pothole And my phase wires came loose, after that i replugged the phase wires and my motors wont spin, Ive already took apart my motor and checked that everything was alright and in tact but nothing works, I also checked the connections and they were well soldered too but I still resoldered them anyways, I plugged my vesc into bldc tool and everything seems to be alright just the motor wont spin, I also checked my remote an set up my spare, also didnt work, I dont have any other motors or esc that can test if anything is screwed up, the lights on the vesc still work
http://prntscr.com/ggrz1a
Im running a 10s setup with a sk3 6374 motor and a vesc from diy<img src="/uploads/db1493/original/3X/8/9/890f7023c8d4dbfc194d4f5b0033b1a6d8776a92.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/e/e/ee8c1718b6be16bafacac0ed5d24338d56c87cfd.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/2/9/299eb0a81c50c79e0acf2536a146da6f60282420.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/9/4/9436380e5ee6b235c796b4b05dd6bcff895c7965.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/3/9/39ec7521e70987a7e0facc8b3ff23b17288598dc.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/d/d/dd7b86720ff89b52be3c178e068b7b3531d06aea.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/2/d/2dcbdc83be0f594a81cbf283c107298029b5f5be.jpg" width="375" height="500">
```

---
## \#2 Posted by: Eboosted Posted at: 2017-09-04T05:44:15.297Z Reads: 76

```
Those phase wire were runing touching each other's copper? Or you removed the heat wrap before taking the picture?

If the phase wires got in contact in a high current moment, as in full throttle on acceleration, then your VESC could be fried.

Connect BLDC tool, go to terminal and type faults, report back. 

Try to do motor direction again without pulleys or belts attached to the motor and test again
```

---
## \#3 Posted by: ARetardedPillow Posted at: 2017-09-04T05:59:16.807Z Reads: 72

```
I dont think my phase wires got shorted during a high current moment (i had heat shrink on all connections and only 1 came apart) im going to plug it in to bldc tool rn
```

---
## \#4 Posted by: ARetardedPillow Posted at: 2017-09-04T06:04:05.051Z Reads: 74

```
<img src="/uploads/db1493/original/3X/2/a/2ae26fa189c97c70266e1b00152d5f6145ad4d7e.png" width="690" height="397">
says No faults registered since startup :/ I really have no idea whats wrong
```

---
## \#5 Posted by: Eboosted Posted at: 2017-09-04T06:18:52.954Z Reads: 68

```
Can you make motor detection?

Try to do it with no load and if nothing happens type faults again
```

---
## \#6 Posted by: ARetardedPillow Posted at: 2017-09-04T06:31:02.408Z Reads: 66

```
I cannot detect the motor but I typed faults again and it showed me this <img src="/uploads/db1493/original/3X/9/e/9ec65ef610a3e37ddabf8737a958b079dfd36053.png" width="690" height="406">
```

---
## \#7 Posted by: ARetardedPillow Posted at: 2017-09-04T06:32:02.087Z Reads: 63

```
I think I fried my drv chip, I was praying for this not to happen, do you know any solutions?
```

---
## \#8 Posted by: florensvb Posted at: 2017-09-04T06:50:43.382Z Reads: 63

```
I had the same issue with the DRV chip. seems to happen quite a lot on the diy vesc :( 
the only solution is to replace the drv chip. The good news is that the chip is cheap. The bad news is that it is super duper hard to get the soldering done, at least it was for me, as i had never attempted a smd soldering job before. I went for it anyways and ended up frying the rest of my vesc because i had some solder bridges between the little connectors. So if you think you can do it and you have the right soldering equipment: Go for it! Otherwise your only option is to find somebody to do it for you, or get a new vesc. I ended up getting the focbox from enertion after that .. Also see if red led on the diy vesc lights up in a repetitive pattern like '3 shorts'? That stands for the drv error.
```

---
## \#9 Posted by: ARetardedPillow Posted at: 2017-09-04T06:55:50.147Z Reads: 62

```
Yep.. I got the 3 red lights, I dont think I can replace the chip with the soldering equipment I have (13 dollar iron from amazon), and I dont think I can find anything to do it for me either so I think Im just going to get a new vesc, but I dont think Ill be getting one from diy anymore, Im thinking of ollins or a focbox, which one do you think is better and wont fry short term, Ive only put about 10 miles on this vesc
```

---
## \#10 Posted by: florensvb Posted at: 2017-09-04T07:10:20.736Z Reads: 58

```
I thought that ollin was the guy who owns enertion? So i think ollins vesc and the focbox are actually the same thing but please if somebody knows better then correct me. 

Like i said i ended up ordering the focbox from enertion and because of my worries that id fry a second vesc i also purchased the 1 year warranty with it. I read somewhere that the focbox has improved some of the regular parts on the vesc 4.12 to reduce the risk of drv errors etc and is definitely the best quality one out there. looking back i wish i had ordered that one immediately cause i spent so much money on stupid vescs haha.
```

---
## \#11 Posted by: ARetardedPillow Posted at: 2017-09-04T07:14:08.920Z Reads: 57

```
Hmm from what I see @chaka runs ollin an @onloop owns enertion, 

I wish I didnt cheap out either buying a 100 dollar vesc from diy, I was looking at the focbox and was freaked out by the price, Im a highschool student going into sophmore year so I really dont have much money to spend haha, I blew all my summer job money on this project and theres just piles and piles of problems, from batteries dying to bmses dying and now I fried my drv chip.
```

---
## \#12 Posted by: florensvb Posted at: 2017-09-04T07:17:41.170Z Reads: 57

```
Oh yeah you're right, i had actually never been on the ollinboards website before :D So i cant talk about how good his vesc is either. But the focbox has been doing a very solid job for me so far. 

Also you might wanna keep the diy vesc because the chip only costs a few dollars and if you can at some point in time manage to replace it, it will be as good as new (dual setup? :D )
```

---
## \#13 Posted by: florensvb Posted at: 2017-09-04T07:19:33.382Z Reads: 57

```
Just browsing ollinboars i would go for the focbox, because its cheaper and you could get a warranty with it. It also looks lighter cause its in a plastic housing
```

---
## \#14 Posted by: ARetardedPillow Posted at: 2017-09-04T07:23:01.774Z Reads: 55

```
Yea Im thinking of getting a soldering station with a heat gun sometime in the future so hopefully Ill either make a dual motor setup or an electric bike if I succeed, Im definitely going for the focbox, how long did it take yours to arrive? I want to get my board up and running before school starts which is in 3 days (yea im not going to get it in 3 days)
```

---
## \#15 Posted by: florensvb Posted at: 2017-09-04T07:41:47.703Z Reads: 52

```
For me it took like around 10 days i think, but I live in Hamburg, Germany and they are shipping from Australia, so not sure how that would vary for you. The support is great, you can just ask them anything in the chat and they will tell you
```

---
## \#16 Posted by: Eboosted Posted at: 2017-09-04T07:47:22.765Z Reads: 48

```
Post your VESC settings even the advanced tab ones, it might help you save the new VESC you are getting
```

---
## \#17 Posted by: ARetardedPillow Posted at: 2017-09-04T07:53:07.616Z Reads: 46

```
alright thanks a lot for the suggestion i will definitely be getting myself a focbox
```

---
## \#18 Posted by: ARetardedPillow Posted at: 2017-09-04T07:54:59.617Z Reads: 50

```
<img src="/uploads/db1493/original/3X/0/0/0096bbdb6339ccd0a68afa8e7306095619afb661.png" width="690" height="399"><img src="/uploads/db1493/original/3X/9/c/9c343e82ba2d48bc43eb73249259f1c3b738f015.png" width="690" height="383"><img src="/uploads/db1493/original/3X/6/1/61505a9fd7b608e54f04cde6c25a2c5b8186eb7f.png" width="690" height="389">
Im running a 10s setup 5x2s 5900 mah
```

---
## \#19 Posted by: ARetardedPillow Posted at: 2017-09-04T07:56:26.108Z Reads: 44

```
Correct me if I need to make any adjustments, Im still very new to this and I havent gotten my board in working condition for more than 2 days at once and Im still working on it and trying to improve it
```

---
## \#20 Posted by: Jinra Posted at: 2017-09-04T08:55:15.570Z Reads: 41

```
your commutation mode should not be on delay, you should be using integrate, you also need to do detection. Might be why it fried
```

---
## \#21 Posted by: pat.speed Posted at: 2017-09-04T10:15:17.352Z Reads: 40

```
You might be able to get @JohnnyMeduse to fix the Vesc for you
```

---
## \#22 Posted by: ARetardedPillow Posted at: 2017-09-04T18:47:34.992Z Reads: 27

```
Hmm I thought I had it on integrate the last time I checked and I did do detection, just that now my drv is fried and I cant do anything
```

---
## \#23 Posted by: ARetardedPillow Posted at: 2017-09-04T18:47:59.955Z Reads: 27

```
Hmmm time to scrap that diy repair idea
```

---
