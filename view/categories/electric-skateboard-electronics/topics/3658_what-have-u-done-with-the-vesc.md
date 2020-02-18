# What have u done with the vesc?

### Replies: 5 Views: 1111

## \#1 Posted by: Hummie Posted at: 2016-05-22T20:56:41.544Z Reads: 106

```
I have a couple questions.  


What is the erpm of a 12x14 motor that equates to 1rpm?

Is the max voltage still 52?  After reading this on vedder's site I'm tempted to go higher 
" NOTE: I changed the voltage dividers in hardware 2015-01-22. If you have built the PCB before that, the maximum voltage can’t be more than 52V. The difference is whether the PCB has 33k or 39k resistors. 33k means that maximum 52V can be measured. The latest PCBs (with 39k resistors) can measure 60V, but you should have some margin on your supply voltage to be safe. You can of course replace all 33k resistors with 39k and measure up to 60V."

I left the braking variables as the default at 60 and am confused..am I going to blow up my batteries going downhill?

Trying to figure my motor's no-load draw the rpm button sends the motor stuttering, racing, stopping.  
 I think finding the no-load should be doable at least and the rpm button worked for me before.  I'll take the rubber off and try again today 

What cool stuff have you done with the vesc?
```

---
## \#2 Posted by: treeme Posted at: 2016-05-22T21:29:56.804Z Reads: 92

```
Not sure what you mean by a 12x14 motor, but there's [this](https://endless-sphere.com/forums/viewtopic.php?f=2&t=34092) post on endless sphere that talks about erpm. Basically, erpm = rpm * number of pole pairs.
```

---
## \#3 Posted by: laurnts Posted at: 2016-05-22T21:30:33.370Z Reads: 90

```
I thought erpm is just motor rotation per meinute (electrical run per minute)
```

---
## \#4 Posted by: treeme Posted at: 2016-05-22T21:32:40.274Z Reads: 83

```
Nope. Also, there's more research that @chaka did [here](http://www.electric-skateboard.builders/t/choosing-the-right-motor-kv-for-the-vesc/3125).
```

---
## \#5 Posted by: Hummie Posted at: 2016-05-22T21:59:19.671Z Reads: 74

```
I think erpm is the rpm times pole pairs, with 14 magnets that's 7 pairs.   So rpm times 7 for probably all of us.  
Maybe I can find my no-load current with that
```

---
