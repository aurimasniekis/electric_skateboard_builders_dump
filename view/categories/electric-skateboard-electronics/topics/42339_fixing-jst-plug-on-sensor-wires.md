# Fixing JST plug on sensor wires

### Replies: 16 Views: 891

## \#1 Posted by: surprisebirthday Posted at: 2017-12-31T00:00:09.278Z Reads: 100

```
I have a sensored Sk3 6374 style motor that has a broken JST connector.  One part of the male connector chippped off.  My first thought was that I could just pop off the connector and put a new one on, but the connector doesn’t seem like it wants me to do that.  

My next thought was to cut the wires and solder on a new set of wires with a JST connector already on it.

Am I going down the right path or is there a better way?

<img src="/uploads/db1493/original/3X/2/a/2acce7e3ca0bb80da50b780615d236cb638c830d.jpeg" width="500" height="500">
```

---
## \#2 Posted by: mmaner Posted at: 2017-12-31T00:02:29.519Z Reads: 93

```
Get a just 2.0 6pin cable and solder it to the existing wires using the same wire layout. That's all I did tone set of motors I use.  It was so they would connect to the VESC sensor ports without an adaptor, but it works for your purpose as well.
```

---
## \#3 Posted by: surprisebirthday Posted at: 2017-12-31T00:04:39.824Z Reads: 89

```
That was probably the fastest resolution ever.  Maybe that means I asked a really simple question. :wink: 

Thanks for the help.  Looking forward to sharing the build.
```

---
## \#4 Posted by: briman05 Posted at: 2017-12-31T00:24:55.877Z Reads: 84

```
Are the pins not able to be taken out of the connector by pushing down the part of the pin. Does anyone know why type of pins they use on these is it molex or something that is specifically for jst
```

---
## \#5 Posted by: GrecoMan Posted at: 2017-12-31T00:27:21.344Z Reads: 74

```
pins can be taken out by lifting up a flap on the connector. maybe try to put it back in before buying. could still work
```

---
## \#6 Posted by: briman05 Posted at: 2017-12-31T00:30:08.149Z Reads: 64

```
Reason I ask is because in my line of work I have had to change reconfigure pins and connectors because customs tried to do it themselves and wired it wrong.
```

---
## \#7 Posted by: laurnts Posted at: 2017-12-31T00:47:49.237Z Reads: 63

```
Make sure to add some hot glue after the fix so they are more robust against vibration.
```

---
## \#8 Posted by: surprisebirthday Posted at: 2017-12-31T01:47:32.658Z Reads: 62

```
The connector was already broken off on one of the pins so I won’t be able to reuse this connector.  All male connectors I could find online have wires attached already, so I’m going to see if I can remove the connector from the new wires and put it on my wires rather than cutting wires and soldering.

@briman05 I’ll see if I can push the pins out.  That’ll help me remove the connector from the new connectors I ordered. 

@laurnts thanks for the tip!
```

---
## \#9 Posted by: briman05 Posted at: 2017-12-31T01:52:58.844Z Reads: 59

```
Digikey has jst 6 pin connector. The pins should be female and the connector male. If they are molex pins they make a pin extractor that help you remove the pins
```

---
## \#10 Posted by: surprisebirthday Posted at: 2017-12-31T03:04:26.196Z Reads: 58

```
Thanks. I couldn't find the right connector on digikey, but I was probably typing in the wrong keywords.  Your prompting did give me renewed hope that I'd find something SOMEWHERE.  I found this on ebay:

https://www.ebay.com/i/171351041635?chn=ps

Since I don't need to keep the old broken connector housing, I'm just going to snap the rest off.  My hope is that I'll just be able to plug the wires with their crimped ends into the new housing.
```

---
## \#11 Posted by: briman05 Posted at: 2017-12-31T03:43:09.018Z Reads: 55

```
https://www.digikey.com/product-detail/en/jst-sales-america-inc/PHR-6/455-1162-ND/608604#

I believe this is the correct part if you need a can cable they sell the 4 pin connector as well the pins in your link look a bit like molex pins and you should be able to push down that tab that is sticking up on the back of that hoop a little and you will be able to pull it out then pop that tab back up and insert it into the new housing
```

---
## \#12 Posted by: surprisebirthday Posted at: 2017-12-31T04:31:43.887Z Reads: 52

```
Yes! That looks like what I need. I went ahead and placed an order for 10, because it seemed silly to order only 1.

If there’s anyone else who stumbles on this thread and needs to replace the JST connector from their motor, let me know and I’ll send you one.

Once I have success repairing, I’ll report back.  The proof will also be in the eventual build thread I create.
```

---
## \#13 Posted by: briman05 Posted at: 2017-12-31T04:39:56.163Z Reads: 47

```
I will actually need 2 so I might take you up on that, but I will need 2 4pos connectors 2 so I might just order them. Let me know how they work out though.
```

---
## \#14 Posted by: surprisebirthday Posted at: 2017-12-31T04:43:13.706Z Reads: 46

```
Will do, thanks for the help. Let me know if you end up wanting a couple. They’re shipping first class, so I assume they’ll here in about a week.
```

---
## \#15 Posted by: surprisebirthday Posted at: 2018-01-06T18:31:09.862Z Reads: 36

```
All fixed!  

Using a very small-nosed pair of tweezers, I lifted up the little plastic tabs holding each of the wires and pulled the wires out.  

<img src="/uploads/db1493/original/3X/8/2/82c1a1c2ad259d940008ed34732dae70bfe161de.jpeg" width="500" height="500">

I then put the wires back into a new housing using my other motor as a reference to make sure the order was correct.

<img src="/uploads/db1493/original/3X/e/5/e5de64cdc51b632b9770779a95f1a862cd0fea0e.jpeg" width="500" height="500">

Thanks for the help, @briman05 and others.  Offer still stands for folks... if you need the housing for the sensor wires, I have 9 left from Digikey.
```

---
## \#16 Posted by: briman05 Posted at: 2018-01-07T02:01:39.533Z Reads: 29

```
Glad you were about to get it to work
```

---
