# Enertion VESC Question

### Replies: 3 Views: 798

## \#1 Posted by: joeadams101 Posted at: 2016-07-30T06:01:42.842Z Reads: 63

```
Hello guys so I got my skateboard built today and I am having a problem when I give it full throttle and try to brake I see the vesc turn red. But if I am going low throttle it brakes with no problem. Does this means I have to change something in the programming of the VESC? I am using Enertion 6372 R spec motor, space cell 3 and standard vesc from Enertion. Any help will be greatly appreciated , also if there are any default that I should be running with this setup let me know. Thanks!
```

---
## \#2 Posted by: onloop Posted at: 2016-07-30T06:09:30.403Z Reads: 61

```
is this on the bench or when riding?

can you see the vesc led when riding? Sounds like you need to adjust the regen current settings.... try to make sure the regen current is not too high & also try to make sure the battery & motor regen current differential is not too wide apart. 

In other words, lower the regen current of the motor & battery and see if the problem goes away... stepping down in 1A increments is best practise.

did you do a motor detection? Also, as a precaution check your motor wires inside the 6374 and make sure they are not moving around too much, there have been a few reports of motors shorting out after a while due to the wires rubbing & wearing away the insulation.

 see here: http://www.electric-skateboard.builders/t/r-spec-shorted-phase-wire-problem-solution/6474
```

---
## \#3 Posted by: joeadams101 Posted at: 2016-07-30T06:12:03.009Z Reads: 56

```
Hey thanks for the quick reply. This was the first test i did on the bench. No settings adjusted, left everything how it came like. What will be the require setting for this set up? @onloop
```

---
