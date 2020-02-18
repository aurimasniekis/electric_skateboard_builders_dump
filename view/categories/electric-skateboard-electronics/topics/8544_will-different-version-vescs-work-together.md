# Will different version VESCs work together?

### Replies: 3 Views: 342

## \#1 Posted by: nick.schweng Posted at: 2016-08-29T02:57:42.851Z Reads: 99

```
I have a dual motor setup each controlled by a different VESC. One of them can't connect to my computer and it seems like I'm going to have to buy a new one. But the ones being sold on the enertion website are different than the ones I currently have. Will they still work if they're connected via canbus? The version I have now is a 4.12.
```

---
## \#2 Posted by: racidon Posted at: 2016-08-29T04:07:55.494Z Reads: 85

```
If you're talking about how the Caps look different they will still work together without an issue I would assume mate. They are still version 4.12 VESCs just a different CAP setup
```

---
## \#3 Posted by: rpn314 Posted at: 2016-08-30T15:13:16.814Z Reads: 41

```
If it turns on and functions properly, but just doesn't connect to your computer via USB, then it probably doesn't have the bootloader on it (which you can load, you just need a programmer). To get the CAN bus functioning properly in a dual setup, the only way I know is to configure the firmware, which you'd need to connect to your computer to do in BLDC tool.
```

---
