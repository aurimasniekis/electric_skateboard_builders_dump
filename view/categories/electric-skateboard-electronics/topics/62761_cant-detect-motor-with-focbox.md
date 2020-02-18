# Can&rsquo;t detect motor with Focbox

### Replies: 9 Views: 276

## \#1 Posted by: Tomer Posted at: 2018-07-24T21:00:21.308Z Reads: 83

```
Hi!

I built a DIY Boostedboard clone and it worked prefect for the last couple weeks. Setup includes:
- 2x Focbox
- dual 6354 motors
- 10S4P battery with Samsung 30Q cells

The other day, on my way to work, my board started to kick me off the board when I was accelerating, and sometimes even at low speeds. It just stopped me off with full braking, motor was acting like it's twitching. 
I forgot to mention - on the very first day I built the board I accidentally caused a little short in the motor. 
I opened it and fixed it immediately before initial riding. 

So I opened the motor again as I was thinking there's a short in the motor again, and saw a little wire out of place, I opened the motor, soldered and everything is good to go.

After fixing the motor I was trying to detect the motor via BLDC tool and it's twitching so hard, not spinning at all. I receive ABS_OVER_CURRENT fault code. I tried a another working motor I have and same happen. What could cause it?
How can I tell if maybe the DRV8302 is dead and need to be replaced? 

Forgot to mention that with the other Focbox I'm able to detect the motor. 

https://www.youtube.com/watch?v=odMfhZOO_Qg

Here are my settings:
![Motor%20settings|690x294](upload://pxidhgkF6OXp15rH39r6NX1g1aO.JPG)
```

---
## \#2 Posted by: CarlCollins Posted at: 2018-07-24T22:17:23.787Z Reads: 62

```
Hi

I think you have to adjust your BLDC settings according to your setup.
This error occurs when there is settings messed up
```

---
## \#3 Posted by: Tomer Posted at: 2018-07-24T22:21:06.577Z Reads: 59

```
These are the same settings I was using for the last 2-3 weeks. What could be wrong with them? Should I lower/raise any value?
```

---
## \#4 Posted by: CarlCollins Posted at: 2018-07-24T22:21:51.067Z Reads: 58

```
I suggest you to return to the default values first and give it a try
```

---
## \#5 Posted by: Tomer Posted at: 2018-07-24T22:26:17.744Z Reads: 53

```
I did try that, didn’t solve it. Unless I missed a tab which I didn’t hit read default conf. and then write.
I’ll verify it tomorrow.
```

---
## \#6 Posted by: CarlCollins Posted at: 2018-07-24T22:38:34.999Z Reads: 47

```
I hope you will get it sorted soon
```

---
## \#7 Posted by: Hummie Posted at: 2018-07-24T22:40:34.323Z Reads: 48

```
sometimes it wont pass bldc detection but will foc.  and then ive found can run the motor even without passing either if it's still a smooth run when trying to do the tests.  sometimes the bearings are too tight or something at first.
```

---
## \#8 Posted by: onepunchboard Posted at: 2018-07-24T22:41:05.739Z Reads: 47

```
edit: when i shorted my motor wire last time i had to  send for the repair.
see if other focbox works if not u need repair
```

---
## \#9 Posted by: JohnnyMeduse Posted at: 2018-07-24T22:58:05.106Z Reads: 45

```
Watching you Video... there one phase that doesn't work, it is most likely to be a blown mosfet, or a broken gate resistor.
```

---
