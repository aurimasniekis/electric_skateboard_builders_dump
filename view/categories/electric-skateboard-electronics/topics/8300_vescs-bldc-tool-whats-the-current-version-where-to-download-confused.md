# VESCs BLDC tool - what&rsquo;s the current version? Where to download? Confused!

### Replies: 7 Views: 2523

## \#1 Posted by: dinodave Posted at: 2016-08-25T10:11:22.889Z Reads: 285

```
I'm trying to figure out what to do with these shiny new VESCs I got from @onloop a couple of weeks ago. My board is nearly ready, so in the next few days I'll be connecting the electronics and configuring this dual Ollin 170kv motor Enertion VESC 8S setup.

But I tried to download the latest BLDC tool, and things are getting weird. Looks like the tool is mid re-locate or something? The links I followed didn't get anywhere, or got to http://vesc.net.au/download-now/ which didn't allow me to download the current version for OS X or Windows, even after the forced sign up to their mailing list next to all the misspelt donation buttons. (I'd happily pay BTW, but not forced before-hand I don't know what I'm getting, let me donate afterwards).

I did manage to find the OS X version of the tool by navigating through their file structure (always disable indexing in your webserver config). The app I got works, and I'm not sure on the version, but it only supports firmware versions 2.17 and 2.18.

So that is the next problem. The tool comes with a bunch of firmwares for different hardware, how do you know which hardware your VESC has? I see this:
<img src="/uploads/db1493/original/2X/f/fc038fb6da48a7e0c328e8c3916495a62a928f0f.png" width="270" height="368">
```

---
## \#2 Posted by: elkick Posted at: 2016-08-25T10:17:49.630Z Reads: 260

```
You'll need the one in hw_410_411_412: VESC_default.bin.

Hardware Version of your VESC is printed on the PCB and it's 4.12 currently.
```

---
## \#3 Posted by: dinodave Posted at: 2016-08-25T10:27:15.343Z Reads: 255

```
So it was, thanks :slight_smile: that's part of the problem solved

<img src="/uploads/db1493/original/2X/4/42f86e360c66554a316aa1e6445db9218a2beaae.jpeg" width="690" height="426">
```

---
## \#4 Posted by: Svenska Posted at: 2016-08-25T10:27:40.918Z Reads: 244

```
latest firmware: https://github.com/vedderb/bldc
latest BLDCTool: https://github.com/vedderb/bldc-tool

Explanation on how to compile the software:
http://vedder.se/2015/01/vesc-open-source-esc/
```

---
## \#5 Posted by: dinodave Posted at: 2016-08-26T20:26:52.172Z Reads: 208

```
Thanks, I would prefer to use OS X, and that didn't look to be an easy option from source. I'm pretty sure that the version I found is correct, however I thought I'd see if I could compile it myself from source too.

It was actually very easy, I just downloaded and installed Qt from the Qt site, then ran qmake and make and now I have an OS X BLDC tool from source. So that's definitely an option. Haven't succeeded in building the firmware yet, but that's not really necessary.
```

---
## \#6 Posted by: Blasto Posted at: 2016-08-26T20:59:13.068Z Reads: 181

```
Did you blow a fet? In the picture your middle fet seems damaged
```

---
## \#7 Posted by: dinodave Posted at: 2016-08-26T21:03:43.777Z Reads: 162

```
I noticed that too, inspected the VESC and it's just a bubble in the heat shrink :)
```

---
