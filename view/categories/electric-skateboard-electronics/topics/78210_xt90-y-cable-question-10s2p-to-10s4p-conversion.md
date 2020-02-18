# XT90 Y Cable Question (10s2p to 10s4p Conversion)

### Replies: 10 Views: 228

## \#1 Posted by: ICEBIRG Posted at: 2018-12-17T01:18:41.069Z Reads: 65

```
Hey guys, so quick question.

We are testing a new board that runs a AWD setup with 2 enclosures and 2 ESCs. Each enclosure/esc has one 10s1p pack. We were discussing today doubling the range and what that would take, and it seems to me all we would need to do is make risers for the enclosure and use y'cables to add in two more stock packs, making a 10s2p into a 10s4p. The problem is it occurred to me that I don't know if the Y splitters should be the in series or parallel type. Series seems to make the most sense to me, but I thought I would ask the pros, thanks!
```

---
## \#2 Posted by: J_Dizzle Posted at: 2018-12-17T01:25:27.997Z Reads: 63

```
Series will double the voltage, parallel will double the amperage. You want to go with parallel.
```

---
## \#3 Posted by: DilatedPupils Posted at: 2018-12-17T01:26:49.590Z Reads: 58

```
What esc are you using? How are you running  2 esc for awd?
```

---
## \#4 Posted by: J_Dizzle Posted at: 2018-12-17T01:28:24.422Z Reads: 57

```
He is probably running dual esc like flipsky or the cheap Chinese ones
```

---
## \#5 Posted by: ICEBIRG Posted at: 2018-12-17T01:33:43.851Z Reads: 52

```
They are two dual channel chinese ESCs from a Meepo boars. Designed to work in 10s config.
```

---
## \#6 Posted by: DilatedPupils Posted at: 2018-12-17T01:34:11.824Z Reads: 50

```
Right. I forgot about all them duals lol.
```

---
## \#7 Posted by: J_Dizzle Posted at: 2018-12-17T01:37:21.350Z Reads: 45

```
In answer to your original question, put the four 10s packs in parallel to get. 10s4p. From what I understand about your layout, you are putting the 4 packs into 2x 10S2P. and then putting those two packs in parallel again to get 10S4p. However if you do this your battery meter on your remote will no longer be acurate
```

---
## \#8 Posted by: ICEBIRG Posted at: 2018-12-17T03:48:22.759Z Reads: 33

```
Thanks a ton J_Dizzle! How would you do this in a better way to maintain the battery indicators?
```

---
## \#9 Posted by: J_Dizzle_2.0 Posted at: 2018-12-17T04:04:59.736Z Reads: 34

```
Attatch a seperate battery meter to the two main leads going to your esc, try this one:
https://www.amazon.com/ABT-Power-Battery-Indicator-Electric/dp/B071FKRDT2/ref=sr_1_fkmr0_3?ie=UTF8&qid=1545019329&sr=8-3-fkmr0&keywords=drok+10s+meter

It will give you a precentage way over 100%, but when looking at the voltage you can still see an acurate representation of how much charge you have left
```

---
## \#10 Posted by: ICEBIRG Posted at: 2018-12-17T04:20:13.104Z Reads: 30

```
Thanks a ton!
```

---
