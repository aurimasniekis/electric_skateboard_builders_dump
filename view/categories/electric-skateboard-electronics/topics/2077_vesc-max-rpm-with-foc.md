# VESC ¦ Max rpm with FOC?

### Replies: 3 Views: 1836

## \#1 Posted by: chibby Posted at: 2016-03-31T10:31:18.913Z Reads: 144

```
Is it possible to set a max rpm when using FOC mode on the VESC? 

In BLDC-tool under RPM limits it says BLDC only, but in the Nunchuck application there is something about ERPM limit start/end, what is the difference?
```

---
## \#2 Posted by: treenutter Posted at: 2016-03-31T11:31:29.882Z Reads: 141

```
@chibby Yes, if you are using FOC you can limit RPM in either controller app that you are using, PPM or Nunchuck. The ERPM is a threshold at which RPM\speed will begin to be limited by VESC, so "Start " is RPM threshold where acceleration will be controlled, and "End" is the absolute max RPM.
```

---
## \#3 Posted by: Ulfberht Posted at: 2016-04-01T21:27:18.308Z Reads: 113

```
Thanks for posting, guys!! I really wanted to know about that as well! :+1:
```

---
