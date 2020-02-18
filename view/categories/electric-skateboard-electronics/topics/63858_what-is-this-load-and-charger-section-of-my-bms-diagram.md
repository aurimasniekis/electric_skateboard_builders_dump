# What is this load and charger section of my BMS diagram?

### Replies: 5 Views: 480

## \#1 Posted by: Taliesin Posted at: 2018-08-04T23:22:43.879Z Reads: 45

```
I’ve finally got my BMS safely wired up to my battery pack with all the balance leads and the B- pad.

I’m trying to work out the rest of my diagram, though I’ve noticed a lot of other diagrams have the same wires (ie - charge port) going to the C- pad and some are going to the P - pad. How do I know for sure which one I should use with my BMS?

1.) what exactly is the load and charger section on my BMS manual? Looks like load - going to P- pad, but I don’t know what the load is.  I’m guessing load equals the + of battery pack? Is that right?

C- is going to charger according to manual. Would that mean the charger port - wire? 

2.) is my volt meter correct in my diagram? + to battery pack and then - to C-?

—-

Then I have my anti spark switch that will go to the ESCapes which I haven’t figured out yet 

3.) if I am correct with everything that would mean my P- pad would go to the ESCapes?

Pics

![image|375x500](upload://bAhU0xZhJ0N3klMjBGmg6jYgcY.jpeg)

![image|375x500](upload://hxtKcJNp8baqHaqdfwrZn6Uqm6t.jpeg)

![image|375x500](upload://xz6r5Lk73zxIexChDsMkOsAHvhE.jpeg)
```

---
## \#2 Posted by: Moros Posted at: 2018-08-04T23:48:02.927Z Reads: 38

```
B- is for negative wire from battery
C- is for negative wire to charge port
P- is for negative wire to Esc’s

Positive wire from the charge port connects to the main battery positive wire.
The BMS looks like a bestech 12S with E-Switch so you don't need the antispark switch with that BMS.  Just wire the button to the white wires coming off the side.

With the voltmeter you can connect it to the positive wire that goes to the vesc and the negative wire coming off the vesc.

Made you a quick diagram in paint.  Pretty sure I get it all connected right, but it is 2am ..

![dirtypaintdiagram|690x438](upload://2EODM98mobi3RulKkf5Ls1Emphc.png)
```

---
## \#3 Posted by: GunnarK Posted at: 2018-08-04T23:59:00.982Z Reads: 32

```
Like @Moros said, but here in diagram form
This is about the 223 BMS

 https://www.electric-skateboard.builders/t/my-monodrive-6374-10s-bamboo-eboard/33460/31?u=gunnark

You don't need the anti spark switch since the BMS takes care of that.
```

---
## \#4 Posted by: Taliesin Posted at: 2018-08-05T00:02:35.857Z Reads: 29

```
Had no idea about the BMS taking care of the anti spark switch. That’s awesome. Thanks guys.
```

---
## \#5 Posted by: Taliesin Posted at: 2018-08-05T00:11:19.844Z Reads: 27

```
Does wiring order matter from this point on?

Like how it does for balance leads?
```

---
