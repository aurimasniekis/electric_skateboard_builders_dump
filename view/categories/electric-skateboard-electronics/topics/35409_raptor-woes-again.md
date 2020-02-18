# Raptor Woes&hellip;.. again

### Replies: 19 Views: 841

## \#1 Posted by: Battosaii Posted at: 2017-10-13T01:04:50.044Z Reads: 213

```
So I feel like i finally got my Raptor to be reliable, i never had remote problems untill recently when i swapped out my motors but the connection problem was super intermittent. I played around with the Vesc settings and hooked up my hall sensors to my Focbox's and now it seems to be worse. my board wont respond with the lid on I have been second guessing my self because ive heard of Carbon lids on the raptors not letting signal through but my board used to work fine before.

Ill try setting them up as Sensorless again and unplugging the hall sensors to see if it makes any difference, but here is a video to demonstrate whats going on. 
https://www.youtube.com/watch?v=oKjsTkpqnhQ
```

---
## \#2 Posted by: barajabali Posted at: 2017-10-13T01:38:11.214Z Reads: 194

```
Hey man I don't think it's your programming on the vescs. What remote/receiver are you using?
```

---
## \#3 Posted by: Battosaii Posted at: 2017-10-13T01:40:37.576Z Reads: 183

```
It's a winning remote
```

---
## \#4 Posted by: GrecoMan Posted at: 2017-10-13T01:41:06.004Z Reads: 174

```
There’s your problem
```

---
## \#5 Posted by: willpark16 Posted at: 2017-10-13T01:41:38.897Z Reads: 174

```
Yea the winning remote isn't the best, gat a $30 mini from @JLabs
```

---
## \#6 Posted by: JLabs Posted at: 2017-10-13T01:44:23.215Z Reads: 168

```
Thanks for the shout @willpark16! I can have it shipped tomorrow:

https://buildkitboards.com/collections/parts/products/mini-remote
```

---
## \#7 Posted by: GrecoMan Posted at: 2017-10-13T01:46:29.694Z Reads: 161

```
Dangit @willpark16 you beat me to it!  I was just about to tag him...
```

---
## \#8 Posted by: barajabali Posted at: 2017-10-13T02:00:56.168Z Reads: 158

```
@Battosaii that should fix your problem :)
```

---
## \#9 Posted by: Battosaii Posted at: 2017-10-13T02:02:05.309Z Reads: 160

```
I'm not a huge fan of finger triggers I like Thumb scroll controls someone else suggested another model that looks like the winning a bit but its reliable
```

---
## \#10 Posted by: Michaelinvegas Posted at: 2017-10-13T02:05:44.380Z Reads: 157

```
https://www.ebay.com/i/112260629401
```

---
## \#11 Posted by: mmaner Posted at: 2017-10-13T02:16:51.358Z Reads: 147

```
You could get a steez v2 from @psychotiller.
```

---
## \#12 Posted by: michaelcpg Posted at: 2017-10-13T02:34:48.833Z Reads: 140

```
http://www.maytech.cn/en/maytech-mtskr1712-e-skateboarding-mini-wireless-remote/11032.html

These ones are pretty good as far as thumb remotes go, I believe they've got frequency hopping which is a big plus
```

---
## \#13 Posted by: baxter Posted at: 2017-10-13T08:07:27.980Z Reads: 116

```
You might also check whether the lid is glass fiber or the carbon fiber version (as with the earlier raptor models).  If it is carbon fiber, it could be blocking the radio signals between the remote and its reciever.
```

---
## \#14 Posted by: MontPierre Posted at: 2017-10-13T08:24:59.730Z Reads: 109

```
[quote="michaelcpg, post:12, topic:35409, full:true"]
http://www.maytech.cn/en/maytech-mtskr1712-e-skateboarding-mini-wireless-remote/11032.html

These ones are pretty good as far as thumb remotes go, I believe they've got frequency hopping which is a big plus
[/quote]


I have been using this remote for 3 months now and no issues so far. I think it is the best thing Maytech produced to date ;)
```

---
## \#15 Posted by: Battosaii Posted at: 2017-10-13T14:33:19.167Z Reads: 79

```
weird i switched the receiver to the other focbox and now my board is working fine.... maybe its an issue with the connector, should i try soldering the wires to the pins on the Focbox? 
Id like to make a second board with all my extra parts eventually. I just need, Trucks, pulleys and a motor mount i have everything else to make a single motor DIY build so I want to use the enertion trucks on the DIY build and buy the 218mm trucks for the Raptor. So for about $200 in parts Ill have a 10s3p single 6355 build and i could add a second motor later  should i go for it?
```

---
## \#16 Posted by: ATLesk8 Posted at: 2017-10-13T14:44:59.569Z Reads: 75

```
It could be something with the ppm connection? I had a vesc that was otherwise perfect but wouldn't connect to a remote for some reason. It would even seem to sync the remote and receiver...so weird
```

---
## \#17 Posted by: Battosaii Posted at: 2017-10-13T22:40:51.381Z Reads: 55

```
I may have found the problem I took a 10 mile ride with out a single hiccup but to be honest I'm not 100% confident. 

The connector for the receiver was connected to the left Focbox and it already almost touches the lid the problem is the left Focbox connector is pretty much in the center of the lid the most flexy part and over time the wires got damaged. Now I connected it to the right side Focbox and the connector is up on the side of the enclosed at the edge of the lid, this part should not flex at all. I hope this is the fix but I may end up buying a remote anyway.

I did order the 218mm torque boards trucks for the raptor and some extras I needed to piece together a second board with left over raptor parts lol
```

---
## \#18 Posted by: dAeM0N1K3 Posted at: 2017-10-13T22:46:42.268Z Reads: 54

```
I've got the same board and had a similar disconnect issues with Winning remote. I upgraded to the new Maytech remote and have had zero issue on disconnect since then. It seriously reaches past 25 feet in distance. Pick one up from Psychotiller for a good price. https://psychotiller.com/product/new-thumb-remotereceiver
```

---
## \#19 Posted by: Battosaii Posted at: 2017-10-13T22:48:00.657Z Reads: 52

```
Oh and I fell again... not the boards fault I've never fallen because of the board. I was doing a slow hard turn to the left and I'm regular so leaning back turning and I didn't notice a piece of wood on the floor or I did and thought it was a leaf but it made me fall lol. 
<img src="/uploads/db1493/original/3X/9/9/992ce80125bd321926ea4ad8fcd9257fae097b52.jpg" width="374" height="500">
```

---
