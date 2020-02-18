# Sanity check on Vesc setting after motor swap

### Replies: 3 Views: 314

## \#1 Posted by: Arzamenable Posted at: 2017-12-12T22:14:29.495Z Reads: 77

```
Howdy y’all. I’ve been busy skating and breaking boards. I’ve stayed away from the tinkering bench for awhile until now. 

I swapped a pair of 6374 190kv 3250w motors (broke a magnet) for a pair of 6374 170kv 3550W motors (from Miami boards) . 

The previous Vesc settings were perfect. I updated the hall table and the new settings appear to be good to go. 

Should I adjust the other settings to protect battery and Vesc? Or are the motors so similar that it shouldn’t matter. 

I’ve got a 12s4p pack rated at 50a. I’ll hunt down my Vesc settings if it helps.
```

---
## \#2 Posted by: Lionpuncher Posted at: 2017-12-12T22:37:57.901Z Reads: 71

```
I think if you're keeping the battery the same and just changing the motors to a different/lower kv rating, no major adjustment is needed. If you were going to a higher kv motor it would be a different story. Would want to limit your Erpm's to 60000 to protect your Vesc.
```

---
## \#3 Posted by: cwazy1 Posted at: 2017-12-12T22:39:21.080Z Reads: 67

```
should be fine.
```

---
