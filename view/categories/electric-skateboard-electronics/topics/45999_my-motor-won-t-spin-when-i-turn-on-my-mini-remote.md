# My motor won’t spin when i turn on my mini remote

### Replies: 4 Views: 424

## \#1 Posted by: Tampaesk8er Posted at: 2018-02-10T00:13:52.055Z Reads: 83

```
I was trying to setup bluetooth module with my vesc and finally gave up on it but when i turned on my blard again using my mini remote, the motor feels locked. When i squeeze the trigger on mini remote, all im getting is very small jerks in motor. I went back on to the NEW VESC TOOL and redid my whole board setup, motor setup, app remote settup, etc. I even changed to a new mini remote did the whole binding process and im still stuck.
When i shutoff the board, i can spin my motor with my hand but when i turn on remote the motor becomes locked, I cant even spin it with my hand, it feels like the brakes are on fully. Does anyone have a solution to fix this issue? Im currently on 3.34 firmware on the vesc and my vesc is a Maytech vesc.
```

---
## \#2 Posted by: pennyboard Posted at: 2018-02-10T00:20:06.863Z Reads: 78

```
 Check your ppm settings, make sure it’s not set up to brake when the remote is in “neutral” also check your minimum voltage cutoff and make sure the VESC isn’t cutting off current to the motor
```

---
## \#3 Posted by: Tampaesk8er Posted at: 2018-02-10T18:24:01.519Z Reads: 51

```
Hope this will help someone - So i resetted vesc to default settings and did a whole setup and i noticed something really odd. when i was setting up controller in ppm settings, the part when i clicked “current, no reverse with brake” and hit apply, the meters were going haywire, from red to green back and forth really really fast. so i completed the setup. so i again did the setup again from scratch and now its finally working correctly.
 Im wondering if theres a glitch in the ppm settings and an update is needed in the new vesc tool software. SMH.
```

---
## \#4 Posted by: scepterr Posted at: 2018-02-10T19:13:17.046Z Reads: 37

```
Personally, I use only @Ackmaniacs 2.54, on all vesc4s, never any issues, ever
```

---
