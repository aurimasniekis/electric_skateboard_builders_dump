# Battery - one series won&rsquo;t charge

### Replies: 9 Views: 274

## \#1 Posted by: Marksmoura Posted at: 2018-12-20T22:02:23.633Z Reads: 90

```
Hello guys, I just finished building my first 10s4p 30Q pack. All went fine I connected everything and after charging for a while I decided to check if all the series were charging accordingly.

I found out that the first series pack is falling behind all the others. 
3.78V while all the others are at 3.93V.

Anyone has advice what's the steps I should take? What should I check first and replace? I was thinking first to charge the series individually until it catches up the others but why isn't the bms doing that already. Is the BMS broken? Or the batteries should be replaced? 

Anyone with experience about this kind of problem?
```

---
## \#2 Posted by: Hummie Posted at: 2018-12-20T22:18:00.233Z Reads: 91

```


  Are u sure they all started at the same voltage?  I’d slow charge n see if it balances. Probably a very slow discharge balancer.
```

---
## \#3 Posted by: AlanZhou Posted at: 2018-12-20T23:49:16.252Z Reads: 77

```
might be the bms, when the one cell group voltage is to different from the other cell groups the bms will not be able to balance it out i think .20v might be to much, try charging that cell group up by itself (balance it to the same voltage as the other series groups) than charge though the bms and see if it will work
```

---
## \#4 Posted by: Marksmoura Posted at: 2018-12-21T04:15:20.894Z Reads: 60

```
I will charge the group separately until it had the Same voltage and see if it works.
```

---
## \#5 Posted by: Marksmoura Posted at: 2018-12-28T22:27:32.092Z Reads: 44

```
Update so I charged manually until I had all cells around 4.08 and went for a quick 15min ride and somehow the first series dropped to 3.6 while all the others at 4.03.
Tonight I left the first series charging separately  the complete night, 8h, and my 4p pack went from 3.6 to 3.93.

Is there maybe a small short circuit discharging the cells? If so I wonder why it didn't dropped bellow 3.6, I guess the problem. Is not the bms. I have two new 30qs, I will order 2 more and substitute them.

Any opinions? Maybe one 30q is damage but I'm not sure how to find out which.
```

---
## \#7 Posted by: Noob-at-building Posted at: 2018-12-29T03:51:20.113Z Reads: 32

```
What Bms are you using? My friend has had lots of problems with cheap
10s bms
Also are you bypassing the BMS discharge?
```

---
## \#8 Posted by: Marksmoura Posted at: 2018-12-29T07:53:54.643Z Reads: 30

```
when charge just one series I don't use the BMS, I use a 4 slot lion charger when I welded two wires and insert them on the first two holes of the balance plug, which are the 0v and the first balancing lead so this way I can charge it but somehow very slow. Its a cheap one.

When I ride I bypassed the BMS for discharge, I use it just for charging unless its not enough current. I am using the BMS from sunkko, should be good. I am currently working in China so I get all very cheap, only the batteries are the same price because its Samsung.. 3€ each

As I write I am driving home, I left it charging the hole day, hopefully I can get it to the same voltage, after this I will ride it again and see if the same happens. In parallel I bought two batteries more and I will be substituting it, normally 2/3 days I have it.
```

---
## \#9 Posted by: Marksmoura Posted at: 2019-01-19T11:34:17.044Z Reads: 21

```
UPDATE:

I finally got the time to replace the faulty pack and now everything looks fine. It could be that one of the cells was faulty not letting others charge accordingly so I welded 4 new Samsung cells and replaced the series 4p pack. 

I am not sure what was the problem but the way I found it out was even after charging separately which would take longer to charge it would also discharge much quicker. It could be that some cells weren't properly making a connection and that would explain the faster discharge but it didn't explain the slow charge. 

After my last ride with my fault pack starting at 42V, at the end of my ride I had the fault pack at 3.6 and all the others still at 41V.
After I replaced I tested the welds and everything was good, I guess I was just unlucky with the cells I had on that pack but lucky enough just to have one series pack with the problem.
```

---
## \#10 Posted by: Noob-at-building Posted at: 2019-01-19T11:48:20.506Z Reads: 20

```
So you finally fixed it, good job man :slight_smile:
```

---
