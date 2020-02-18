# Low Current BMS Utilised For High Current Discharge

### Replies: 4 Views: 355

## \#1 Posted by: darkkevind Posted at: 2018-03-06T23:43:10.318Z Reads: 74

```
I've worked out a little setup to utilise a cheap tiny BMS with an on/off switch, that normally come with a really low current discharge rate - like the little ones that I use which are 16A cont. - for a high current discharge setup but have the voltage cutoff protection of the BMS still work...

When you turn the BMS on current passes from B- out through P- (Right, we all knew that though).
But then that energises the coil of the relay to allow current to pass through the main relay switch (which is high current), straight from the battery, bypassing the BMS altogether allowing the full current ability of the battery to be used.

However, when the battery gets too low for the cutoff voltages of the BMS, it'll turn off the current output from the BMS right? Well then that will stop energising the relay, therefore, the relay will switch off too... Thus protecting the battery from over-discharge...

Thoughts?

![20180306_233043|500x375](upload://yENvEqhIVJbnodKksecppgErO4j.jpg)
```

---
## \#2 Posted by: b264 Posted at: 2018-03-06T23:44:31.353Z Reads: 66

```
Instead of a relay, how about a regular electronic switch using FETs?
```

---
## \#3 Posted by: darkkevind Posted at: 2018-03-06T23:44:53.119Z Reads: 66

```
Yep, that would work too... :+1:
```

---
## \#4 Posted by: darkkevind Posted at: 2018-03-07T13:53:48.206Z Reads: 39

```
Does anyone else have any thoughts on this? Could it not be a viable stead for a large high current output BMS?
```

---
