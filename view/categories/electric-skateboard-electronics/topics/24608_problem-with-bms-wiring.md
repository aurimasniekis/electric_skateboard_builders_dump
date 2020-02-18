# Problem with bms wiring

### Replies: 13 Views: 996

## \#1 Posted by: Jammeslu Posted at: 2017-06-05T11:16:01.374Z Reads: 120

```
As you can se in the picture the connector doesnt fit, its 2 3s zippys connected in serie with that connector which has 7 pins but the bms says its for 6s and only has 6 pins, it came with A 6 pin connector but it doesnt seem right pls help
```

---
## \#2 Posted by: Namasaki Posted at: 2017-06-05T16:14:03.729Z Reads: 109

```
The bms only has 6 pins and wires because it doesn't use the ground wire from the Lipo balance plug
```

---
## \#3 Posted by: Jammeslu Posted at: 2017-06-05T16:46:30.915Z Reads: 105

```
Which wire should i cut? <img src="/uploads/db1493/original/3X/d/1/d149d52c94b9f9d304af8e6a046be1787113ed8e.JPG" width="281" height="499">
```

---
## \#4 Posted by: Namasaki Posted at: 2017-06-05T17:40:58.472Z Reads: 97

```
The black wire on the outer edge of the 6s connector. 
_CAUTION_
It is absolutely critical that you connect the batteries in the correct order concerning their main power leads and the the balance wires. If you get it wrong, you will short out the battery. 
Battery 1 and Battery 2
 Battery1's red main connects to  battery2's black main
Then, 
Battery 1  supplies  main negative wire and balance wires 1,2,3
 Battery 2 supplies  main positive wire and balance wires 4,5,6
On the Lipo balance connectors, the red wire on the outer edge is always the last cell in the pack.
```

---
## \#5 Posted by: Jammeslu Posted at: 2017-06-05T20:03:23.508Z Reads: 79

```
I got the series connection right so if I'm understanding this 
battery 1 which is lead neg, balance lead 1 black 2 white 3 yellow
battery 2 which is lead pos, balance lead 4 white 5 yellow 6 red 

btw is it connected from right to left on bms as the number there?
```

---
## \#6 Posted by: Namasaki Posted at: 2017-06-05T20:16:30.894Z Reads: 76

```
I might have a diagram already drawn. 
When I get home from work I'll look and post it here.
```

---
## \#7 Posted by: Namasaki Posted at: 2017-06-05T20:55:54.117Z Reads: 64

```
You got it wrong on battery 1
It's: 
Black = ground
White = 1
Yellow = 2
Red = 3
```

---
## \#8 Posted by: Jammeslu Posted at: 2017-06-05T23:02:00.794Z Reads: 61

```
But if baattery 2 is correct then Thats 7? And connector is only 6?
```

---
## \#9 Posted by: Namasaki Posted at: 2017-06-05T23:19:46.267Z Reads: 60

```
<img src="/uploads/db1493/original/3X/4/5/4594524ad71f6ef37fd1ed2e1833d1edb0f27f75.png" width="640" height="484">
```

---
## \#10 Posted by: Jammeslu Posted at: 2017-06-05T23:37:32.492Z Reads: 57

```
Thanks but its the ground thing that doesnt fit?
```

---
## \#11 Posted by: Namasaki Posted at: 2017-06-05T23:47:38.628Z Reads: 56

```
<img src="/uploads/db1493/original/3X/8/0/80997e905e21b7359016e3e9cb18ba3ef237db71.png" width="690" height="400">
```

---
## \#12 Posted by: Namasaki Posted at: 2017-06-05T23:49:51.661Z Reads: 55

```
the Lipo balance connector will not fit the bms.
You have to use the harness/connector that comes with the bms.
Cut the wires from the 6s end of your dual 3s to single 6s series adapter cable and connect the wires to the bms harness as shown in the diagram.
```

---
## \#13 Posted by: Jammeslu Posted at: 2017-06-06T08:17:04.764Z Reads: 52

```
Thanks alot, I hope i get it right
```

---
