# Not enough power

### Replies: 12 Views: 669

## \#1 Posted by: firenikeboy Posted at: 2017-11-13T00:58:10.367Z Reads: 98

```
Hi, I've just finished building my first Eboard. My board is able to move by itself however once I'm on it, it's barely moving or doesn't move at all. I was wondering whether my build is faulty or I have to configure my VESC. These are the parts I've used: 
motor: http://www.hobbypartz.com/96m608-bigfoot160-5335-245kv.html
Battery: 2 of https://hobbyking.com/en_us/zippy-compact-5000mah-3s-25c-lipo-pack.html
VESC http://www.enertionboards.com/electric-skateboard-parts/FOCBOX-programmable-brushless-motor-controller/
Drive Pulley (36T) & Motor Pulley (16T) & 12mm Belt: products/36t-kegel-pulley-combo-kit
```

---
## \#2 Posted by: faithfulpuppy Posted at: 2017-11-13T01:02:57.184Z Reads: 93

```
are your batteries wired in series or parallel?
```

---
## \#3 Posted by: ARetardedPillow Posted at: 2017-11-13T01:03:09.893Z Reads: 91

```
Was about to ask the same lol
```

---
## \#4 Posted by: faithfulpuppy Posted at: 2017-11-13T01:04:40.098Z Reads: 87

```
also, have you run motor detection (with the pulley off)
for your performance to be that bad you'd probably have a battery issue or a problem in your settings
even on relatively small motors, the first time you accelerate on an eboard should be pretty scary.
```

---
## \#5 Posted by: onepunchboard Posted at: 2017-11-13T01:37:55.545Z Reads: 68

```
bought wrong motor perhaps, for that ratio it's better to be lower kv
```

---
## \#6 Posted by: firenikeboy Posted at: 2017-11-13T01:39:51.034Z Reads: 66

```
The batteries are in series.
What do you mean motor detection?
```

---
## \#7 Posted by: onepunchboard Posted at: 2017-11-13T01:43:34.109Z Reads: 65

```
Oh here we go, u have to set vesc parameter/ program, for specific motor u use in order to use it
```

---
## \#8 Posted by: GrecoMan Posted at: 2017-11-13T01:44:10.880Z Reads: 60

```
lol another example of someone who jumped in blind...
```

---
## \#9 Posted by: SeanHacker Posted at: 2017-11-13T01:46:51.203Z Reads: 56

```
Configure your vesc. http://www.electric-skateboard.builders/search?q=Vesc%20faq
```

---
## \#10 Posted by: firenikeboy Posted at: 2017-11-13T01:52:19.713Z Reads: 53

```
yea thats what I was asking. Thanks
```

---
## \#11 Posted by: MysticalDork Posted at: 2017-11-13T02:25:12.437Z Reads: 45

```
Make sure you've set your cutoff voltages correctly in the vesc, if they're set too high the board will be weak and not have much range. If set too low, you risk damaging the batteries. 

For lipo batteries, 3.5 or 3.6v per cell is a good number for "cutoff end", for 18650, you can go lower like 3.0. For "cutoff start", go about 0.2-0.3v higher than cutoff end.
```

---
## \#12 Posted by: firenikeboy Posted at: 2017-11-13T02:39:50.787Z Reads: 37

```
thanks for the advice
```

---
