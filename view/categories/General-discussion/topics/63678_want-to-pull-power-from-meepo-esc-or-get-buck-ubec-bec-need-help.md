# Want to pull power from Meepo ESC or get buck/ubec/bec. Need help!

### Replies: 12 Views: 521

## \#1 Posted by: tkc Posted at: 2018-08-03T04:04:37.843Z Reads: 91

```
I bought this:
https://meepoboard.com/products/meepo-electric-skateboard-without-deck-kit

I have 5v LED strips I want to power up. I tried using a USB stick but I went over some bricks and it vibrated the USB stick to a point it wouldn't turn on anymore (only took minutes lol). I rather just wire it into the ESC or inline from battery. Possible? If so, how?
```

---
## \#2 Posted by: telnoi Posted at: 2018-08-03T05:44:54.684Z Reads: 85

```
Any 5v supply from that esc is most likely going to be low amperage, thus I would not wire anything to it. You'd need to add a buck converter to your Li-Ion output.
```

---
## \#3 Posted by: tkc Posted at: 2018-08-03T06:19:44.443Z Reads: 79

```
Yeah I was thinking that. So based on the kit and battery I purchased, what kind of buck would I need to get? Confused as to the specs I’d need to be within range of.
```

---
## \#4 Posted by: telnoi Posted at: 2018-08-03T06:22:34.425Z Reads: 76

```
Depends on the voltage of your pack and the amp draw of the led strip.
```

---
## \#5 Posted by: tkc Posted at: 2018-08-03T06:36:00.000Z Reads: 74

```
I linked to the kit that I bought. It should have the specs on the battery. The lights are here:
https://www.amazon.com/dp/B075VSRKB3/ref=cm_sw_r_cp_api_QD.yBb073A6F4

I only know they’re 5v led strips.
```

---
## \#6 Posted by: telnoi Posted at: 2018-08-03T09:42:27.171Z Reads: 61

```
Yup.. They don't mention the pack voltage/for you to figure out. Get a multimeter, ask the vendor, see if it's mentioned on the label of the pack or elsewhere.

Since the led strip has a USB connection, I am Going to assume the led strip needs 500-900 mA (USB 2 vs USB 3). It's always a good practice to get something that delivers a bit more, thus I'd recommend a buck converter capable of delivering 1.5A at 5v.
```

---
## \#7 Posted by: tkc Posted at: 2018-08-03T14:35:45.884Z Reads: 54

```
This is the battery:
https://meepoboard.com/products/battery-of-meepo-v1-5

So I guess it’s 36v? So I need a 36v to 5v step down?
```

---
## \#8 Posted by: tkc Posted at: 2018-08-03T14:54:08.529Z Reads: 52

```
Would this work then?
https://www.amazon.com/dp/B00RE6QN4U/ref=cm_sw_r_cp_api_rXgzBb7D9A7D4
```

---
## \#9 Posted by: telnoi Posted at: 2018-08-03T17:06:51.086Z Reads: 47

```
Fully charger is actually 42v, but the description mentions 52 max input. Should work.
```

---
## \#10 Posted by: tkc Posted at: 2018-08-03T17:19:12.916Z Reads: 46

```
Thank you for the help! I get the device tomorrow so hopefully it's an easy fix. Was super annoyed when my USB charger died at the start of my ride because of the rattling on a brick street.
```

---
## \#11 Posted by: tkc Posted at: 2018-08-05T22:59:32.408Z Reads: 38

```
Wired it all up today and it came out great!
```

---
## \#12 Posted by: accrobrandon Posted at: 2018-08-05T23:22:44.780Z Reads: 35

```
if you decide you want something smaller lemme know...i had a big converter like that at the beginning but was huge...

https://www.amazon.com/DZS-Elec-Adjustable-Electronic-Stabilizer/dp/B06XRN7NFQ/ref=sr_1_1_sspa?ie=UTF8&qid=1533511248&sr=8-1-spons&keywords=dc+dc+buck+converter&psc=1

this could fit "craft-ily" inside the battery case and have extras since i dont need 6 =P
```

---
