# Mixing different type of lipos

### Replies: 12 Views: 464

## \#1 Posted by: dragopepper Posted at: 2018-01-25T15:42:37.250Z Reads: 89

```
I have here four lipo packs 2 * 5500mAh 45C 3s and 2 * 5500mAh 35C 3s. 
I would like to connect the 45c and the 35c each togther to 6s, and this both package in series so that the result is 6s 11000 mAh. 
Does it make sense, or could it be better, to stay by 2 packs each 5500mAh because of the gap between 45c and 35C ?
```

---
## \#2 Posted by: faithfulpuppy Posted at: 2018-01-25T15:56:31.347Z Reads: 88

```
It should be fine as long as you don't exceed 35c, which is like 175a
```

---
## \#3 Posted by: Exiledd_Top Posted at: 2018-01-25T16:05:11.239Z Reads: 81

```
Correct me of am wrong, but I think your wrong for the fact that they have different discharge rates, thus discharging the cells at different rate and making the cells get unbalanced
```

---
## \#4 Posted by: aigenic Posted at: 2018-01-25T16:15:15.763Z Reads: 73

```
I must agree with @Exiledd_Top the cells will probably get unbalanced due to a different discahrge rating, 35C will loose capacity faster, which means its voltage will be lower :)
```

---
## \#5 Posted by: Slak Posted at: 2018-01-25T16:51:43.167Z Reads: 60

```
I second that !
```

---
## \#6 Posted by: Giga Posted at: 2018-01-25T17:24:17.412Z Reads: 51

```
Since you have same capacity there should be no difference. Current is running through both packs, so I don't get why one would have voltage drift (like people above stated). And parallel packs even out voltage anyway. 
But usually you connect batteries from same batch (same specifications/capacity) in series and different capacities can only be connected parallel.
```

---
## \#7 Posted by: ducktaperules Posted at: 2018-01-25T19:07:21.726Z Reads: 42

```
If you connect a 35c and a 45c in parallel you basically create a large 40c pack. 

cells in parallel basically act as one cell. If your adding packs in parallel your basically combining the packs giving you a battery with twice the capacity and the sum of the current outputs. you can run lipos with different capacity's parallel without any problems. 

You will only have balancing issues if you have packs of different current rating or capacity's in series as this causes some cells to discharge at different rates.
```

---
## \#8 Posted by: Namasaki Posted at: 2018-01-25T20:12:20.969Z Reads: 39

```
[quote="faithfulpuppy, post:2, topic:44646, full:true"]
It should be fine as long as you don’t exceed 35c, which is like 175a
[/quote]
First of all, 35C 5500mah Lipos will not handle 175a.
C rating X  capacity gives a false current capability with Lipos. 
Second, as others have said, the two different Crated packs will not discharge evenly and voltage sag will be worse with the 35C
```

---
## \#9 Posted by: bartroosen12 Posted at: 2018-01-25T20:17:25.040Z Reads: 38

```
Just make 2 packs which you can swap 👌
```

---
## \#10 Posted by: longhairedboy Posted at: 2018-01-25T20:19:12.364Z Reads: 36

```
You're going to need one of these. 

https://i5.walmartimages.com/asr/dafc49d0-98d5-4a96-b1d5-ad6cc0a94240_1.1c178402db001d1b3eadde250633107a.jpeg?odnHeight=450&odnWidth=450&odnBg=FFFFFF

I recommend a more aggressive mix setting because you have to overcome a lot of potential energy in those packs. 

Once you have a smooth even mix you can slather the packs onto your board as needed.
```

---
## \#11 Posted by: faithfulpuppy Posted at: 2018-01-25T21:17:24.963Z Reads: 29

```
Dude I WISH I had a stand mixer. Do you know how hard it is to make a pie crust by hand while keeping the butter cold?
```

---
## \#12 Posted by: aigenic Posted at: 2018-01-25T21:19:48.960Z Reads: 28

```
I always wanted to have a mamooth...like it is cool to ride an electric skateboard, but just imagine riding a giant mamooth to school :D :D 

(Sorry for hijacking the topic, I just had to say it :D )
```

---
