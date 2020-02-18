# VESC configuration tips

### Replies: 3 Views: 1223

## \#1 Posted by: DaffieT Posted at: 2017-06-30T01:10:53.476Z Reads: 121

```
I recently built a board and i am configuring the vesc, recommendations for the BDLC tool configurations?
This is my setup:
190kv torque boards motor (single motor build)
4.12 VESC
on off switch speed controller
11.1v 3200 man battery (for now)
```

---
## \#2 Posted by: DaffieT Posted at: 2017-06-30T01:11:21.027Z Reads: 122

```
Current configurations:

<img src="/uploads/db1493/original/3X/e/c/ecd98d3b9bcaffe2f5e1eb5f83ef8e878adf59f0.png" width="690" height="379">
```

---
## \#3 Posted by: wafflejock Posted at: 2017-06-30T01:34:58.789Z Reads: 111

```
Have you read through this? http://www.electric-skateboard.builders/t/new-vesc-user-read-this-complete-walktrough-of-the-vesc/2980  Also have you done the BLDC detection for your motor already? 

In general you'll just want to set the Battery cutoff start and end to make sense for your battery voltage so it lets power through and then do the detection of the motor params on the BLDC page.  Once you have the motor configuration detected and entered in (read config when you first open a tab then write config when you finish making changes), then you'll go to the app configuration and adjust the control mode and input settings for what type of remote connection you're using.
```

---
