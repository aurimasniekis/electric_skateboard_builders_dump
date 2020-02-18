# How to calculate your top speed setting using VESC and ERPM settings?

### Replies: 3 Views: 2537

## \#1 Posted by: jazzcool Posted at: 2017-06-17T16:38:45.741Z Reads: 276

```
I've been searching around with no answer to be found, if there is a good summary please direct me to it.

I wish to understand how do I use ERPM to speed limit my top speed on my mountain board. I know it has to so with soft ERPM limit, gear ratio and tire diameter. Rather than just playing around with the values until I get the speed I want, is there a formula I can use? 

thanks!
```

---
## \#2 Posted by: SageTX Posted at: 2017-06-17T16:45:09.583Z Reads: 274

```
I used this calculator. You have to play around to get it, but all the info is there. Just change # of cells up and down until the speed is what you need. You can then see the rpm at which will be what you need to set for that speed. 
    
http://calc.esk8.it/#{"batt-type-lipo":1,"batt-cells":8,"motor-kv":190,"system-efficiency":95,"motor-pulley-teeth":13,"wheel-pulley-teeth":36,"wheel-size":97}|


Of course you need to set your other parameters accurately.
```

---
## \#3 Posted by: jazzcool Posted at: 2017-06-18T01:18:10.318Z Reads: 250

```
Good info. I calculated my top speed to be around 45Kph. 
It also calculated 49728 ERPM on a 7 pair pole (I am using a 14T SK3 aerodrive so this is correct). If I limit ERPM to about 25000 should I expect the speed to be halved? 


<img src="/uploads/db1493/original/3X/a/e/ae8a1755a536fbc0872a91051f55a153080fd9b3.jpg" width="690" height="346">
```

---
