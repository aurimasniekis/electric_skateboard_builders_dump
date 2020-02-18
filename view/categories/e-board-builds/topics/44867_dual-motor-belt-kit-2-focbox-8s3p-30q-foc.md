# Dual motor belt kit, 2 focbox, 8s3p 30Q, FOC

### Replies: 15 Views: 641

## \#1 Posted by: Jammeslu Posted at: 2018-01-28T13:21:54.185Z Reads: 153

```
Hello esk8ters.

This will be my second build and i have learned a lot in the time i have been active here. 

So this board is for **pure commuting**  now since I will start "collage" now and I have to go by train. My commute back an forth is only 10km so I am not looking for range so I already know my pack is small ok you dint have to tell me. But I have seen the commute boards with 10s2p and its doable. I have it quite hilly here so a dual drive is a must and I want more torque than my current mono drive. I don't think there is more to discuss so here is the dilema. 


**The chinese dual belt drive kit** with no belt tensioning etc has two kinds of motors.
The one from diyboard. This is the reason I will be able to do a dual drive still with my budget of 600 us.

* Option one is the 5055 motors which is what I want the most because its cheaper but most of all its lighter! 
But this option is only available in **270kv** meaning i need to run **6s** to still reach my desired 40kmh. The pack will be a 6s3p with 30Q so a 60A con.

* Option two is the 6354 motors in **180kv** . this paired with a 10s2p 30Q pack will also reach 40kmh but adds weight and price.  but pack is only 40A con 

Here is where I need opinions. I am running two **focboxes in FOC** so 6s is more stable. 

The best is to run 270kv with 10s2p with erpm limit but is that safe in foc etc? 

help appreciated!


**Here is the list of the rest of my items.**

* Dual focbox

* A pack not deiced with 30Q I can buy from nkon from EU without VAT so price per cell is like 2.82 shipped.

* Besttech bms with antispark switch. if 10s3p I will try the 35A one since the pack can only max a 40A otherwise the 70A version.

* My board is either a Oxelo fishtail. really recommend it like its really fkn good. Wide and has concave etc. I am thinking of a board that is lurking around in the forum to.

* Custom glasfiber enclosure

* Firefly remote so no need of percentage display etc. 

Also the board is going to be fully waterproof.

yeah thats it bros
```

---
## \#2 Posted by: Martinsp Posted at: 2018-01-28T13:42:11.842Z Reads: 133

```
30Q in a 3P config is 45A since it is 15A per cell, unless you want to go hard on them and pull 20A per cell.

I have been running FOC with a regular 4.12 using the soft ERPM function to limit it to 55k ERPM. 10S and 245kv
```

---
## \#3 Posted by: Jammeslu Posted at: 2018-01-28T13:46:46.145Z Reads: 123

```
So limit erpm vs true kv match has no difference in foc reliability ? @Martinsp
```

---
## \#4 Posted by: Martinsp Posted at: 2018-01-28T13:58:35.494Z Reads: 125

```
Well it is hard to say for sure, I think it is more of a hit or miss (luck).
It is safer to go for a kv that is suitable for your battery but if you cant or dont want to for whatever reason it is OK to limit the ERPM and you should be safe as far as ERPM goes.

I would choose the 270kv if you want it more and go with 8S3P probably.
```

---
## \#5 Posted by: Jammeslu Posted at: 2018-01-28T14:09:31.870Z Reads: 108

```
ok will take into consideration. currently running 8s3p 30q with a 213kv motor. 

but with 8s and 270kv I will still need to limit the erpm so whats the difference between 8-10s then?
```

---
## \#6 Posted by: Jammeslu Posted at: 2018-01-28T14:10:42.254Z Reads: 98

```
is it because lower v and less to limit which makes it safer in foc?
```

---
## \#7 Posted by: Martinsp Posted at: 2018-01-28T14:16:40.801Z Reads: 95

```
With 8S you will have to pull more current to achieve the same power compared to 10S, that means more heat.

FOC is generally less stable than BLDC but with FOCBOX you should be safe with just limiting the erpm
```

---
## \#8 Posted by: Jammeslu Posted at: 2018-01-28T14:53:47.525Z Reads: 91

```
But Why did you recomend 8s instead of 10s then?
```

---
## \#9 Posted by: Martinsp Posted at: 2018-01-28T15:02:16.628Z Reads: 86

```
Oh, that was a misunderstanding I meant 8 instead of 6, you mentioned that you want to run the 270kv with 6s
```

---
## \#10 Posted by: Jammeslu Posted at: 2018-01-28T15:09:29.711Z Reads: 83

```
Aha Yeah now I get it. But then a last question. 

Would you take a 8s3p or 10s2p? Both limited erpm so both should have the same top speed?
```

---
## \#11 Posted by: Martinsp Posted at: 2018-01-28T15:11:12.107Z Reads: 83

```
I think 8s3p would be better because you also have to consider voltage sag
```

---
## \#12 Posted by: Nordle Posted at: 2018-01-28T15:14:11.619Z Reads: 74

```
I would rather build a decent single drive (63mm motor + vesc) than cheap out a dual.
```

---
## \#13 Posted by: Jammeslu Posted at: 2018-01-28T15:16:15.908Z Reads: 76

```
Thats What I have now. I want more torqe and I feel like I am stressig my motor on my long hills here in sweden
```

---
## \#14 Posted by: Sebike Posted at: 2018-01-28T15:22:24.134Z Reads: 76

```
add another 63xx motor then? :slight_smile:
```

---
## \#15 Posted by: Jammeslu Posted at: 2018-01-28T15:31:49.226Z Reads: 72

```
Doesnt fit the truck and if I want buy quality pulley and motor mount, longer truck and another motor I can buy that whole kit
```

---
