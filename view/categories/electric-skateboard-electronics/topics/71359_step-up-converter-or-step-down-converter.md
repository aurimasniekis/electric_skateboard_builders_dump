# Step-Up Converter (or step -down converter)?

### Replies: 5 Views: 201

## \#1 Posted by: TheGreekGuy Posted at: 2018-10-16T01:57:27.446Z Reads: 56

```
Hi All,
I'm gathering parts to build my own Esk8board and I had an idea. 
Since I have two 36V 10S3P batteries and my controller is rated up to 48V what if between the batteries and the controller I put a step-up converter
(I bought this from ebay to test it out: https://www.ebay.com/itm/900W-DC-DC-Boost-Converter-8-60V-To-10-120V-15A-Step-Up-Power-Supply-Module-US/291861952982?ssPageName=STRK%3AMEBIDX%3AIT&_trksid=p2057872.m2749.l2649 )
is this a viable idea?
```

---
## \#2 Posted by: mynamesmatt Posted at: 2018-10-16T02:04:09.241Z Reads: 54

```
hello my friend. if you had read some other posts first, you would have learnt that your controller is "rated" to 48v, it means this is the MAXimum your controller can handle. If you put your 2 10s3p packs in parallel, you'll a) get double the range b) be able to pull more current and c) not have issues with your esc.
That up converter can only push max 15a. your esc will need more than double this and it will be very ineffecient as it produces heat.
So in short, no, not 

[quote="TheGreekGuy, post:1, topic:71359"]
a viable idea
[/quote]
```

---
## \#3 Posted by: skatardude10 Posted at: 2018-10-16T02:13:17.620Z Reads: 49

```
Hmm, I hear you can put multiple boost/buck converters in parallel to carry higher loads. 

It might be possible to get like 4 - 6 boost converters and boost your voltage that way to carry the load :-) 

If you only want 20 amps or so, maybe two boost converters :-)
```

---
## \#4 Posted by: mynamesmatt Posted at: 2018-10-16T02:38:24.654Z Reads: 42

```
yeah it'll work. But why?
```

---
## \#5 Posted by: skatardude10 Posted at: 2018-10-16T02:51:28.016Z Reads: 41

```
hmm... why not I guess lol. 

![whynot|690x393](upload://dvxjEfNkDQemnToMhgq3n0JcA9Y.png)
```

---
