# Dual vesc6 flipsky motor detection shows wrong values after short on 3.3 rail and stm swap

### Replies: 1 Views: 102

## \#1 Posted by: Micro Posted at: 2019-08-18T00:11:00.012Z Reads: 28

```
Hi, after a short on one site of my dual vesc6 3.3v rail, i managed to swap the stmF4 and one 3.3v LDO. Chip is one of my Flight controller from my Fpv mini quad The green lights working again using stlink v2 But the motor detection gives to high values. Resistance on the bad side is, Motor R =950mohm while the other working side is 9mohm. The values for Motor L are fine. Motor flux linkage sometimes 0 mWb on bad side. Max motor current 7 A. 6374 GTx 200kv, on good site 72A Seems that the VESC doesn't see the encoder. I tested the motor from the working side same behavior. So i think motors and encoders are fine. Getting no faults. I've decreased the current start value manually in foc tab but the motor have a hard time to start spinning.(cogging) Bad DVR?

Any ideas?
![IMG-20190817-WA0006|333x500](upload://1tkATO3BHLI3M7iSAocnAsgqVbf.jpeg)
```

---
