# Need Help with key loop

### Replies: 14 Views: 820

## \#1 Posted by: da_Qunster Posted at: 2018-04-06T03:29:43.039Z Reads: 142

```
Hey everybody,

So I'm currently working on my first build and it's coming along pretty well, until I tried building my anti spark key loop. I have two lipos connected in series with a series adapter going into another series switch which connects the anti spark key and the vesc. When I tried plugging in the key switch for the first time, there was a huge spark that basically fried one of my series adapters. Thankfully the batteries and vesc still work. So is there something I did wrong? And can someone tell me some specifics about how to build an anti-spark key loop? Should I just give up and buy a vedder switch instead?
```

---
## \#2 Posted by: bsancken Posted at: 2018-04-06T03:56:59.846Z Reads: 129

```
https://www.electric-skateboard.builders/t/how-to-anti-spark-xt-90-loop-key/204
```

---
## \#3 Posted by: da_Qunster Posted at: 2018-04-06T04:10:11.911Z Reads: 123

```
This was the first page I went to when researching. Everyone says that it's just a simple series adapter with a key switch that closes the circuit. I'm pretty sure that's what I did, unless I missed something?
```

---
## \#4 Posted by: ZackoryCramer Posted at: 2018-04-06T04:10:34.145Z Reads: 112

```
Show us your connections irl or on diagram. I had a situation similar to that of your's but that's when I used 13s. Not sure how much difference it would make depending on your setup but voltage could definitely be a factor.
Could you have gotten the polarity wrong? :thinking:
```

---
## \#5 Posted by: bsancken Posted at: 2018-04-06T04:12:50.512Z Reads: 107

```
Just to make it clear you are NOT connecting + and -. You are taking for example the red/+ line between the battery and the vesc and breaking that with an XT90 Antispark connector.
```

---
## \#6 Posted by: da_Qunster Posted at: 2018-04-06T04:21:43.698Z Reads: 105

```
That is what I did ;(
```

---
## \#7 Posted by: da_Qunster Posted at: 2018-04-06T04:26:16.564Z Reads: 104

```
I'm running on two 4S in series so basically in 8S, so not as much voltage as you're running lol. I'll have pictures up in a moment so I could show you what I did.![diagramesk8|690x312](upload://zimCljJ8OMHKFy37Niax7SMQ7VC.png)

Edit: Not the best Diagram in the world but I hope that's understandable
```

---
## \#8 Posted by: Jumpman Posted at: 2018-04-06T09:20:01.641Z Reads: 92

```
It looks from the diagram that you connected the battery negative to the Vesc positive.
```

---
## \#9 Posted by: b264 Posted at: 2018-04-06T09:32:54.559Z Reads: 90

```
[quote="da_Qunster, post:1, topic:51374"]
there was a huge spark
[/quote]

How huge?  Show us a photo of the burn mark.  Some sparking may be normal under some circumstances, but unless I see the crater in the metal I can't say.

A photo of the wiring and adaptors and loop key would help as well
```

---
## \#10 Posted by: TarzanHBK Posted at: 2018-04-06T10:19:16.609Z Reads: 82

```
Are you using a XT90 and not a XT90s?
The first one is a normal plug, the second one has the inbuild resistor, which surpresses the spark.
```

---
## \#11 Posted by: da_Qunster Posted at: 2018-04-09T02:08:26.177Z Reads: 55

```
Oh yeah I made this in a hurry, so it wasn't really that good. But I did make sure that the positives were only connected with the positives, same with the negative wires. Sorry for the confusion.
```

---
## \#12 Posted by: da_Qunster Posted at: 2018-04-09T02:09:57.132Z Reads: 53

```
I did not know there were different variations to prevent a spark. This is probably what I need. Thank you!
```

---
## \#13 Posted by: da_Qunster Posted at: 2018-04-09T02:14:36.688Z Reads: 54

```
It was pretty huge.  Almost like a small ball of light lol. I'm not at home right now so I can't show you some pictures, but the burn marks weren't that bad. I just saw some black marks inside of the connectors. But it was enough to short out the series connector I made.
```

---
## \#14 Posted by: bsancken Posted at: 2018-04-09T18:18:09.420Z Reads: 40

```
If you dont have a specific anti-spark connector like this ( https://hobbyking.com/en_us/xt90-s-anti-spark-connector-2pairs-bag.html) then it will spark alittle every time you connect it.
```

---
