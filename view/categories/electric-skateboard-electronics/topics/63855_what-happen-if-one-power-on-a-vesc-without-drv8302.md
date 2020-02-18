# What happen if one power on a VESC without DRV8302?

### Replies: 2 Views: 133

## \#1 Posted by: Tomer Posted at: 2018-08-04T22:51:23.673Z Reads: 58

```
I’m trying to investigate an issue I’m facing with. 
If you power on a VESC without DRV8302 installed on it, what will be the results? Will it power on? LED lights should turn?
```

---
## \#2 Posted by: ThermalM16 Posted at: 2018-08-05T03:51:30.542Z Reads: 43

```
It will not power on at all. The DRV is what creates the 3.3v rail, so without it, your MCU has no power and your VESC has no brain essentially
```

---
