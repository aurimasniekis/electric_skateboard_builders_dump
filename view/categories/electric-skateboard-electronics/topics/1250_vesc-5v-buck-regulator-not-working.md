# VESC 5V buck regulator not working

### Replies: 3 Views: 1129

## \#1 Posted by: DougM Posted at: 2016-02-07T00:34:09.703Z Reads: 95

```
Hi,  I have built 4 VESC 4.10's and the first two worked great.  But the 3rd and 4th suffer the same problem - as soon as I power them up D5, the 5V TVS, makes some crackling sounds and then smokes for a while then finally gives up.

This is because the buck regulator circuit off the DRV8302 is putting out 8v.  I assume this is the unswitched output voltage - so the switching part of the switching regulator circuit is not working.  

I have replaced all components in that circuit (there's only like 5 of them) and it did not change.  I replaced the DRV8302 and it worked correctly the night before, but the next morning same problem.

Has anyone seen and been able to successfully diagnose this problem?

Thanks,

DougM
```

---
## \#2 Posted by: DougM Posted at: 2016-06-01T02:25:09.314Z Reads: 67

```
I have the same problem.

The only thing I have found that decreases the incidence of it is a really good ground pad to ground connection on the DRV chip.  I originally used that silver CPU heat sink grease thinking it was conductive, but then when I actually tested it turns out it wasn't, so I went to silver heat sink grease, but it's not much better.

Finally I just used solder paste on the center ground pad and hotplate reflowed the DRV chip. Even with that it only worked 3 times out 4.

Like you I spent a lot of time looking at the buck reg circuit, and it's a pretty simple circuit, so shouldn't be the problem.  I even spent some time swapping in different values of components (different inductor, different diode, resistor divider network with different values increasing/decreasing the current back to the chip).

Please let me know if you find the root cause.

DougM
```

---
## \#3 Posted by: chipoi84 Posted at: 2016-06-01T02:38:42.052Z Reads: 54

```
When this happened to me, it was because I accidentally shorted the u2 regulator with the ground capacitor across from it. I'm replacing the mcu, drv8302, u2 regulator, d4, and d5 buck converter to see if it will works again.
```

---
