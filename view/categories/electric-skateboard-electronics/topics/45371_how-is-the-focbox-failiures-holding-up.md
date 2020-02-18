# How is the focbox failiures holding up?

### Replies: 13 Views: 539

## \#1 Posted by: Jammeslu Posted at: 2018-02-02T18:56:45.601Z Reads: 117

```
Hi I'm waiting for my focboxes to arrive, in the meantime I have noticed alot of focbox failiures in FOC mainly in the new vesc-tool which seems to have a bug which the Ackmaniac-tool solved. But how is it now? 
Is the new firmware for vesc-tool stable or should I downgrade to bldc tool which I am used to and the community also know well.

Plan is Dual focbox in FOC with limit erpm and split ppm. Pre loaded with Ackmaniac 3.1

Feel free to discuss anything related to this and sidetrackes aswell.
```

---
## \#2 Posted by: JohnnyMeduse Posted at: 2018-02-02T19:03:17.963Z Reads: 111

```
[quote="Jammeslu, post:1, topic:45371"]
Plan is Dual focbox in FOC with limit erpm and split ppm
[/quote]

There is no ERPM limit in FOC :wink:.
```

---
## \#3 Posted by: Jammeslu Posted at: 2018-02-02T19:04:18.185Z Reads: 111

```
Soft erpm limit? there must be haha @JohnnyMeduse
```

---
## \#4 Posted by: JohnnyMeduse Posted at: 2018-02-02T19:05:17.601Z Reads: 111

```
no there not... Erpm limit is only for BLDC

EDIT:

![image|619x283](upload://j1OkKJKIIVxYdrHE6Dn1rjzmZLE.png)
```

---
## \#5 Posted by: Jammeslu Posted at: 2018-02-02T19:06:18.788Z Reads: 108

```
then I really have to rethink, anyways want to know about the rest of my questions for the sake of the community
```

---
## \#6 Posted by: DeathCookies Posted at: 2018-02-02T19:08:05.197Z Reads: 105

```
You cannot Set a erpm limit in FOC Mode at all or there is no critical erpm number which could burn the drv?
```

---
## \#7 Posted by: Hummie Posted at: 2018-02-02T19:13:30.781Z Reads: 101

```
So I should download the ackamaniac software if I'm doing foc w focbox?
```

---
## \#8 Posted by: JohnnyMeduse Posted at: 2018-02-02T19:14:41.218Z Reads: 99

```
Not Really we have been able to push it up to 130K, without blowing anything. 

here it is at 86K

https://www.instagram.com/p/BXZQA5uHlvO/?taken-by=johnnymeduse
```

---
## \#9 Posted by: Jammeslu Posted at: 2018-02-02T19:14:44.095Z Reads: 98

```
thats my question aswell since no one has made any researched topic of a bug fix
```

---
## \#10 Posted by: onepunchboard Posted at: 2018-02-02T19:30:13.515Z Reads: 90

```
u can set rpm limit with ppm
```

---
## \#11 Posted by: Jammeslu Posted at: 2018-02-02T19:30:53.903Z Reads: 91

```
yeah its called soft limit or something
```

---
## \#12 Posted by: onepunchboard Posted at: 2018-02-02T19:33:36.212Z Reads: 90

```
i found foc without erpm limit triger focbox reset. 
when it loose traction and spins motor fast short time, it turns off and on. 
because of this i changed back to bldc
```

---
## \#13 Posted by: kyletrainy Posted at: 2018-02-03T01:56:42.638Z Reads: 72

```
Is the bug on the vesc tool firmware fixed? I’ve been using it for a couple miles with no problems. Also I set my erpm limit in the motor tab to around 37,000 with 20% limit start. This limits my speed to around 20 mph.
```

---
