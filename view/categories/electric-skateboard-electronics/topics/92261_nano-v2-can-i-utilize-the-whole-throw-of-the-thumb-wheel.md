# Nano V2: Can I utilize the whole &ldquo;throw&rdquo; of the thumb wheel?

### Replies: 6 Views: 113

## \#1 Posted by: Jaydawg56 Posted at: 2019-04-30T00:37:42.171Z Reads: 54

```
Noob question here, but am I doing something wrong?

I've noticed I am topped out with my V2 remote after about 30% throttle position and the entire top half of my thumb throw is useless.  Is it a unity setting?  A remote calibration trick? motor AMP setting?

Or is it perfectly fine and this is expected with teh V2?

Thanks gents (and ladies)!
```

---
## \#2 Posted by: mynamesmatt Posted at: 2019-04-30T00:39:59.597Z Reads: 52

```
have you adjusted the minimum and Max in the unity App?
If you're using current control, you'll find that the wheels will go top speed by about the first 30% on the bench. however once you're on it you'll feel more throw
```

---
## \#3 Posted by: Jaydawg56 Posted at: 2019-04-30T00:44:16.505Z Reads: 46

```
Other than doing the remote min/max calibration procedures I haven't messed with anything in the Unity app.  As for my experiences with the throw, that is while I'm on the board and not bench testing. 

How would I go about messing with the min/max?  Not throttle/brake all the way to the physical limits of the remote?
```

---
## \#4 Posted by: Jinra Posted at: 2019-04-30T01:14:57.041Z Reads: 36

```
This is how current control works on vescs. You don't control speed based off throttle position, you control current, or acceleration. You can use ackmaniacs custom fw for greater control at speed. 

With no load, such as in bench testing, your motors will ramp up to full stopped quickly. When you're on the board it'll take more throttle.
```

---
## \#5 Posted by: AlanZhou Posted at: 2019-04-30T02:51:52.135Z Reads: 19

```
No that’s why you have to adjust the ppm input values on the vesc, to utilize the whole throw of the remote

Every remote is different that’s why calibration during setup is needed
```

---
## \#6 Posted by: Jaydawg56 Posted at: 2019-04-30T02:54:22.854Z Reads: 19

```
So for the Unity, what values do you speak of?  Probably have to be done throught the VESC tool vs Focbox Unity UI?
```

---
