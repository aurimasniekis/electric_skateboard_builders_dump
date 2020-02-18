# Help picking BMS amperage

### Replies: 7 Views: 2113

## \#1 Posted by: buip Posted at: 2017-12-07T03:38:26.244Z Reads: 150

```
Hi everyone, I'm planning on building a board that can handle some small hills(San Francisco) and range of 3mile or 5km(range is not too important). I've done some research but need help choosing a BMS. 

For example if my build:
 2 x 80A 190KV [motors](collections/featured-items/products/electric-skateboard-motor-6355-190kv) 
2 x  50A [VESC](collections/featured-items/products/torque-esc-vesc-bldc-electronic-speed-controller)
10S2P Li-Ion cells 3000mah 20A(const.) so it'll be 40A

I know the motors won't always be pulling so much current unless going uphill. If my battery is capable of discharging 40A, what amperage should the BMS be? If I get a 80A BMS, does that mean the max current output would still be 40A, meaning each motor's max current draw be 20A. I'd love to read your input and see what I'm misunderstanding. Thank you
```

---
## \#2 Posted by: Namasaki Posted at: 2017-12-07T03:48:50.171Z Reads: 141

```
your gonna need more battery power than that for Frisco hills.
The problem you will have is voltage sag. If your battery is 40a and you draw 20a your voltage will sag a lot.
Since your not worried about range, Lipos would be your best choice.
You could do something as simple a 2 Lipos and use a hobby charger. Then you wouldn't have to worry about bms limitations.
Or you could do something like I did with Lipos and a high output bms.
Make some popcorn and check out my build thread
http://www.electric-skateboard.builders/t/high-power-10s-lipo-battery-pack-with-bms/10014
```

---
## \#3 Posted by: buip Posted at: 2017-12-07T03:56:09.321Z Reads: 131

```
Hi Namasaki, thank you for replying. This board is mainly for commuting to work and there are not that many hills on my route and are not significantly steep. I am set on Li-ion and BMS build in order to have an easier charging method, safety, and lifespan. I don't mind learning about the BMS.
```

---
## \#4 Posted by: Namasaki Posted at: 2017-12-07T04:02:31.756Z Reads: 126

```
ok but if your thinking of using Samsung 25R's they are known for sagging.
with those you'll need at least a 10s3p or 10s4p
actually you'd be better off with Samsung 30Q's
```

---
## \#5 Posted by: willpark16 Posted at: 2017-12-07T07:23:26.494Z Reads: 112

```
For San Fran you want a 4p pack minimum
```

---
## \#6 Posted by: buip Posted at: 2017-12-07T21:09:32.121Z Reads: 96

```
The build I listed was mainly an example as my main question was picking the right specifications for the BMS.
```

---
## \#7 Posted by: michaelcpg Posted at: 2017-12-07T21:25:06.956Z Reads: 92

```
You'd be better to finalise the specs of your battery first as this will largely determine what sort of BMS you need. As others have said, I'd also recommend at least 3P but ideally 4P.

Also, just because the battery cells are rated for 20A, it's a bad idea to design around the maximum rated current of the cells. If you're drawing right up to the rated limit of the cells regularly, the cells will get hotter, sag more and give you no way near as many charge cycles so you'll end up having to replace the battery a lot sooner. 

A good rule of thumb is to design the pack to use only around half the rated current of the battery so if you're planning to regularly be drawing 40A from the pack then a 4P pack would be a good way to go.
```

---
