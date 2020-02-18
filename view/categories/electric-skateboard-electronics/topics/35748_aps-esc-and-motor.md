# APS ESC and motor

### Replies: 3 Views: 336

## \#1 Posted by: freeman Posted at: 2017-10-17T06:30:30.732Z Reads: 40

```
Hi,

I recently bought an APS ESC 120A with sensor and a 6473 130Kv motor also sensored.
When I connect all the stuff and using a servo tester, the motor is emitting five times a double bips after 10 seconds, and nothing happens when I try to change the pulse.
Just to be sure, I'd like to know if the initialization neutral point of the ESC is 1000µs or 1500µs. I already tested both and nothing is working.

If anybody has an idea about this bip sequence, please let me know.

Thanks,
```

---
## \#2 Posted by: onepunchboard Posted at: 2017-10-17T06:46:38.161Z Reads: 36

```
its 1500.
usually esc needs to programed neutural forward and brake position before start working. 
never tries aps esc but most of esc need initial programing. and i recommend using ppm remote and receiver
```

---
## \#3 Posted by: freeman Posted at: 2017-10-17T07:28:53.792Z Reads: 34

```
Sounds correct, I also checked the code in the wiiceiver and there is an initialization function 
Level -1 is 1000µs, 1 is 2000, 0 is 1500.

    setLevel(0);
    delay(100);
    setLevel(1);
    delay(50);
    setLevel(-1);
    delay(50);
    setLevel(0);
    delay(100);
    setLevel(1);
    delay(100);
    setLevel(0);
delay(100); 

I'll try that with an arduino and see if it works.
If anybody can confirm that initialization procedure, it would be great.

Thanks,
```

---
