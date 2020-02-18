# Using Boosted v1 Parts to make a DIY Board (VESC/BMS/controller)

### Replies: 16 Views: 278

## \#1 Posted by: sameerpinheiro Posted at: 2019-07-01T18:25:12.960Z Reads: 72

```
Hello everyone,
I have a v1 boosted board in great condition. It charges, its remote is working properly, and its motors are running smoothly. The problem is, I wanted something that can go for more then 3 miles. I considered building a Foosted board from scratch, but what puts me off the most is the controller systems they use. I like the v1 controller, and I wanted to know if I can do the following.
Take Board Apart.
1. Add Caliber II trunks
2. 85 Orangutang wheels, with kegel system
3. TorqueBoards 190 kV 6355 Outrunners
4. TorqueBoards reverse motor mounts, TorqueBoards 12mm Kegel pulley/belt kit

In other words, making a Foosted board.
Now this is where I wanted some opinions. I Wanted to Re-use my BMS, VESC, build a Samsung 30q cells in a 10S4P inside one of 
https://www.eboardsperu.com/product/loaded-vanguard-enclosure-set-10s4p/
I really wanted to maintain the Boosted controller, and options, but Im worried that the ESC will limit the battery, and It will ultimately hinder the speed.

I wanted to Use as Much as possible of what I have.
```

---
## \#2 Posted by: pjotr47 Posted at: 2019-07-01T19:19:43.870Z Reads: 65

```
If you are going to take that board appart I want to buy the battery with original bms. 

I have a used boosted v1 laying with a broken battery.
```

---
## \#3 Posted by: sameerpinheiro Posted at: 2019-07-18T16:34:37.714Z Reads: 47

```
I would gladly give it to you, let me just check if its working still. I have 2 gen 1 boards, one of them came for parts, other I decided I wont mess too much with. Il check the BMS this weekend, (problem is im in Brazil, so shipping might suck haha), if they work, il give it to you, just cover the shipping.
```

---
## \#4 Posted by: AlanZhou Posted at: 2019-07-18T16:46:55.107Z Reads: 44

```
Boosted v1 runs on 12S Lipofe4 which is 39.6V max.

Using 10s 18650's won't be compatible with the bms.

It you change out the original bms, than the controller won't be able to read voltage.
```

---
## \#5 Posted by: sameerpinheiro Posted at: 2019-07-18T16:51:25.713Z Reads: 43

```
So I can add Lipofe4, such as the 6s1p one 32700 ones?
```

---
## \#6 Posted by: AlanZhou Posted at: 2019-07-18T16:58:46.229Z Reads: 45

```
Nope gotta be 12s Lipofe4
```

---
## \#7 Posted by: sameerpinheiro Posted at: 2019-07-28T14:32:00.299Z Reads: 35

```
One thing I dont understand very well is the 39.6v the board uses. If it has 12 cells at 3.2-3.3, it makes sense that it totalizes 39.6v. I know mixing chemistries isnt good, but I saw some people adding 4 zippy's 4200 13.3v to the board, wouldnt 3 be the ideal amount? Hypothetically, if I wanted tl add range, and i added 10s at 39.6v (with a separate bms), would it still be considered mixing lf chemistries if they have separate bms?
```

---
## \#8 Posted by: AlanZhou Posted at: 2019-07-28T14:32:40.806Z Reads: 31

```
[quote="sameerpinheiro, post:7, topic:97654"]
zippy’s 4200 13.3v
[/quote]

lipo's dont come in 13.3v
```

---
## \#9 Posted by: sameerpinheiro Posted at: 2019-07-28T14:32:48.751Z Reads: 30

```
Im referring now to the possibility of adding extra cells to existing ones.
```

---
## \#10 Posted by: AlanZhou Posted at: 2019-07-28T14:33:13.413Z Reads: 28

```
Huh then add Lipofe4 cells, the same ones that boosted uses
```

---
## \#11 Posted by: AlanZhou Posted at: 2019-07-28T14:33:36.333Z Reads: 29

```
[quote="sameerpinheiro, post:7, topic:97654"]
would it still be considered mixing lf chemistries if they have separate bms?
[/quote]

yes it would.
```

---
## \#12 Posted by: sameerpinheiro Posted at: 2019-07-31T04:53:01.079Z Reads: 27

```
thanks @AlanZhou!
```

---
## \#13 Posted by: sameerpinheiro Posted at: 2019-07-31T16:32:24.216Z Reads: 24

```
let me pick your brain on another idea, sorry to bother so much! If I was to open a boosted v2 battery SR, and attach it to positive and negative, with the v2 BMS, keeping in mind that I would charge them separately, would it work? Since they would both be Lipo4, im trying to think of an easy solution, to extend the range of the v1, without payng too much and being safe. Ive seen sone V2 SR going for less then 100 dollars.
```

---
## \#14 Posted by: walleywalker Posted at: 2019-07-31T17:34:13.807Z Reads: 24

```
My understanding is that the VESC and the BMS cannot operate independently from one another because they use a secure CAN bus protocol. 

If you want more range, really the only thing you're going to be able to do is make a 12s2p a123 LiPoFe4 battery and then solder up the OG Boosted BMS to that. You'll need a custom enclosure.

Also not sure if you'll be getting the full potential out of those 6355 motors as the wattage from the Boosted Boards is limited by the VESC, not the motors.
```

---
## \#15 Posted by: sameerpinheiro Posted at: 2019-08-01T13:50:19.041Z Reads: 18

```
Hum, makes sense! I thought that by simply adding another battery without a BMS directly to the VESC + and -, if it is within the same chemistry, would allow the boosted boards BMS to also control it. Having to open up the preexisting battery, remove the BMS (making sure not to fry it), then buying the same a123 cells, and putting everything into an enclosure seems way to much work! 
in this scenario @walleywalker I wouldnt use the 2 6355 I mentioned, rather, just adapt onto a pre-existing boosted v1 board an extra battery pack. 

I actually started this thread because I have a functioning boosted v1, but at max speed, I only manage 3.5 miles TOPS. I love the board, but ultimately, it is a waste of potential! I wanted to do something with it, so I thought of stripping it, or adding new motors/lion battery system, but all these ideas are very costly, and it would be cheaper to BUILD a board from scratch. I decided to find a way to add more cells to it, but, in a safe way! I saw one user adding 2 packs of 10s 18650, and he did a very thorough job with voltage regulations, even without a BMS. I am not experienced enough to even consider anything like this, I wanted something safe (ish), "easy", and not THAT expensive. That's why I thought of using a "old/used" boosted v2 SR battery, opening it up, taking out the BMS (or not, depending if it would work), and attaching it to the + and -, like the person did in this video. I know he explained very well about how mixing chems can be OK, and how he has been using his setup for 2 years, but on the safe side, I would mimic his plans with Lipo4 cells (I am assuming that even without a BMS, they would be SAFER-ish to use, considering at least there wouldn't be mixing of chemistry, and they are safer in general).

the video I refer to is this one 
1. https://www.youtube.com/watch?v=eAuGvzz8VdY&t=195s
and this one
2. https://www.youtube.com/watch?v=dEED8037tKk&t=275s  

The problem I am having is Location. I am in Brazil at the moment, and will remain here for the next year or so. Getting parts shipped here is a pain in the ass, especially battery cells. I cannot stress enough how hard it is, as an example, the  "best" deal we can get here, on what we can assume are original samsung 30q is around 15 dollars per cell. 
A friend has a SR v2 battery he said I can have for cheap, so I am trying to figure out a plan to use them.

Thank-you again for reading/responding to my post. As I mentioned, I am very inexperienced, But I  have been reading as many posts as I can, even when most of the information I come across seems Alien to me. After about 3 months of constant reading, I am now understanding most of the basic concepts, like how I need 12s1p at least, to have the correct 39.6v using a123. Sorry if I said anything too incorrect, and thank you all for helping me, it has been really great!
```

---
## \#16 Posted by: Dog Posted at: 2019-09-01T06:06:19.947Z Reads: 11

```
Is it 100% true that you can make a 12s2p lipofe4 with the OG v1 bms in a custom enclosure?
```

---
