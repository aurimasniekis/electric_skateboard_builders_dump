# 6374 Winding Pattern

### Replies: 3 Views: 349

## \#1 Posted by: clayskaight Posted at: 2017-10-13T02:16:42.351Z Reads: 72

```
Hey everyone, I am looking to fabricate my own 3D printed motor just for fun and I want to base my design off of the 6374 motor as it has a ton of power output and is very efficient. Looking at pictures I have come to the conclusion that it has 14 fixed magnets and 12 stator poles but I cannot figure out how that combination would work electronically.

 http://www.bavaria-direct.co.za/scheme/calculator/ 
Using this calculator it gives two weird answers depending on how many layers you choose.

Does anyone know how they are wound? Is there a more efficient way of winding?

Thanks!
Clayton
```

---
## \#2 Posted by: MysticalDork Posted at: 2017-10-13T02:25:09.391Z Reads: 67

```
2 layer D termination is correct. That's the most efficient way. Since the poles and stators are different, that means only one pair of stators lines up at any given time, and that coincides more or less with the phase that's on at that point. I can't be bothered to give a whole lecture on motor theory here, but if you're interested there are some good articles online.
```

---
## \#3 Posted by: MysticalDork Posted at: 2017-10-13T06:26:20.827Z Reads: 46

```
Bear in mind that the steel bell and stators are important for magnetic field conduction, and a 3d printed motor (even with magnetic filament) won't be as effective. Should work though.
```

---
