# How does cruise control work in principle?

### Replies: 2 Views: 351

## \#1 Posted by: threebysix Posted at: 2018-04-08T19:45:59.684Z Reads: 102

```
I know what cruise control is and I know how to set it up in the Extended BLDC tool. My question is how do I set it up in terms of the remote/receiver and the dual vesc.

My dual vesc is connected via the can bus and my receiver for my remote is connected to the master vesc. But do I need another receiver connected to the slave vesc? Because according to the extended BLDC tool setting, cruise control is enabled by “Cruise Control via Secondary Channel” (I do not know what secondary channel in this case means).

If I'm using this [remote](https://www.ebay.ca/itm/2-4GHz-Radio-Remote-Controller-Receiver-Transmitter-For-Electric-Skateboard/201983841938?hash=item2f072cd692:g:Ua8AAOSwRMtZY4CD), do I need to buy another remote to use cruise control
```

---
## \#2 Posted by: RedEagle Posted at: 2018-04-08T22:36:08.019Z Reads: 81

```
It means cruise control has its own dedicated channel to operate. Your receiver has multiple connectors. So let's say one for normal throttle and one for cruise control. 
On the remote you linked you can just turn the right knob a bit and that will act like a cruise control knob.
```

---
