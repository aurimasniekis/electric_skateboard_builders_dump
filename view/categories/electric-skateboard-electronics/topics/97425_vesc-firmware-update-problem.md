# Vesc firmware update problem

### Replies: 6 Views: 397

## \#1 Posted by: Ron189 Posted at: 2019-06-28T00:28:38.959Z Reads: 73

```
Hey
I am trying to update my maytech vesc(3.56, vesc tool refuse to work with it till I update it). It tells that the supported firmware is 3.57. Can't find that firmware anywhere. Where can I find it?

Thanks in advance; Ron
```

---
## \#2 Posted by: rojitor Posted at: 2019-06-28T05:49:40.076Z Reads: 62

```
You do not need to look for files. The vesc tool will find them.

https://youtu.be/jN7rfZyzzq8
```

---
## \#3 Posted by: Ron189 Posted at: 2019-06-28T10:20:57.540Z Reads: 49

```
When I do that it like fails to update it and and the vesc stays at 3.56.. What is the problem? Maytech vesc 50a
```

---
## \#4 Posted by: Ron189 Posted at: 2019-06-28T10:25:27.866Z Reads: 50

```
that is the error I get:
Serial port error: The I/O operation has been aborted because of either a thread exit or an application request
```

---
## \#5 Posted by: rojitor Posted at: 2019-06-28T11:26:19.641Z Reads: 46

```
Did you wait at least ten seconds after firmware download? If you did and the firmware is not upgrading you have the same problem I had not so long ago. Only st-link can solve it in that case.
Do you know how to flash it?
If you do not know there's a few threads about it.

https://www.electric-skateboard.builders/t/vesc-boot-loader-installation-tutorial/32103

This is how mine looks:

![15617209036574635371425086558117|374x500](upload://pOaJH42ZxDAqUU2LcCmOOfqtZ5g.jpeg) 

![15617210257875510027945974817663|666x500](upload://ahNZcysjJSCPFVuKODF3cWNKz63.jpeg) 


![15617211004494962873504280120793|375x500](upload://kyCrXCNVErjsekugbLiCmAPYbdO.jpeg)


useful links:

https://fishpepper.de/2017/10/31/tutorial-initial-flashing-a-new-born-vesc/

http://fishpepper.de/wp-content/uploads/2017/09/VESC_FW_AND_BL_092017.zip
```

---
## \#6 Posted by: Ron189 Posted at: 2019-06-28T17:43:09.279Z Reads: 33

```
I will check this out. Thanks a lot!
```

---
