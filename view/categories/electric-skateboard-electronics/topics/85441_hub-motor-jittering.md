# Hub motor jittering

### Replies: 2 Views: 161

## \#1 Posted by: Goldenmonkey089 Posted at: 2019-02-26T04:44:44.964Z Reads: 56

```
I recently got my hands on a new Raldey skateboard (the RES2 V1) yesterday from a friend. It had been sitting in his house for a while now (he said 2 years) and I got to ride it around today. I linked the product page below if you don't want to search it up but it's a dual hub motor longboard. I rode it around my school parking lot for a while earlier today, and then when I got home I rode it around my neighborhood. One of the motors suddenly started making a grinding sound and began jittering back and forth every time I hit the accelerator. The other motor spins with little resistance, but the motor in question has a higher resistance and feels stuck. I took it home and tried to run it again to see if it would unstick but if I try to use it too much right now it begins to smoke a little. I'm thinking this happened because breaking too hard after skating at a high speed might have messed up the motor. Any help would be appreciated. Thanks.


https://youtu.be/2dU9sRjI4Mc (This is a video of the stuck motor)

http://www.raldeyskateboards.com/product.htm
```

---
## \#2 Posted by: MysticalDork Posted at: 2019-02-26T06:25:34.496Z Reads: 36

```
The two most likely causes are either (A): the ESC is damaged in some way (One of the phases blown, maybe) or (B): the motor has an internal fault of some kind. 

Depending on the construction of the board you may be able to replace the stock ESC with a vesc or pair of vescs, and depending on your skill and stubbornness you may be able to disassemble the motor, repair the short (Possibly rewind, depends how bad it is) and reassemble it.

To determine which of those problems it is, if possible, disconnect the motors and switch them around, so the left motor is plugged into the right position, and vice versa. See if the problem stays in the same motor, or switches. If it stays in the same place, the motor is bad. If it moves, the ESC is the problem.

You can also use a multimeter to check the phase resistance of each motor, and see if there's any significant difference between the working motor and the bad one.
```

---
