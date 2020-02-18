# Switching between different cell batteries

### Replies: 3 Views: 201

## \#1 Posted by: chewydinosaurs Posted at: 2017-09-24T04:50:06.072Z Reads: 45

```
Im currently running 6s2p and was going to upgrade to 8s2p for a lot more torque on my 280kv sk3. Id need to limit the erpm since thatd give me too much speed, but if I was to switch between battery packs would I need to adjust vesc settings?
```

---
## \#2 Posted by: Namasaki Posted at: 2017-09-24T05:02:54.898Z Reads: 43

```
upgrading from 6s to 12s would yield a substantial increase in torque.
upgrading from 6s to 8s is probably not gonna make much difference in torque.

You can however increase torque by increasing motor max current.
I  found that when I increased my motor max from 60a to 80a that it increased my torque noticeably.
```

---
## \#3 Posted by: Ishayc Posted at: 2017-09-24T05:34:06.697Z Reads: 35

```
Basically the Cutoff voltage.
Just monitor your battery.
```

---
