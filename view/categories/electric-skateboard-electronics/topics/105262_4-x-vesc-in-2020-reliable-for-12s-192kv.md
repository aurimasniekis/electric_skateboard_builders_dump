# 4.x VESC in 2020. Reliable For 12s 192kv

### Replies: 5 Views: 233

## \#1 Posted by: OleksiiF Posted at: 2020-01-14T08:53:42.144Z Reads: 85

```
Hi everyone

Question here as old as this it could be. I've have read all topics, but i would be happy to hear some more conversation on this topic since some vesc are out of stock now.

I need to get reliable vesc. Old one fried 3rd time (drv) and i dont want to give it for repair again (its chinese with heat shrink from eBay. Bought it in UK store 2 years ago. it was not the cheapest but quality turned out to be not good). And Im looking for replacement.


I have 3.5 year old setup. and last year i made a kydex case, and since its beautiful and i spend ton of time making it and its limited in space - its going to fit only 4.x vesc. not 6.x due to dimension limitations.

So any suggestions for vesc 4.x in 2020? 

I need it to be reliable.  I run single motor 12s 192kv setup. ill set it up to 45amps. and it will be under load regularly.

what ive found from the best options so far that is available is torqueboards vesc https:///products/torque-esc-bldc-electronic-speed-controller


and vanda vesc https://vandaelectronics.myshopify.com/products/vesc-motor-controller-custom-cables-and-connectors

i would appreciate suggestions
it would be great if it can run in foc, but if not - bldc is fine. i dont like a lot of noise, but is not highest priority.
```

---
## \#2 Posted by: Natewjh07 Posted at: 2020-01-15T09:30:15.643Z Reads: 65

```
I too would like to know what is a reliable 12s esc
```

---
## \#3 Posted by: evoheyax Posted at: 2020-01-16T15:04:20.162Z Reads: 52

```
The Official VESC 6 from Trampa has been extremely reliable for me. FocBox has been reliable for me.

Honestly, it all depends on how much current you'll be pulling also. I pull 3000 watts per motor for 12000 watts total on a full acceleration and my focbox's have lasted. But they also are not being made anymore.

Avoid flipsky and get a v6 version. The v4 version has 2 shunts which is a huge weak point. It calculates the 3rd phase in software, and is prone to error and causes fets to blow up. The v6 has 3 shunts so it measures all 3 phases in hardware, which is much safer.
```

---
## \#4 Posted by: BillGordon Posted at: 2020-01-16T16:49:33.983Z Reads: 46

```
[quote="evoheyax, post:3, topic:105262"]
It calculates the 3rd phase in software, and is prone to error and causes fets to blow up. The v6 has 3 shunts so it measures all 3 phases in hardware, which is much safer.
[/quote]

Thanks for this. Never really understood this issue until now.
```

---
## \#5 Posted by: Blitz Posted at: 2020-01-16T20:10:40.207Z Reads: 40

```
TO be sure you're talking about focbox v1.6 right?
```

---
