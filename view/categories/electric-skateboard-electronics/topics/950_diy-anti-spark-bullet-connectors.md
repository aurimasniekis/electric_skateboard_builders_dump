# DIY Anti-Spark Bullet Connectors

### Replies: 9 Views: 2894

## \#1 Posted by: chaka Posted at: 2016-01-09T05:30:29.608Z Reads: 351

```
The picture says it all! I took a little break today while I had some VESC's in the oven and crafted this little gem. I used three 1K resistors to make it. 

I should add that I didn't just dream this up. I don't remember the source but I did find it on google images a few months back.

<img src="/uploads/db1493/original/2X/2/2952929de111fbe39eed24f3e5f3fd2f1fdcdcd2.jpg" width="690" height="488">
```

---
## \#2 Posted by: lowGuido Posted at: 2016-01-09T06:16:35.658Z Reads: 331

```
that's pretty cool. I had thought about doing this myself, but I didn't have any SMD resistors laying around.
did you use a dremel to cut the end off the socket?
```

---
## \#3 Posted by: chaka Posted at: 2016-01-09T06:54:15.982Z Reads: 325

```
I used a jewelers saw but a dremel would have worked just as well.
```

---
## \#4 Posted by: trbt555 Posted at: 2016-01-09T12:10:16.098Z Reads: 309

```
Cool idea !
How do you know the resistance is enough to prevent a spark ?
```

---
## \#5 Posted by: Blasto Posted at: 2016-01-09T15:41:24.335Z Reads: 289

```
Very clever, the idea here is to limit the current inrush cause by the bulk capacitor (the big cans) by placing a resistance directly in series with the rest of the circuit. 

Chaka's is placing 333 ohms in series with the rest of the circuit. If he is running a 40V system, that will allow a maximum of 120mA to charge the bulk capacitors and to reduce/eliminate the inrush current once the bullet gets to the end of the barrel.

How do you determine what resistance to put? Well, is 120mA enough to create a spark, I don't think so. Is 120mA enough to charge the bulk caps in a few mili seconds, probably 90% charge yes. You want that windowed sweet spot.
```

---
## \#6 Posted by: chaka Posted at: 2016-01-09T17:31:53.766Z Reads: 263

```
[quote="trbt555, post:4, topic:950"]
How do you know the resistance is enough to prevent a spark ?
[/quote]


They were resistors I had from another project.  There are calculations you can run to find the sweet spot but these should work fine. I tried it with a 6s pack but I will try a 12s pack later today when I am back in the shop to confirm.

Edit: 12s confirmed! Three 1k resistors is definitely the sweet spot.
```

---
## \#7 Posted by: longhairedboy Posted at: 2016-01-10T00:44:01.423Z Reads: 241

```
this is brilliant! a double layer of heat shrink and it would be tough enough to withstand regular disconnects for a while.
```

---
## \#8 Posted by: lowGuido Posted at: 2016-01-10T03:23:11.245Z Reads: 237

```
I got another tip for you,  drill a hole in a double sided PCB the same size as the internal diameter od the socket and solder the 2 pieces of socket each side trim off the excess and then solder your resistors on.
It will give the socket a bit of mechanical strength other than just that of the resistors.
```

---
## \#9 Posted by: chaka Posted at: 2016-01-10T06:51:14.731Z Reads: 227

```
Genius idea! It would be "bullet" proof.
```

---
