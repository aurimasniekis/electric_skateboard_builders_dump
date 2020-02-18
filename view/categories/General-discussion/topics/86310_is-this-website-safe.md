# Is this website safe?

### Replies: 5 Views: 198

## \#1 Posted by: Wulfsberg Posted at: 2019-03-06T14:57:22.599Z Reads: 118

```
So i am looking for batterie packs and i found this website: http://www.hbsluk.co.uk/AERDU-36V-10S3P-42V-75Ah-Ultra-thin-15A-BMS-High-power-capacity-18650-lithium-battery-pack-ebike-electric-bicycle-motor-scooter-p-7864.html 
Does this seem sketchy to you guys?
```

---
## \#2 Posted by: rusins Posted at: 2019-03-06T15:21:04.039Z Reads: 94

```
It says 15A, whereas a 10s3p from something like Samsung 30Q cells should safely support 60A. Either they're using cheap, low quality cells, or a cheap BMS without discharge bypass, or thin wires, or maybe all 3. + that price is too good to be true. I would advise not purchasing that.

Edit: And 75Wh is way too small for a pack of that size :smiley:
```

---
## \#3 Posted by: sk8l8r Posted at: 2019-03-06T15:25:55.475Z Reads: 82

```
You should keep your battery discussion in one thread there is no need to keep creating more!
```

---
## \#4 Posted by: Wulfsberg Posted at: 2019-03-06T15:47:05.737Z Reads: 64

```
[quote="rusins, post:2, topic:86310"]
15A, whereas a
[/quote]

Im kinda new to this, what does 15A BMS differ from a 60A?
```

---
## \#5 Posted by: rusins Posted at: 2019-03-06T16:07:16.130Z Reads: 46

```
It basically tells you what the max current you can draw from the battery is. Because people often use charge only BMSs, they will have separate wires to charge the battery from their charger, and wires to connect the battery to the ESC. This way you can balance your battery when charging, and don't need an expensive BMS that can handle enough current to run the board at the power you want it to run.

Then there are more expensive high-discharge BMSs, which will allow you to balance your pack when discharging + with regenerative breaking. For those BMSs the max discharge current matters, because you will fry the BMS if going above it.

The higher your overall discharge current, the longer you can maintain max acceleration / the steeper hills you can climb, assuming your motor and ESC can handle it as well. Most people on this forum build boards with ~60A max current. (Except for mountainboards / extremely powerfull builds) Prebuilt boards will often be a bit lower.
```

---
