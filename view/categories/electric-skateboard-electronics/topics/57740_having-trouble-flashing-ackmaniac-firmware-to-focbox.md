# Having trouble flashing Ackmaniac firmware to FOCBOX

### Replies: 15 Views: 731

## \#1 Posted by: kaaaaahle Posted at: 2018-06-04T02:22:14.819Z Reads: 175

```
I am having an issue where I'm getting "motor detection failed" from ackmaniac ESC-tool during automatic motor detection/configuration. The motor will not spin even though everything appears to be connected properly.

This was after I tried flashing both firmware versions 2.54 and 3.101 to the FOCBOX. I read a thread by ackmaniac about the version 2.54.bin and when I try that one it the ESC-tool doesn't even seem to connect to the VESC.

@Ackmaniac
```

---
## \#2 Posted by: CarlCollins Posted at: 2018-06-04T03:50:06.019Z Reads: 159

```
@kaaaaahle
Kyle, From where you purchased your FOCBOX?
```

---
## \#3 Posted by: kaaaaahle Posted at: 2018-06-04T13:56:04.074Z Reads: 117

```
I purchased it from longhairedboy.com just a couple weeks ago
```

---
## \#4 Posted by: longhairedboy Posted at: 2018-06-04T14:07:59.943Z Reads: 115

```
@CarlCollins What is Enertion's policy on bricking a focbox exactly? 

And is there a way to easily restore a FocBox from "bad firmware?" If it can be done easily, it may be worth putting together some kind of "FocBox Doctor" package for it.
```

---
## \#5 Posted by: Blasto Posted at: 2018-06-04T14:23:52.188Z Reads: 107

```
think FISA (fuck it start again) is needed.

With the **ackmaniac ESC-tool**, reload the **bootloader.**
Then reload **3.101** FW.

now make a quick video of your failing motor detection, explain you battery setup.

You might just be trying to perform a motor detection while outside of your working parameters (ie battery voltage cutoffs out of bounds) or you need to tweak your detection parameters.
```

---
## \#6 Posted by: kaaaaahle Posted at: 2018-06-04T14:25:37.841Z Reads: 105

```
I don't think I bricked it. I'm still able to power it up and connect to it.

I'm gonna try again with firmware version 3.101 when I get home, I was getting confused because the "official" @Ackmaniac thread kept referring to downloading and flashing ackmaniac_2_54.bin.

That should probably be updated.
```

---
## \#7 Posted by: longhairedboy Posted at: 2018-06-04T14:26:34.325Z Reads: 102

```
let us know how it goes!
```

---
## \#8 Posted by: Maxid Posted at: 2018-06-04T14:27:18.061Z Reads: 97

```
[quote="kaaaaahle, post:6, topic:57740, full:true"]
I was getting confused because the "official" @Ackmaniac thread kept referring to downloading and flashing ackmaniac_2_54.bin.
[/quote]

That was before VESC-Tool came along.
```

---
## \#9 Posted by: CarlCollins Posted at: 2018-06-04T21:49:57.065Z Reads: 83

```
@longhairedboy

The policy is same which I told you via Personal message
```

---
## \#10 Posted by: mmaner Posted at: 2018-06-04T22:04:54.090Z Reads: 82

```
Would you mind sharing it with the rest of is?  This is info a lot of us could use.
```

---
## \#11 Posted by: kaaaaahle Posted at: 2018-06-05T00:27:15.394Z Reads: 73

```
![20180604_182528|690x388](upload://kL40goXB4G2ZIdcFZVL79AZJEXE.jpg)

Can anyone help? There are multiple selections about which firmware to upload.

@Blasto @skatardude10 @longhairedboy
```

---
## \#12 Posted by: Blasto Posted at: 2018-06-05T00:30:34.508Z Reads: 71

```
Focbox is 4_10&4_11&4_12, click that, then click default
```

---
## \#13 Posted by: kaaaaahle Posted at: 2018-06-05T00:39:13.268Z Reads: 68

```
sweet, it's working now. Thanks so much for the help. 

I had to increase the motor detection parameters w from 150 -> 400 and D 0.05 to 0.1 to get the thing to spin up properly.

Turnigy sk3 192kv. not sure about the build quality of these motors yet but we will see.
```

---
## \#14 Posted by: skatardude10 Posted at: 2018-06-05T00:39:20.152Z Reads: 66

```
This ☺️ 101010
```

---
## \#15 Posted by: skatardude10 Posted at: 2018-06-05T00:39:48.551Z Reads: 62

```
Sweet! Glad to hear you got it working dude 😎
```

---
