# Could you help me? I haveone error upgrade firmware to myVESC

### Replies: 6 Views: 204

## \#1 Posted by: Hansg Posted at: 2019-04-08T01:35:30.535Z Reads: 57

```
Hello, I hace currently one error with my VESC I am try to upgrade the firmware but I cant install the last version, attachment the video for your information, thanks a lot for your help.

I am upgrade my firmware with the last version VEST TOOL version cvesc_tool_1.08

The VESC color when it is conected is blue

https://tinytake.s3.amazonaws.com/pulse/hans-nserio/attachments/10313456/TinyTake07-04-2019-08-32-32.mp4

![49%20PM|666x500](upload://fuktRjCzbZJnDvmYFHliOWo1WX.jpeg)
```

---
## \#2 Posted by: Andy87 Posted at: 2019-04-10T06:58:30.190Z Reads: 32

```
Maybe @trampa can help you and explain why you can´t upload the newest FW.

One side note. Take care about your phase wires here:
![vesc|676x500](upload://dwfwLgdt5etuAjprtnfowabOdEz.png) 

You about to short them out like this. Please alwayse keep them isolatied from each other.
```

---
## \#3 Posted by: trampa Posted at: 2019-04-10T07:02:27.695Z Reads: 32

```
Probably bootloader missing. Third party hardware often comes without bootloader. You can re-flash the bootloader with VESC-Tool. If that doesn't work you can flash the ESC via SWD, using another VESC based ESC as a programmer. This is a new feature.
```

---
## \#4 Posted by: trampa Posted at: 2019-04-10T07:12:32.819Z Reads: 31

```
If you flash via SWD please connect  GND, IO, CLK and do not spin up the motor while ESCs are connected via SWD.
```

---
## \#5 Posted by: Hansg Posted at: 2019-04-10T13:13:32.119Z Reads: 28

```
@trampa Could you let me know how can can re-flash the bootloader with VESC-Tool? or how can I flash the ESC via SWD? thanks
```

---
## \#6 Posted by: trampa Posted at: 2019-04-11T09:59:29.823Z Reads: 25

```
Interconnect two ESC via SWD (IO, CLK; GND). Do not interconnect VCC! Use short cables (6cm)
Connect to the working ESC and go to the SWD PROG tab. You will get relevant FW listed, which you can select. Choose correct FW (e.g. 410,411,412 FW for Hw 4.12). Click Upload.
```

---
