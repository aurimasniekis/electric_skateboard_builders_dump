# Balancing/Equilibrium Board vs BMS. Whats the difference?

### Replies: 7 Views: 2709

## \#1 Posted by: evoheyax Posted at: 2016-08-09T01:12:36.354Z Reads: 221

```
Maybe someone on here can clear this up. What's the difference between a Battery Management System and a Balancing/Equilibrium Board?

It seems like the BMS controls the electrical flow and helps prevent overcharging/over discharging while the Balancing/Equilibrium Board just keeps the cells balance. Is this interpretation correct?

I think for anyone running a vesc, a bms is a bit of an overkill if you just need to keep cells balanced, and a Balancing/Equilibrium Board does that... thoughts?
```

---
## \#2 Posted by: chaka Posted at: 2016-08-09T01:30:41.875Z Reads: 218

```
LVC using the VESC at pack level is useless to protect the pack if you have a failing cell. The bad cells in the pack will drop below safe levels before the pack voltage trips LVC. This ends up killing all the cells in that paralleled pack and if you are unlucky enough to get reverse polarity you could end up losing the whole pack. One way around this is by building a tesla style pack with cell level fusing.
```

---
## \#3 Posted by: evoheyax Posted at: 2016-08-09T01:38:41.267Z Reads: 214

```
Would a bms have any help in stopping this? My understanding is the bms only balances the cells at the end of a full charge, and it monitors the whole battery packs voltage, not each parallel cell. Also, how would you fit 60 fuses into a battery pack without adding to the size? Have you tried this yet?

What do you think overall is the best way to keep cells balanced with the least amount of space? This is why I was looking at Balancing/Equilibrium Boards, as they seem to be much smaller than a bms.
```

---
## \#4 Posted by: chaka Posted at: 2016-08-09T01:46:43.403Z Reads: 200

```
A bms also monitors individual cell voltage and shuts it down if one strays too low. I build my packs using cell level fusing, just as compact as using nickel strips. You can then use an appropriately sized mains fuse for the whole pack to guard against short circuit and over discharge.  You want the mains fuse to blow before blowing your cell level fuses.
```

---
## \#5 Posted by: evoheyax Posted at: 2016-08-09T01:55:00.331Z Reads: 208

```
lol, jesus. You are man. Any chance of getting you to make and sell me a custom pack? haha that's more effort than I can put into it.

Also, I was looking at the ES thread about nickel strips and the amp ratings of the nickel plating was horrible. The thickest one the guy tested was only good at like 35 amps. What size do you use?
```

---
## \#6 Posted by: Randyc1 Posted at: 2016-08-09T02:08:37.378Z Reads: 226

```
Are there any "How To" Videos of cell level fusing technique? for our application in e skates?
```

---
## \#7 Posted by: Kaly Posted at: 2016-08-09T19:12:48.924Z Reads: 202

```
Tesla uses fuse metal strip attach to each cell wich then are group in parallel packs, this metal strip will take around 5 mm of space to make it workable and with the constrains that we have, we just can't afford to waste that much space. 

And this is not a prevention method ratter a damage control one, because it just come into action in the case of extreme over discharge or cell extreme failure, by this time the cell in question is already dead and the pack compromise due to the capacity of one of its components been severely damage, this method is engineered to prevent runaway effect cause by the damage cell that can result in dangerous situation ( fire) by effectively cutting this dead/dangerous cell out off the pack. 

Can you please show us a pic or explain in concept how can you achieve this, with the high cell density you like to pack in your built ?
```

---
