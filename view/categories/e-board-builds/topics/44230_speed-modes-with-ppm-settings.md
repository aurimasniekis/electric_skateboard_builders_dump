# Speed modes with ppm settings?

### Replies: 6 Views: 450

## \#1 Posted by: Leo31016 Posted at: 2018-01-21T02:38:40.023Z Reads: 78

```
hey guys, I was wondering if there is a way to switch speed modes without the Bluetooth thing.
After some research, I can't really find anything useful except finding my nano remote has a dedicated switch for modes. I tried the switch, but there's basically no difference on the rpm(which I assume is the speed)

This is my settings and real time data of the two modes!
![image|690x385](upload://pXe8tuIlBaahRBZdK8LDBdxnTry.png)




the is the second mode 
![image|690x388](upload://l3arTDfqATZ08m4hqdXsWsCsgla.png)



my settings
![image|690x398](upload://2t18ZA4lYB0gtBpJ8ebPhU3AR95.png)



Thanks in advance.
```

---
## \#2 Posted by: Deckoz Posted at: 2018-01-21T02:41:25.099Z Reads: 71

```
Your erpm will be the same

You won't notice a difference in rpm with the switch on ppm

You'll feel the difference on the board while the motors are loaded... No load isn't gonna show you what you wanna see
```

---
## \#3 Posted by: Leo31016 Posted at: 2018-01-21T02:43:45.051Z Reads: 71

```
so does the max min pluse width matter ? because when I switch to the second mode it shows the pulse width is 86% while the first mode goes up to 100%
```

---
## \#4 Posted by: Deckoz Posted at: 2018-01-21T02:49:06.742Z Reads: 68

```
Yes that matters. You want to tune your max and min for the 100% mode.

But you won't see the difference on the bench.. essentially what happens is your throttle gets limited to 83% of the total capable throttle, and rescaled over the throw of the stick. This changes the ramp your dutycycle over the throw of the stick. But you need load(ie ride it) to see the difference. Basically this doesn't limit speed except the very top, and really just controls acceleration

If you want to limit speed you need Bluetooth and to calculate and set a max erpm for the speed you don't want to go over.
```

---
## \#5 Posted by: Leo31016 Posted at: 2018-01-21T03:03:54.683Z Reads: 58

```
Thanks @Deckoz , will do that
now I have a new problem, he motor stutters sometimes, but sometimes it just works perfectly fine.

I thinks it has something to do with my settings, but I can't seem to find the problem. 
Can anyone take a look at my settings?
![image|690x406](upload://lyvS4VfY2zLSdf8CYGWRmuxgT6g.png)
![image|690x444](upload://neBs2gFoJXHhJRjYH0vwoYPR6dO.png)


edit: I have a torque boards 260 kv motor
```

---
## \#6 Posted by: Deckoz Posted at: 2018-01-21T03:15:35.297Z Reads: 46

```
Show the motor tab

But also... Sensors or no?

Low throttle input upside down without sensors can cause "rocking" or"cogging" where the drive train bounces back because there's no load instead of tensioning. (Shouldn't happen with sensors)

Put the board on the ground and see if it rolls like you'd expect while not standing on it...
```

---
