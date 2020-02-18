# VESC/CANBUS/Y? Motor Mixture

### Replies: 2 Views: 109

## \#1 Posted by: SlimSh8y Posted at: 2018-10-04T06:37:25.781Z Reads: 32

```
When using CANBUS to connect two VESC for dual motor setup, can I use a combination of one Brushless and one Brushed Motor? Can the Slave VESC control a different type Motor than the Master? Can the Master VESC keep two different Motor types in sync?
Would this setup instead be possible with a VESC "Y" connection?
If not, is there any way to add to it or tweak it so that it will?
Any help is greatly appreciated.
```

---
## \#3 Posted by: dareno Posted at: 2018-10-04T06:54:22.005Z Reads: 26

```
No No No.  vesc is a brushless motor controller.  Do not connect a brushed motor to it.  Bldc stands for brushless dc motor  Emphasis on the brushless.
```

---
