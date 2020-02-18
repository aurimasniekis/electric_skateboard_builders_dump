# BLDC tool doesn&rsquo;t display fault codes on Window 10

### Replies: 7 Views: 696

## \#1 Posted by: BigBoyToys Posted at: 2017-01-10T07:47:23.946Z Reads: 84

```
While on the "Real Time Data" tab of the BLDC tool version 2.18 the lower part of the window where the data and fault codes are displayed is cut off. Resizing the window doesn't help. Any idea how I can fix this? Has anyone else experienced this issue? 

I'm using a Microsoft Surface book on Windows 10 pro if it matters.

<img src="/uploads/db1493/original/3X/5/5/55e66862d0ca39a527440a59d84621ced0e1a84d.PNG" width="690" height="188">
```

---
## \#2 Posted by: Stefan Posted at: 2017-01-10T08:07:52.125Z Reads: 78

```
I have the same problem on windows 10. Within a virtual machine running Linux the problem does not occur.
```

---
## \#3 Posted by: BigBoyToys Posted at: 2017-01-10T08:27:03.111Z Reads: 77

```
Thanks for confirming. I also tried running the app in compatibility mode for window 8,7 and XP. That didn't work either :(. I'd hate to have to find a different computer or install another OS just to read my fault codes. Hopefully someone on here has a simple work around.
```

---
## \#4 Posted by: IDVert3X Posted at: 2017-01-10T08:36:19.271Z Reads: 70

```
BLDC tool was designed as a GTK+ app for Linux, dont expect it to be perfect on Windows. Using it on a native OS is always better.
```

---
## \#5 Posted by: Maxid Posted at: 2017-01-10T08:43:04.266Z Reads: 68

```
fault codes can be read by typing "faults" in the BLDC Tool's terminal.
```

---
## \#6 Posted by: BigBoyToys Posted at: 2017-01-10T09:50:41.989Z Reads: 61

```
Thank you both for your replies. I was able to retrieve the fault codes via the terminal as explained.
```

---
## \#7 Posted by: palmi Posted at: 2017-03-07T07:43:08.136Z Reads: 36

```
Change the text and app size under display settings to 100% fixes the issue for me when the "Recommended" settings are above 100%. E.g.

<img src="/uploads/db1493/original/3X/e/2/e21b8bb1b9ce83835e767184189b128b3bacfdf6.PNG" width="690" height="199">
```

---
