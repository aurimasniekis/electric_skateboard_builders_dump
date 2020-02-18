# Battery percentage meter

### Replies: 5 Views: 823

## \#1 Posted by: MrDGOrman Posted at: 2018-07-27T09:53:48.712Z Reads: 184

```
Hi everyone,

I purchased this battery percentage meter and I have a question.
https://www.ebay.co.uk/itm/LY6-8-63V-Lithium-ion-Lead-Acid-Battery-Meter-Capacity-Tester-Monitor-Indicator/152998863677

So I've got 3 Zippy Flightmax 5000mah LiPo batteries (3s1p per battery). With that in mind, based on the sellers instructions, I put 9c in the settings (9 cells overall). Have I done that right or would it be 3c as it's 3 batteries? I'm guessing I've done it right as a full cell is 4.2v. I can't tell if this takes into account that LiPo batteries shouldn't be full drained and should have 3.2v remaining in them (I think?)

Basically my concern is that I've covered about 5 miles today and I'm showing as having 73% battery left. I thought I would only get about 8 miles range?

Anyone able to help with this?

Thanks,
Daniel
```

---
## \#2 Posted by: FredrikHems Posted at: 2018-07-27T09:59:59.937Z Reads: 164

```
I guess you have serie connected your batteries in to a 9s/33,3v battery? If so, then you should set the battery meter to 9c. (Which means 9 cell in series) :grinning:
```

---
## \#3 Posted by: MrDGOrman Posted at: 2018-07-27T10:04:45.399Z Reads: 162

```
@FredrikHems I've got my batteries set up like the below image but 3 rather than 2.
http://www.skyhighhobby.com/wp-content/uploads/2011/04/lipo-SERIES-connection.gif

I've selected 9c which I thought was right, but the next question - is this device smart enough to know that there is a "safe limit" with LiPo batteries? If not and it judges from 4.2v to 0v then we/I would need to set up the meter to a smaller number of cells to get the correct "remaining" life which works with the safe limit on the LiPo batteries.

4.2v per cell to 0v = 9c?
4.2v per cell to 3.2v = ?

Cheers,
Daniel
```

---
## \#4 Posted by: FredrikHems Posted at: 2018-07-27T10:24:26.134Z Reads: 141

```
I have never been a fan of these cheap battery meters myself, as i feel like they are way to inaccurate. If you can get your battery meter to show voltage instead of percentage, that will be much better. Also you cant set a voltage cut off on these things.. 
Btw If you are using lipos i would recommend you to not drain them past 3.6v. Run them below that and you will shorten their life alot, for just a tiny bit more range.
```

---
## \#5 Posted by: MrDGOrman Posted at: 2018-07-27T11:15:28.860Z Reads: 129

```
So I've done some maths and this is what I've found.

![image|637x500](upload://8v1fl7B1kTIyl7UoM0SOtHwSgk8.png)

Basically, based on those calculations I would have somewhere between 33%-35% remaining. Concluding that the battery percentage indicator doesn't take into account a minimal voltage level which is totally understandable.

Is there anything on the market that's the same size but will allow you to put in max voltage and minimum voltage and then calculate the percentage based off of that? It's a lot more effective that way.

Cheers,
Daniel
```

---
