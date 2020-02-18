# What does &ldquo;Over Voltage protection&rdquo; do on the FocBox

### Replies: 2 Views: 116

## \#1 Posted by: amansawhney Posted at: 2018-07-26T05:28:59.556Z Reads: 46

```
I had a TB Vesc die on me bc the heatstrink on my bullet failed and it touched and now its toast.  Would "Over Voltage protection" on the FocBox protect against that?
```

---
## \#2 Posted by: AutoItKing Posted at: 2018-07-26T06:23:09.059Z Reads: 37

```
The over voltage protection is to protect the battery, not necessarily the circuitry. It will stop regen braking when the battery voltage reaches that set point to avoid over charging (very dangerous). Shorting something will kill something no matter what software limits you set. So no, it won't protect against that.
Make sure to secure your connections to avoid that issue.
```

---
