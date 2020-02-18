# New Trottinette (Electric Scooter), Advice needed

### Replies: 10 Views: 2406

## \#1 Posted by: petmakris Posted at: 2016-08-13T10:53:17.502Z Reads: 218

```
Hello guys, 
I am building and electric kick scooter using a VESC 4.12, a 149KV Turnigy Motor and a 8S or 12S LiPO battery setup.


<img src="/uploads/db1493/original/2X/e/e619deb5c0c84eaf3be93f92c0ef12fb764fabb6.JPG" width="666" height="500">

For controlling the scooter I am using two electric throttles for e-bikes (commons from ebay) and I have written a custom app using vedder's tutorial which works smoothly for the moment (I have written only the throttle, while the second control will serve for electric braking).

As I am not expert with poles and ERPM I would like to get some advice on how to configure limits for this scooter. It has a wheel with a 200mm diameter and 5:1 gearing. 

Any advices on limits, current limits and other critical information before connecting the batteries would be much much appreciated. 

For the batteries I planned to use a 12S configuration but I blew very easily my previously used vesc  so I would go for 8S at least for starters.

Of course in parallel I will try to understand on my own ERPM & limits configuration.

Thanks
```

---
## \#2 Posted by: Michaelinvegas Posted at: 2016-08-13T11:04:01.019Z Reads: 197

```
http://www.electric-skateboard.builders/t/new-vesc-user-read-this-complete-walktrough-of-the-vesc/2980?u=michaelinvegas


And ingenious way of using a styrofoam plate as a deck for the scooter....should dampen the vibrations lol
```

---
## \#3 Posted by: oneafrikan Posted at: 2016-08-13T11:04:15.585Z Reads: 185

```
There's a guy called beetbocks on the ES forum who is building these as well. Might be worth checking his builds out.
```

---
## \#4 Posted by: petmakris Posted at: 2016-08-13T11:10:24.835Z Reads: 178

```
[quote="Michaelinvegas, post:2, topic:7590"]
And ingenious way of using a styrofoam plate as a deck for the scooter....should dampen the vibrations
[/quote]

Well this is a draft, I plan to make aluminum deck but from casted aluminum, let's just not focus on the deck right now :slight_smile:
```

---
## \#5 Posted by: petmakris Posted at: 2016-08-13T16:02:15.920Z Reads: 151

```
If I have a motor with that is 149KV

but the Calculated KV: 840.96 rpm/volt

when using detection from BLDC_tool, what does this mean?

I went through a lot of the documentation but..

Is this a good back emf plot? I assume not.

<img src="/uploads/db1493/original/2X/0/073c02f014673719b427c84ff3b7ecea9d0f74e0.png" width="656" height="500">
```

---
## \#6 Posted by: barajabali Posted at: 2016-08-14T04:55:53.211Z Reads: 122

```
Coming from the guy who goes eboard parts shopping at IKEA 

:)
```

---
## \#7 Posted by: Michaelinvegas Posted at: 2016-08-14T04:58:52.800Z Reads: 126

```
Hells to the yeah

And if you look closely ... A few other have followed 😜
```

---
## \#8 Posted by: rtasca Posted at: 2016-10-20T14:30:31.368Z Reads: 91

```
did u finish this build? I am really curious to find out how the range will compare to a longboard.
```

---
## \#9 Posted by: epss4 Posted at: 2019-06-26T18:36:53.875Z Reads: 21

```
Would you mind sharing your app for the throttle?? Thanks!
```

---
## \#10 Posted by: Octave Posted at: 2019-06-26T18:42:20.062Z Reads: 19

```
Sadly the guy hasn't been on the forum in 3 years I don't think he will send the app.
```

---
