# What to do if windows will not detect VESC

### Replies: 6 Views: 1008

## \#1 Posted by: gamma2 Posted at: 2016-03-24T02:07:14.871Z Reads: 71

```
I've tried looking through all the FAQ posts on here. I'm trying to setup my VESC using windows and the BLDC tool but I can't get the computer to connect to it when I plug in the USB.
```

---
## \#2 Posted by: EnertionSupport Posted at: 2016-03-24T03:37:53.903Z Reads: 64

```
try changing your COM port to different numbers. 

For example on a laptop we use to test VESC's the com port has to be 4, whereas on our other computer COM 3 is what works. 

You can find that particular setting on the top right of the BLDC home page.
```

---
## \#5 Posted by: gamma2 Posted at: 2016-03-24T04:19:43.111Z Reads: 58

```
This issue was solved if an admin would like to delete/lock this thread.
```

---
## \#6 Posted by: longhairedboy Posted at: 2016-03-24T12:55:26.771Z Reads: 50

```
i say we keep this thread up in case somebody else needs it. 

The last time i had this issue was when i was helping a friend out with his VESCs. Turned out the version of BLDC tool i was using was older than the firmware on the VESC,which was surprising to me since there was barely a month's age difference between them and mine, and i had to download yet another version of windows BLDC tool to get it working. 

So for some people, the solution could be to find the absolute latest version of BLDC tool. 

Which reminds me that i want to start hosting that on my site soon.
```

---
## \#7 Posted by: chaka Posted at: 2016-03-24T13:19:15.827Z Reads: 45

```
Hey Gamma,

You have one of my VESC's so you do not need to use a lab power supply. It has already been tested so you can use system voltage to run configuration and detection....unless you are using an unusual motor.
```

---
## \#8 Posted by: gamma2 Posted at: 2016-03-25T00:14:57.687Z Reads: 38

```
Just to clarify how I solved it, for some reason my desktop on Win7 only showed a COM1 and would not accept the VESC. The same BLDC Tool version on my laptop running Win10 worked flawlessly.
```

---
