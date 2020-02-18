# Different models of VESC for dual motor

### Replies: 4 Views: 135

## \#1 Posted by: weccles Posted at: 2019-09-24T04:08:22.996Z Reads: 48

```
 I am curious if anyone has ever ran a dual motor set up with a VESC 6 and a VESC4 as the slave. Does anybody know if this would work? I’m considering buying a hub motor set up but currently only have one of each model. Both work fine I just would prefer to not have to buy another VESC6 

Thanks!
```

---
## \#2 Posted by: ChrisZ Posted at: 2019-11-15T03:47:24.555Z Reads: 24

```
check michobby , it has promotion on different vesc controllers
```

---
## \#3 Posted by: flipskytech01 Posted at: 2019-11-20T03:52:36.990Z Reads: 17

```
If want to use two single VESC to build a dual, the vesc needs to have same specifications, using a can-bus wire connect two singles and use a Y type battery wire for battery. Also, when choose a motor. Please make sure the motor RPM < vesc (V4=60000; V6=150000); Motor physical RPM=battery/power voltage (V)*motor KV value*pole pairs q'ty
```

---
## \#4 Posted by: flipskytech01 Posted at: 2019-11-20T03:54:06.012Z Reads: 17

```
The vesc 6 & vesc 4 cannot be built a dual for different specifications. If you think the vesc6 is not cost-effective enough, you can use 2 single vesc4
```

---
