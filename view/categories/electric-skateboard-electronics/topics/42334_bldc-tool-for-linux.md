# BLDC Tool for Linux

### Replies: 12 Views: 1290

## \#1 Posted by: b264 Posted at: 2017-12-30T22:42:43.323Z Reads: 92

```
All the places to get the BLDC Tool are either gone from the web or they are broken, including Vedder's.  Does anyone know a working place to get the BLDC Tool for Linux?
```

---
## \#2 Posted by: wafflejock Posted at: 2017-12-31T02:40:37.979Z Reads: 85

```
I compiled it can post it somewhere here for you give me a few minutes...
```

---
## \#3 Posted by: b264 Posted at: 2017-12-31T02:58:35.567Z Reads: 82

```
Now I got it to compile but figured out you have to have a discovery board to use it
```

---
## \#4 Posted by: wafflejock Posted at: 2017-12-31T02:59:20.364Z Reads: 79

```
Not sure what you mean by a discovery board? I've been using it fine here I did have to upgrade my firmware right away but just did it over USB using the new vesc_tool (just make sure you pick the right hardware/firmware).
```

---
## \#5 Posted by: b264 Posted at: 2017-12-31T02:59:51.861Z Reads: 77

```
Yeah, it wants upgraded firmware...  how did you do that over USB

I even rolled-back the BLDC Tool to the version board I have in git ... and it still wants newer firmware
```

---
## \#6 Posted by: wafflejock Posted at: 2017-12-31T03:00:52.485Z Reads: 73

```
When I started up the vesc tool basically upgrading firmware was the only option of things to do everything else was disabled.... I found instructions somewhere too will link here if I can dig them up again

Think this was the thread actually:

http://www.electric-skateboard.builders/t/vesc-faq-firmware-upgrade-guide-windows-osx/852

I didn't have to download it manually though I don't think pretty sure I just selected a firmware that was baked into the vesc_tool.
```

---
## \#7 Posted by: b264 Posted at: 2017-12-31T03:02:55.613Z Reads: 70

```
The tool just says

[quote]
The firmware on the connected VESC is too old. Please update it using a programmer.
[/quote]

That's it.  No version, no details.

Also, that error message does not appear in the source code.
```

---
## \#8 Posted by: wafflejock Posted at: 2017-12-31T03:22:16.810Z Reads: 61

```
Possible it's telling you the right thing but pretty sure my VESC had some ancient firmware on it too, stuck in dependency building hell here, have some version of qt5 that's missing some things but will let you know when I get it back up and running and have a screenshot to show what I'm seeing or what I used there.
```

---
## \#9 Posted by: b264 Posted at: 2017-12-31T03:28:40.991Z Reads: 57

```
I decided for the full nuke option and just ordered a discovery board.  If it won't work, my friend has a JTag.  It might be some custom firmware too by someone else, who knows
```

---
## \#10 Posted by: wafflejock Posted at: 2017-12-31T07:59:44.086Z Reads: 51

```
I finally got it compiled here I upgraded some code to make it work with Qt 5.10.0 cause I couldn't figure out what version it was compiled with originally.  Anyhow doing a firmware update right now... doing it over network to phone to bluetooth to VESC... just one bad decision after another haha, it's still uploading but moving at a snails pace, over USB the firmware update went fast.  I just selected firmware on the left then after connecting to my VESC hit the up-arrow to have it show the version in the bottom right, then hit the down arrow next to the progress bar, now just waiting on progress bar.

<img src="/uploads/db1493/original/3X/2/4/240a12311f7f45c28fd9ca8b8adec66ca18f15a4.png" width="690" height="389">

This upload speed brings me back to the 28.8kbps days ;)

About to pass out here but this might help too http://vesc-project.com/node/175

https://drive.google.com/file/d/15-q8dPbS0KV5W4FC6Ea0mKHNvl3CjW3e/view?usp=sharing <-- prebuilt version 0.87 of vesc_tool
```

---
## \#12 Posted by: b264 Posted at: 2017-12-31T19:04:48.834Z Reads: 44

```
`QSocketNotifier: Invalid socket specified`

is also displayed in the terminal when the error message is displayed.  It won't tell me the current firmware version or anything, this is when clicking "Connect"
```

---
## \#13 Posted by: wafflejock Posted at: 2018-01-01T05:56:22.257Z Reads: 37

```
Found that error message in the source, looks like it's just split across a couple of lines:

https://github.com/vedderb/vesc_tool/blob/edec2d046d7c07969b7a21744715a007cc0f6bf5/vescinterface.cpp#L660

regarding the socket one though not sure something framework level where it isn't able to find whatever socket it's trying to connect to.  Still not sure what you can do if it doesn't connect though aside from what you already said.
```

---
