# DC-DC Step Down Converter 6.5V-60V to 1.25-30V

### Replies: 4 Views: 143

## \#1 Posted by: gmurad Posted at: 2019-05-23T12:38:52.179Z Reads: 63

```
Found this step down converter which seems decent for e-skate application, has anyone tried it to add USB ports to an enclosure?

- https://www.aliexpress.com/i/32845852284.html
- https://www.amazon.ca/gp/product/B074C3JH87/ref=ox_sc_act_title_1?smid=A36ZH2MCHPKXUA&amp;psc=1

Found a review of it [here](https://lygte-info.dk/review/Converter%20DC-DC%2010A%206.5-60V%20to%201.25-30V%20UK.html) which is disappointing but it's probably still ok for drawing a couple of amps.
```

---
## \#2 Posted by: janpom Posted at: 2019-05-23T12:47:50.065Z Reads: 58

```
I purchased this one (https://www.aliexpress.com/item/32861200188.html), which seems to be the same. Got magic smoke the first time I connected my 10S battery to the input. That's 42V, not even close to 60V. Can't recommend it.

This one works for me though: https://www.aliexpress.com/item/32878065864.html

I use it to power ESP8266 development board with a 2.0" display connected. I step down the input voltage (35-42V) to 8V and draw around 100 mA. I haven't tried drawing more than that.
```

---
## \#3 Posted by: mmaner Posted at: 2019-05-23T12:56:11.251Z Reads: 53

```
Its probably hit & miss.  I'm using the same one in my Lacroix to power lights and it's been flawless.
```

---
## \#4 Posted by: gmurad Posted at: 2019-05-23T21:20:40.390Z Reads: 27

```
That's a 10s6p right, so 42V max. I'm looking at this for a 12S build. It's not looking like a great choice but might still try it.

There aren't many small buck converters from 12S voltage to 5V output.
```

---
