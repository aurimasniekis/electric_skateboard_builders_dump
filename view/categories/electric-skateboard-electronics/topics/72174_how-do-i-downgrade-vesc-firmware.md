# How do I downgrade vesc firmware?

### Replies: 13 Views: 1041

## \#1 Posted by: Acklavidian Posted at: 2018-10-24T11:05:08.450Z Reads: 168

```
Im trying to downgrade my focbox firmware from 3.40 to 3.39 as part of troubleshooting some problems with my setup. Does the vesc tool come with the older versions of the firmware stored somewhere? If not where do I download the old firmware versions? 

 This seems like a common question so I'm sure someone will be able to link the info I need even though I couldn't find it. Sorry if that's the case.
```

---
## \#2 Posted by: Andy87 Posted at: 2018-10-24T13:01:28.116Z Reads: 158

```
https://www.electric-skateboard.builders/t/flipsky-bluetooth-help/70536/5?u=andy87
maybe @Jmding can tell you where he found the old FW.
```

---
## \#3 Posted by: taz Posted at: 2018-10-24T13:03:42.996Z Reads: 153

```
I have vesc tool 0.94 which should include 3.38FW, let me know if you want it.
```

---
## \#4 Posted by: Jmding Posted at: 2018-10-24T14:09:29.134Z Reads: 145

```
Yes please upload that somewhere!
I used ackmaniac's fw since I couldn't find 3.39
```

---
## \#5 Posted by: Wajdi Posted at: 2018-10-24T15:38:22.640Z Reads: 136

```
You can find them in Vedder's GitHub page, https://github.com/vedderb/bldc/tree/master/build_all just click on history and browse to the version you want.
```

---
## \#6 Posted by: Acido Posted at: 2018-10-24T16:02:18.909Z Reads: 131

```
cant you just flash ackmaniacs?
```

---
## \#7 Posted by: Acklavidian Posted at: 2018-10-24T19:04:16.835Z Reads: 118

```
Seems that is just all the built firmwares for the latest version. I don't see a catalog of old versions.
```

---
## \#8 Posted by: Acklavidian Posted at: 2018-10-24T19:05:31.915Z Reads: 110

```
I don't want to lose the ability to use Bluetooth and metr.
```

---
## \#9 Posted by: wafflejock Posted at: 2018-10-24T19:12:17.361Z Reads: 106

```
Like @Wajdi mentioned can just go through the history on the github to see any version in the history of the git repository https://github.com/vedderb/bldc/commit/a20c35b33863b85bc5a11b80d30e4df3d8066cc3#diff-00a64554bd590b5d21cdd76c4998d52c

Think you can just hit view button there on the one for appropriate hardware and then hit download button on the top right of the 'file view'

For 4.10 4.11 and 4.12 HW versions would be this one:
https://github.com/vedderb/bldc/blob/a20c35b33863b85bc5a11b80d30e4df3d8066cc3/build_all/410_o_411_o_412/VESC_default.bin
```

---
## \#10 Posted by: Acido Posted at: 2018-10-24T19:17:16.723Z Reads: 98

```
ackmaniacs firmware supports bluetooth modules
i guess you have a built in one then?
```

---
## \#11 Posted by: taz Posted at: 2018-10-25T13:46:17.792Z Reads: 79

```
Sorry guys, totally forgot about it.
Here is the link
https://www.dropbox.com/s/wil4fbo5djvt042/vesc_tool_0.94.exe?dl=0
```

---
## \#12 Posted by: Acklavidian Posted at: 2018-10-25T18:11:38.693Z Reads: 72

```
Oh wow. I'm dumb. I didn't expect the commits to be organized so well. That worked perfectly. Thank you. Too bad downgrading the firmware didn't help me figure out my canbus problem.  😒
```

---
## \#13 Posted by: Acklavidian Posted at: 2018-10-25T18:14:04.431Z Reads: 70

```
With ackmainac's firmware in the past I have had problems connecting with Android and through other apps then just ackmainac's.
```

---
