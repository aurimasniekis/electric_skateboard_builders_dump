# 10s3p 30Q battery from ownboard

### Replies: 7 Views: 256

## \#1 Posted by: joshie Posted at: 2019-03-04T13:25:15.230Z Reads: 80

```
Hey guys, I'm new to this ESK8 thing. I'm about to build my very first board. I've contacted OWNBOARD for their 10s3p 30Q pack that they will be using on their W2. 

They told me that the battery will only draws 40A. Just wondering if this battery pack going to be compatible for my build? As I'm about to run with two VESC 4.12 AND two 6355 190kv motors.

Cheers,
Josh
```

---
## \#2 Posted by: Sn4pz Posted at: 2019-03-04T13:29:25.025Z Reads: 79

```
Its not a bad starter pack, but people will warn you against the build quality of Chinese packs, as well as their shotty BMSs

That being said, if they tell you that 40a is the limit, I would respect that. Your cells can do more, but I wouldnt stress the BMS with that kind of output. Its possible to open up the back and install another BMS, making it a vastly superior battery. 

This isnt recommended unless  you know EXACTLY what youre doing, I trashed a pack like this before :upside_down_face:

Learn from our mistakes and make a great board, good luck!
```

---
## \#3 Posted by: bartroosen12 Posted at: 2019-03-04T13:35:09.966Z Reads: 74

```
If you would like a higher discharge than 40A, I should just bypass the bms and you are able to set the max battery current to 50A max (or change the bms like sn4pz said).

If not just use max 40A, because I guess the bms is the weak part in this battery.
```

---
## \#4 Posted by: Sn4pz Posted at: 2019-03-04T13:38:19.795Z Reads: 63

```
The battery should output 60a max, although you shouldnt set your vesc parameters to this, youll burn through it faster than.... I dunno something about coke and vegas

A good medium setting would be 20a on each ESC, that should provide enough oomph to get you started, and then you can decide to scale upward(less range, more power) or downwards(more range, less power)
```

---
## \#5 Posted by: joshie Posted at: 2019-03-04T13:44:00.235Z Reads: 61

```
Will I burn the battery with this setup?

* **Motor Type** : BLDC
* **Motor Max** : 80 A
* **Motor Min** : -35 A
* **Batt max** : 15 A
* **Batt min** : -12 A
* **Absolute max** : 130 A
```

---
## \#6 Posted by: Sn4pz Posted at: 2019-03-04T13:48:05.892Z Reads: 60

```
Good: Batt max, Absolute max, 'Motor Type'

Not good: Motor Max (just lower it a little, Ive ran 80a each motor on 6355s with a 4.12 Vesc before and nothing bad happened, but I struggled with cogging at high speeds and some weird temperatures)

Dont know: Batt min and motor min


Do you know how to properly program your vescs?
```

---
## \#7 Posted by: joshie Posted at: 2019-03-04T13:56:59.764Z Reads: 55

```
Not quite sure, but I've been searching through Youtube like how to set it up.
```

---
