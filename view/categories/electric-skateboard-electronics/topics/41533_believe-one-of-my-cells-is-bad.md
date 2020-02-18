# Believe one of my cells is bad

### Replies: 12 Views: 877

## \#1 Posted by: keegancdr Posted at: 2017-12-20T07:05:25.288Z Reads: 205

```
So I have ridden my board about 6 or 7 times now, always ride it from 100% down to about 30-40%. Yesterday I was trying to test the distance of the board and I basically ran it down to 0% on the battery. Now this is an enertion spacecell 10s3p pack so it has a built in BMS and running dual VESC with proper cutoff voltage. 

So when it hit zero I felt the board jolt slightly and then power down.

I took home plugged it in, and after about 3 minutes of charging I turned it on to see if my screen would turn on again to show voltage. Green light lit up and showed about 4% or something like that. So I turned the board off and then left it to charge back up to 100%. 

Today when I went to grab the board, I pulled it off the charger and the very moment I clicked the on button to turn it on, I heard a tiny little pop sound and could smell a very faint but distinct burning smell. 

The voltage read out actually turns on however it shows 0% and no green backlighting. 

I took a look inside the battery bay and I do not see any issues with the cells themselves. And I cannot see anything melted anywhere on the connections. 

Any theories as to what happened here?

Here are some pictures of the BMS, and I typically have it wrapped in electrical tape for insulation. 

In the following pictures I have the voltage read out coming off the xt90 showing 31.6v and the voltage readout showing 0%. 

<img src="/uploads/db1493/original/3X/7/9/79a902c8529aae714db2bbe1a67661e12a856843.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/5/8/58b115a7fea92cc0538425324bcb75c8f3345bb2.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/e/c/ec6958a711000a4a2ca4b8d11cc8681083a2de96.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/0/8/08b4183e2fe653e93f3a3ea45411092365e9ea6a.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/3/d/3d6756ca3cf5df46b873a90dbebe93486117e02b.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/6/2/629ed3ab3dba408bc1b9e82b5a9641e950f2271e.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/5/7/578a52d60731760d06ba2cb2478f23a1e3a4795e.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/d/d/dd01228f73fb4de58304ce63a8922cdf64fb454a.JPG" width="375" height="500">
```

---
## \#2 Posted by: b264 Posted at: 2017-12-20T07:35:28.880Z Reads: 178

```
Can you use your nose to try to figure where (which board) the burn smell is coming from?  It fades, so do it soon
```

---
## \#3 Posted by: keegancdr Posted at: 2017-12-20T08:01:42.241Z Reads: 171

```
Ok, I used my nose and I think I have found the issue. Thank for the tip! I traced the smell back to one of the BMS balance wires. It looks like the small tab that I have spot welded on here has come free.  Which leads to my next question. If that had popped off during charging, would the BMS have even charged those cells properly? Would I need to pull it apart and balance charge that 1s?

https://media.giphy.com/media/26FfbhUY6eycMYS8o/giphy.gif
```

---
## \#4 Posted by: lowGuido Posted at: 2017-12-20T08:24:53.277Z Reads: 160

```
ahh the old using your nose technique. good tip!

although @keegancdr I think that your issue sounds like a component failure possibly caused by your loose connection.
```

---
## \#5 Posted by: keegancdr Posted at: 2017-12-20T16:21:01.014Z Reads: 135

```
When you say a component failure what do you think it could be failing?
```

---
## \#6 Posted by: lowGuido Posted at: 2017-12-20T16:25:06.730Z Reads: 134

```
if I were to guess I would say one of the FETS, but im only guessing, you would have to have a more thorough investigation. 
just the fact that you said pop and smoke makes me think that..
```

---
## \#7 Posted by: chuttney1 Posted at: 2017-12-21T06:34:56.016Z Reads: 110

```
Add a few layers of packaging tape or Kapton tape to the balance lead and call it a day. I assume it's just the balance lead rubbing on the cell's wrap.
```

---
## \#8 Posted by: keegancdr Posted at: 2017-12-21T16:35:05.888Z Reads: 83

```
Why do you think it was reading out 31.6v ?
```

---
## \#9 Posted by: chuttney1 Posted at: 2017-12-21T19:57:25.741Z Reads: 73

```
That happens to be normal range of a 10S pack. I personally would check the voltage to make sure none of the cells are shorted, but the shorted one would be warmer than the normal ones when charging. Then there's the part of I'm not sure what the voltage cutoff you set on the VESC versus the one set by the BMS.
```

---
## \#10 Posted by: keegancdr Posted at: 2017-12-21T20:11:57.490Z Reads: 69

```
do you think it is possible that the loose balance wire caused that particular cell to not charge at all, or potentially that the bms didnt allow any charging because it wasnt properly reading correctly?
```

---
## \#11 Posted by: chuttney1 Posted at: 2017-12-22T06:02:31.422Z Reads: 55

```
If the loose balance wired was rubbing on the cell wrapper till it caused a short, it's possible, but then this would be the one cell to not charge. It's unlikely a loose balance wire cannot cause a cell to charge as the purpose is to give a voltage readout for the BMS. I'm unsure how to go about this. Does the cell wrapper where you found the balance wire was exposed? It looks like it was exposed in the gif.
```

---
## \#12 Posted by: keegancdr Posted at: 2018-01-03T23:00:02.788Z Reads: 43

```
So does anyone recommend a good replacement BMS? I think mine may be shot?
```

---
