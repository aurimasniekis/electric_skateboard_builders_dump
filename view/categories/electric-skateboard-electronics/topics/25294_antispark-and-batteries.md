# Antispark and batteries?

### Replies: 21 Views: 1629

## \#1 Posted by: William_Trojel Posted at: 2017-06-13T17:59:22.870Z Reads: 156

```
Hi 
I'm planning on building a setup with 2 5s lipos in series these are the batteries https://hobbyking.com/en_us/turnigy-5000mah-5s-20c-lipo-pack.html, I'm also using a Maytech 190kv motor https://www.proto-boards.com/product-page/190kv-electric-skateboard-motor-6355, so what is my top speed and range with this?
And I don't quite know how the antispark system thing works, so please write a solution to the antispark. I would also appreciate a simple wiring diagram.
```

---
## \#2 Posted by: William_Trojel Posted at: 2017-06-13T17:59:59.024Z Reads: 155

```
Oh and I weigh around 52 kg and im using a VESC if it helps
```

---
## \#3 Posted by: Decdog Posted at: 2017-06-13T18:22:32.126Z Reads: 147

```
You can use this calculator to find your top speed. http://calc.esk8.it/#{"batt-type-lipo":1,"batt-cells":8,"motor-kv":192,"system-efficiency":90,"motor-pulley-teeth":16,"wheel-pulley-teeth":36,"wheel-size":90}|
```

---
## \#4 Posted by: Smorto Posted at: 2017-06-13T18:41:06.208Z Reads: 136

```
By anti spark system I assume you mean an anti spark loop key. All this is is one of [these](https://hobbyking.com/en_us/xt90-s-anti-spark-connector-2pairs-bag.html) in your circuit. All it does is interrupt (break) the circuit then you use the other piece to complete it. I use mine on the positive wire going to my esc.

A picture says a thousand words so a bunch of pictures should help.
<img src="/uploads/db1493/original/3X/a/a/aaaa3c5210cda44e62ff4e560d9de8fe5820dbb3.jpg" width="690" height="459">

<img src="/uploads/db1493/original/3X/4/d/4dcdfe6ca7df56df3e4e1efceb820cd812472bfe.jpg" width="690" height="459">

<img src="/uploads/db1493/original/3X/d/f/df73bf57d0693f02198792052b1044d1564ca4ac.jpg" width="690" height="459">

<img src="/uploads/db1493/original/3X/e/d/edee6f3472fd0e597fe23abb61743cf6d9ba5002.jpg" width="690" height="459">

<img src="/uploads/db1493/original/3X/a/f/aff1096a6932382aeb45acb9fe1858b8e64e75f5.jpg" width="690" height="459">
```

---
## \#5 Posted by: William_Trojel Posted at: 2017-06-13T18:45:32.207Z Reads: 110

```
Can i use this https://hobbyking.com/en_us/xt90-s-anti-spark-connector-2pairs-bag.html
i'm not so good at soldering.
```

---
## \#6 Posted by: Smorto Posted at: 2017-06-13T18:46:57.297Z Reads: 109

```
Yes sorry I linked the wrong thing but you still will have to solder.
```

---
## \#7 Posted by: William_Trojel Posted at: 2017-06-13T18:48:01.067Z Reads: 105

```
Okay, so i buy one of those (https://hobbyking.com/en_us/xt90-s-anti-spark-connector-2pairs-bag.html) and solder a wire in a loop?
```

---
## \#8 Posted by: Smorto Posted at: 2017-06-13T18:49:35.912Z Reads: 100

```
Yes, the female one (the one with the green design) you will solder a loop into it. The male one (the other one) you will cut your positive wire going to your esc and solder one end on one side of the connector and the other side on the other side of the connector.
```

---
## \#9 Posted by: Smorto Posted at: 2017-06-13T18:50:29.420Z Reads: 100

```
This is a simple digram for 4s batteries but it is the same thing.

https://docs.google.com/drawings/d/1OTONGWbgS9XbY82Uh9YTEgZYb8_zqEJVXfqQTjNvynY/edit
```

---
## \#10 Posted by: William_Trojel Posted at: 2017-06-13T18:54:29.322Z Reads: 91

```
Ah okay thanks, i think that i understand it now.
But the pictures you send, it looks like different antispark loops key? (just to be sure)
```

---
## \#11 Posted by: sl33py Posted at: 2017-06-13T18:56:58.588Z Reads: 88

```
I have an old "how-to" with lots of pictures and step by step.  You can make it much simpler... but they are very easy to make w/ moderate soldering skill and a few simple tools.

https://www.electric-skateboard.builders/t/how-to-anti-spark-xt-90-loop-key/204

HTH - GL!
```

---
## \#12 Posted by: Smorto Posted at: 2017-06-13T19:32:04.580Z Reads: 80

```
yes it is the same.
```

---
## \#13 Posted by: William_Trojel Posted at: 2017-06-13T19:57:49.480Z Reads: 76

```
I have been looking into this antispark https://hobbyking.com/en_us/xt90-s-anti-spark-connector-2pairs-bag.html and i think that it has an in-built antispark system, so i dont think that i have to solder anything.
```

---
## \#14 Posted by: Smorto Posted at: 2017-06-13T19:58:28.512Z Reads: 69

```
Ok that is the same thing I am talking about... you have to solder it to your system.
```

---
## \#15 Posted by: William_Trojel Posted at: 2017-06-13T20:04:30.032Z Reads: 68

```
ah okay, now i get it. Thanks
```

---
## \#16 Posted by: Namasaki Posted at: 2017-06-13T20:20:57.150Z Reads: 63

```
10s with 5000 mah= about 10-14 miles depending on several variables
```

---
## \#17 Posted by: mmaner Posted at: 2017-06-13T20:23:46.817Z Reads: 61

```
Keep in mind...the higher the C rating, the less sag, the longer the travel time.
```

---
## \#18 Posted by: Smorto Posted at: 2017-06-13T23:12:20.988Z Reads: 56

```
no problem.
```

---
## \#19 Posted by: William_Trojel Posted at: 2017-06-14T19:32:18.802Z Reads: 49

```
One extra thing when I want to turn off my board, should I just pull the antispark connector?
```

---
## \#20 Posted by: Smorto Posted at: 2017-06-14T19:32:46.697Z Reads: 47

```
Yes.

tenchar
```

---
## \#21 Posted by: William_Trojel Posted at: 2017-06-14T19:40:14.114Z Reads: 45

```
ok, thanks
```

---
