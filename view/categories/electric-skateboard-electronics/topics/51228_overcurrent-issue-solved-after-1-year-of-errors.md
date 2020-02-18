# Overcurrent issue solved after 1 year of errors

### Replies: 2 Views: 253

## \#1 Posted by: Michael319 Posted at: 2018-04-04T17:09:41.667Z Reads: 91

```
I figured I'd share my findings. I had my battery Max and Min custom values. Min was set to -11 and Max was set to 20. Apparently, if your battery min is below what your battery can actually output, then you will get constant overcurrent errors every time the battery exceeds that. The vesc didn't limit the current coming from the battery pack. I set my Max and Min to 50 amps, because that's what my BMS can handle. Now I haven't gotten an overcurrent error ever and all of my problems are fixed.
```

---
## \#2 Posted by: Sebike Posted at: 2018-04-04T21:36:23.006Z Reads: 53

```
[quote="Michael319, post:1, topic:51228"]
if your battery min is below what your battery can actually output,
[/quote]

Does that make sense? Batt min is what battery will get from the vesc as regen braking current, isn't it? 

So how is that related to battery output?
```

---
