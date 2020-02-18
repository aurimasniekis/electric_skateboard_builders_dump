# VESC firmware back end configuration

### Replies: 3 Views: 869

## \#1 Posted by: jacobbloy Posted at: 2016-03-07T08:00:59.040Z Reads: 73

```
https://youtu.be/daGGrAplBwg

This video is not for those without basic knowledge of coding.
if you can not do this your self but need to then please let me know and i can do it for you.

I go through the steps to modify the default motor and application configuration setting in the firmware and show you how to make configuration files that you can use as defaults when ever you are updating your firmware so that you can save time on configuring your vesc agin after firmware updates.

i also show you how to make modifications to the baud rate of bloc tool.

the process isn't complicated but if you get it wrong you can mess up your vesc.

i demonstrate how i have configured default setting for enertion raptor electric skateboards
```

---
## \#2 Posted by: trbt555 Posted at: 2016-03-07T17:10:08.680Z Reads: 54

```
Great stuff, thanks for posting.
However, I feel this shouldn't be necessary if BLDC tool were able to save entire settings to XML, not just only motor parameters. It could then also read defaults from XML on launch.
```

---
## \#3 Posted by: jacobbloy Posted at: 2016-03-07T21:27:02.545Z Reads: 43

```
yes that is correct, but for me once i have made the changes to the firmware i only have to do it once and then i can recompile it every update and i don't even have tooled an xml file.

but the practical nature of doing this is when you have to program over 100 vesc saves a lot of time and then you can spend that time doing spin tests to actual test the vesc.
```

---
