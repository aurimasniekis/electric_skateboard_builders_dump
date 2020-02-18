# Battery that fits Vesc specs

### Replies: 26 Views: 307

## \#1 Posted by: curtis Posted at: 2019-12-16T13:51:02.670Z Reads: 64

```
I am trying to figure out all I can about dual vescs.

Which ones can support four wheel drive? Can you please give the vesc's specs. Aka what voltage and amps they support. How fast I can push my board. Basically trying to figure out how big of a battery I can create with a given vesc?

I believe the flypsky 6.xxx can be wired for 4 wd. Is there any other vescs that support 4wd?

Curtis.
```

---
## \#2 Posted by: Benjo Posted at: 2019-12-16T15:23:45.560Z Reads: 63

```
Is you question about battery configuration or vescs? I don't get it.
You can use any Vesc and just connect two in the front and two in the back via CAN, both the front and back with their own receiver. Most Vescs max out at 60v (12s) and <100A, the 75/300 can do 75v (16s) and 300A.
Battery depends on your motors and how much you want to push them. Also which cell your will use. Anything from 8p to 12p could be reasonable.
```

---
## \#3 Posted by: curtis Posted at: 2019-12-16T23:57:50.667Z Reads: 55

```
I named the post battery that fits vescs specs.
The 2 different battery diagrams I set up are 720 watt hours. 12s 3p
The other set up I have is 840 watt hours.  352.8 volts I think it's 21s 3p

So I figured it out 12s 12p 720 watt hours.
```

---
## \#4 Posted by: curtis Posted at: 2019-12-17T00:38:35.378Z Reads: 48

```
https://drive.google.com/drive/u/2/recent

and https://drive.google.com/drive/u/2/my-drive
```

---
## \#5 Posted by: Tinp123 Posted at: 2019-12-17T06:42:10.391Z Reads: 43

```
every vesc supports 4wd

all esc are good up to 10s, some are good up to 12s and only few are good up to 13s. please do not use 21s battery, you will destroy your vesc immediately. also 21s battery can't output 352.8 volts, you got something wrong here?

as for cells in parallel, only limit is how many you can fit on your board
```

---
## \#6 Posted by: Benjo Posted at: 2019-12-17T07:40:56.914Z Reads: 41

```
21s would be 77.7v. I am not aware of an esc that can handle that. 
The natural choice would be 12s. And 3p is way too low for a 4wd setup, even with high discharge cells. Think about it, even with 35A per cell, that is only ~26A per motor (absolute maximum). If you dont want to use toy motors you will need 8p+.

You didn't upload any pictures btw, you just posted links to your private google drive that noone can access.
```

---
## \#7 Posted by: tex Posted at: 2019-12-17T07:52:16.729Z Reads: 36

```
Im a little bit confused about the 21s, why all these batteries in series?
And if is possible what kind of motors will you use?
```

---
## \#8 Posted by: curtis Posted at: 2019-12-17T15:35:19.692Z Reads: 33

```
So I am going to have 2 batteries and 2 vescs. 12s 6p. The diagram has 6 negative batteries facing up. then 6 batteries connected in series. Then then 6 batteries on the bottom with positive facing down.
I changed my mind I am going to split them into 2 12s 3p.

What do you mean parallel is the limit?  Series should be the limit?

Curtis
```

---
## \#9 Posted by: tex Posted at: 2019-12-17T22:05:18.252Z Reads: 28

```
I think with pararel, he means the space that you are able to use on your board.
```

---
## \#10 Posted by: Tinp123 Posted at: 2019-12-17T22:24:11.838Z Reads: 27

```
Yep exactly! Parallel has no number limit, only limit is how much cell could you put in your enclosure
```

---
## \#11 Posted by: curtis Posted at: 2019-12-17T22:49:13.471Z Reads: 26

```
Exactly!  I want my battery to last longer. Series 12s is pretty much the limit. 12s 6p sounds logical
```

---
## \#12 Posted by: Benjo Posted at: 2019-12-17T23:21:37.947Z Reads: 24

```
I am not sure, either I am slow or you are writing a lot of confusing and contradictory things. Do you want 12s12p? 12s6p? 21s anything? 3p?
Also what even is the question here?

Please be concise about what you have and what you want.
```

---
## \#13 Posted by: Tinp123 Posted at: 2019-12-17T23:29:59.260Z Reads: 24

```
@curtis if you have enough space, go with 12s6p samsung 30Q battery. That will be 778Wh battery. It will be enough even for 4WD. If you have more space and money, go with 12s7p or 12s8p. Anything bigger than 12s8p will only fit in custom top mount box or Lacroix deck and enclosure. There is no need for further philosophy.
```

---
## \#14 Posted by: curtis Posted at: 2019-12-19T04:54:14.361Z Reads: 22

```
I would go with 12s 3p one battery then 12s 3p another battery and 2 dual vescs. How far distance could I push on average with a 12s 8p setup 4 direct drive motors?
```

---
## \#15 Posted by: curtis Posted at: 2019-12-19T04:59:09.253Z Reads: 22

```
Don't worry about it I got another post for that focus on the battery.
```

---
## \#16 Posted by: curtis Posted at: 2019-12-19T05:00:59.818Z Reads: 18

```
LOL dude go to the top my friend.
```

---
## \#17 Posted by: Tinp123 Posted at: 2019-12-19T06:07:02.461Z Reads: 17

```
you don't need two batteries for 4WD, you can wire two connectors out of battery or if you gonna use anti spark, you can wire two connectors in Y (parallel) after anti spark. 

you will have range anywhere between 30-90km on 12s8p.
```

---
## \#18 Posted by: Benjo Posted at: 2019-12-19T08:33:16.984Z Reads: 15

```
@curtis Whatever you say 😂
```

---
## \#19 Posted by: curtis Posted at: 2019-12-19T14:47:58.878Z Reads: 14

```
I can convert but just to let you know I live in United States and am on the central system. 18.6 miles to 56 miles
```

---
## \#20 Posted by: meesie Posted at: 2019-12-20T09:31:41.767Z Reads: 12

```
You said 3p gives low amps per motor, but keep in mind you have 4 motors. On a 2wd setup each motor would ask say 40 amps for hard acceleration for example. To get the same acceleration on a 4wd setup each motor would only need 20 amps. 

Anyhow, get two dual vescs or four single vescs, Doesnt matter which ones as long as its not flipsky. You can connect two duals with canbus i believe, or connect em all with ppm splitters.


As far as batteries go, A 12s5p would probably be okay. But if you got the space and money for it you can go for 12s8p or something like that. You don’t have to max out on the vesc specs because you’re probably never gonna draw that much.

Good luck!
```

---
## \#21 Posted by: curtis Posted at: 2019-12-20T15:37:32.016Z Reads: 12

```
? why not flypsky?  Where are you getting 12 5p? Which vesc would you recommend?
```

---
## \#22 Posted by: meesie Posted at: 2019-12-20T16:37:08.342Z Reads: 11

```
flipsky is less reliable than others.

got it custom built.

any.
```

---
## \#23 Posted by: curtis Posted at: 2019-12-31T02:17:04.814Z Reads: 9

```
What do you mean custom built? I need 2 dual vesc I am going to run 2 12s 3p.
```

---
## \#24 Posted by: meesie Posted at: 2019-12-31T11:02:20.031Z Reads: 8

```
[quote="curtis, post:21, topic:104772"]
Where are you getting 12 5p
[/quote]

A friend of mine built my battery, that’s what i meant with custom built.

[quote="curtis, post:23, topic:104772"]
I need 2 dual vesc
[/quote]

You need 1 vesc per motor. If you have 2 motors you can choose between 2 dual vescs (2 in 1) like the focbox unity or 4 single vescs.
```

---
## \#25 Posted by: curtis Posted at: 2019-12-31T21:25:43.603Z Reads: 7

```
No my dude I want 4 wheel drive. 4 motors that means 2 dual vescs.
```

---
## \#26 Posted by: curtis Posted at: 2019-12-31T21:29:41.500Z Reads: 7

```
Ok then which vesc do you recommend then?
```

---
