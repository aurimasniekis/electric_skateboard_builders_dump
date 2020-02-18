# New maytech remote weird problems?

### Replies: 4 Views: 378

## \#1 Posted by: Danny414 Posted at: 2018-04-24T23:34:51.671Z Reads: 97

```
I have the nano-x remote and when I first got it, it was giving me some problems.. it would disconnect.. then the board just drove off by itself.. and once it switched acceleration (up) to brake.. and when I would press down it would accelerate.. weird.. so I bought a maytech remote and connected it.. I did the calibration in bldc tool and it will not accelerate when I hit up.. but if I push down it accelerates and then won’t stop

https://streamable.com/gwitv

super weird!!

any ideas?

thanks!
```

---
## \#2 Posted by: suntorytime Posted at: 2018-04-26T19:58:20.838Z Reads: 69

```
Did you configure your PPM mapping to "Current no reverse with brake"?
```

---
## \#3 Posted by: wafflejock Posted at: 2018-04-26T20:13:51.103Z Reads: 67

```
Show some screenshots of what you see with throttle at idle vs throttle at full brake vs throttle at full acceleration (three pics ideally showing the ms value for each and what you have set for top and bottom)
```

---
## \#4 Posted by: Danny414 Posted at: 2018-04-26T20:18:20.537Z Reads: 64

```
Yeah I configed everything but I noticed the max and min were significantly different so I subtracted the difference from max - the 1.5 that the remote sends out and then I added that to the min and now it’s running amazingly! Best remote I’ve tried so far! Thanks!
```

---
