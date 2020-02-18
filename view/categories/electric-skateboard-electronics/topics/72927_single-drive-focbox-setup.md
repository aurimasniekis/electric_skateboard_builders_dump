# Single drive FOCBOX setup

### Replies: 6 Views: 229

## \#1 Posted by: MrDGOrman Posted at: 2018-10-31T16:14:59.628Z Reads: 99

```
Hi everyone,

My replacement FOCBOX has arrived so I need to program it. I was just hoping I could get some advice with setting up the FOCBOX correctly.

Single drive motor (6374) using 3 lipo batteries (9 cells total). What settings should I go for? I know the VESC PROJECT tool will set most of it up for me, but what do people suggest for the max/min limits? Also, I've got a BT module aswell (Ackmaniack). How do I go about setting that up?

Cheers,
Daniel
```

---
## \#2 Posted by: Andy87 Posted at: 2018-10-31T17:50:02.813Z Reads: 89

```
Here are a lot of threads which handle that topic.
With the search function you will get all information you need.
Basically you need to know
What your motor is rated to (6374 should be about 60-100a)
What your battery is rated for discharge 
What is your focbox rated for

Let’s say your motor is rated 80a start with
Motor max 60a
If your battery is rated to 60a start with
Bat max 40a
Motor min you can set to the same value as your motor max just in minus, so -60 or -55a
Your bat min depends on your battery max charge value... idk your lipos so you need to figure out by your own. Something between -10 and -20a will probably hit that, but check your battery specs for it.

To enable your bt module you need to set your focbox in ppm and uart mode and choose the right baudrate.

During your first rides check your values.
If your motor or your focbox becomes too hot lower your values. If you don’t have enough power and still everything runs cool (40-50degree) then slowly rise up the values
```

---
## \#3 Posted by: DavidBanner Posted at: 2018-10-31T18:23:05.021Z Reads: 70

```
keep the batt max to 30a or under to be safe, up the motor amps if you need more torque
```

---
## \#4 Posted by: Andy87 Posted at: 2018-10-31T18:24:11.835Z Reads: 66

```
Why so low with a focbox?
```

---
## \#5 Posted by: DavidBanner Posted at: 2018-10-31T18:26:02.611Z Reads: 66

```
[quote="Andy87, post:4, topic:72927, full:true"]
Why so low with a focbox?
[/quote]
that advice came directly from bara @ enertion - I could go into why this is good practice but at the end of the day bara knows more about the focbox than anyone so I take his advice and stick with it
```

---
## \#6 Posted by: dareno Posted at: 2018-11-01T20:32:05.973Z Reads: 47

```
Think he might be talking about dual there man.  I run mine at 40 batt as do lots of others and they are good as gold.
```

---
