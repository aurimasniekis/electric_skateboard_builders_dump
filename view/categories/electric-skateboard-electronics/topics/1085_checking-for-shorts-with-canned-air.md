# Checking for shorts with canned air

### Replies: 4 Views: 879

## \#1 Posted by: chaka Posted at: 2016-01-23T21:43:32.229Z Reads: 67

```
I recently repaired a VESC which had been shorted through the P1 header/encoder/hall sensor port. 

The result was a dead vesc with a hot voltage regulator when powered on. I was short on time and my multi meter needed a new 9v battery so I resorted to less professional means of finding the offending short.

I took a some canned air and sprayed the vesc making sure to invert the can in order to get the VESC lightly frosted. Once powered on, you could see the short circuit emerge as the heat generated thawed the frost, eventually terminating at the stm32 processor. After replacing the processor the VESC was back in full operation.

<img src="/uploads/db1493/original/2X/3/34269bfeb3a9caad2e4497cd484cf821a06c292e.jpg" width="690" height="446">
```

---
## \#2 Posted by: lowGuido Posted at: 2016-01-23T22:00:14.044Z Reads: 61

```
ingenious!


----------
```

---
## \#3 Posted by: longhairedboy Posted at: 2016-01-23T23:28:16.831Z Reads: 57

```
very clever! I had never heard of this trick until now.
```

---
## \#4 Posted by: chaka Posted at: 2016-01-24T02:54:03.220Z Reads: 53

```
This is a quick and dirty method.

 I pulled this one from the bone yard for myself. Really surprised by how well it worked, wouldn't recommend this for everyone but it was fun to try on something I wasn't worried about ruining.
```

---
