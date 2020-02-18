# Do i need 2 flipsky bluetooth modules for my fsesc 6.6 dual?

### Replies: 7 Views: 302

## \#1 Posted by: Skyart15 Posted at: 2019-04-12T18:34:21.107Z Reads: 98

```
Question for all y'all. I just got my flipsky dual 6.6 fsesc and a bluetooth adapter i ordered from them. And i found something on their website that says people use 2 bluetooth adapters...does this mean i can only connect to half of my dual 6.6?
```

---
## \#2 Posted by: chrischo1996 Posted at: 2019-04-12T18:37:33.385Z Reads: 95

```
No, you only need to connect to the master VESC, the bluetooth adapter will be able to connect to both by using the canbus signal.
```

---
## \#3 Posted by: Skyart15 Posted at: 2019-04-12T18:38:08.086Z Reads: 92

```
How do i tell which one is the master vesc?
```

---
## \#4 Posted by: brenternet Posted at: 2019-04-12T18:39:15.694Z Reads: 89

```
You set the master when you set the esc up.
```

---
## \#5 Posted by: Skyart15 Posted at: 2019-04-12T18:39:55.211Z Reads: 85

```
Oh cool. Just downloaded the vesc tool. Going to tackle that tonight. Thanks for your help!
```

---
## \#6 Posted by: ervinelin Posted at: 2019-04-13T03:18:06.694Z Reads: 69

```
The flipsky bluetooth adapter is plugged into the master esc. In the app you can scan the canbus and swap to the slave esc to adjust settings.

Do note you need to have both the firmware on the vesc and the phone app to be the same version.

In the latest versions of vesctool you can even update the firmware remotely. (Takes a while)
```

---
## \#7 Posted by: Menjos Posted at: 2019-07-26T11:48:03.215Z Reads: 33

```
Flipsky "suggests" to plug-in the bluetooth module on the slave side:
https://flipsky.net/blogs/vesc-tool/having-trouble-using-flipsky-bluetooth

I wonder why and what difference does it make in practice?
```

---
