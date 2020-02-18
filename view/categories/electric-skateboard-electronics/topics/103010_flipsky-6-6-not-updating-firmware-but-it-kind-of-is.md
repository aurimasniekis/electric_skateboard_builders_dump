# Flipsky 6.6 not updating firmware (but it kind of is)?

### Replies: 4 Views: 150

## \#1 Posted by: Ultimiant Posted at: 2019-10-16T15:29:40.398Z Reads: 41

```
Alright so I got everything hooked up last night and got my Flipsky 6.6 Pro hooked up to VESC Tool. I tried updating the firmware and it seemed to update correctly and it upgraded from 3.53 to 3.62. But whenever I run the FOC setup and get to "run detection" for the wheels I get this error:
![unknown-2|425x115](upload://Ap9KIH6IWulwEnxYPvyk1WH7cFk.png) 

After which if I go back to the firmware page it says that I am running 3.62 which is the latest version:
![unknown-3|690x46](upload://fiJuknEtRbISqWvlQHAGIbWOTJR.png) 

If I hit check version after that it'll then say 3.53
![unknown-4|690x48](upload://nQofvVVXj9CXWa5Z8A1z9Z3wdmW.png) 

And if I dont run FOC setup qizard and I hit check vesc version it will stay at 3.62. I've tried running the bootloader but to no avail, I still get the same error when using the FOC setup wizard. Anyone know a way around this or what might be happening? I'm not getting anything in the faults screen either.
```

---
## \#2 Posted by: esk8snith Posted at: 2019-10-16T18:14:43.957Z Reads: 26

```
This has happened to me a couple of times but only while setting up input. I usually just close the dialog box and try again a couple times and it works then.
```

---
## \#3 Posted by: Ultimiant Posted at: 2019-10-16T19:12:34.487Z Reads: 24

```
Yeah I tried around 5 times but was met with the same error each time, I even tried power cycling. I'm hoping to at least be able to input the values manually tonight.
```

---
## \#4 Posted by: Movation Posted at: 2019-10-16T22:06:46.716Z Reads: 21

```
I had this isdues with my 4.2 plus the second vesc woudnt update via canbus so i had to treat them as seperate vesc even then updates took 2 or 3 goes to work via seperate usb. Updates since have been fine. Its like when you create a mismatch of firmware canbus features stopped working. With one side updated i could see the second vesc but not update it. Try removing all uart devices. Controllers and metr ect.
```

---
