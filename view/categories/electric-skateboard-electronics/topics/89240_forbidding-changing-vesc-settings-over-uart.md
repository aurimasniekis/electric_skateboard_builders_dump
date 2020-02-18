# Forbidding changing VESC settings over UART

### Replies: 9 Views: 250

## \#1 Posted by: janpom Posted at: 2019-04-03T15:02:40.779Z Reads: 96

```
I recently purchased the Unity, which has BT module built-in. While that's certainly a nice and useful feature, there's a big security hole. The problem is that there's no BT pairing or any other security mechanism implemented. What that means is that anyone with a BT enabled mobile phone (= any mobile phone today) can connect to your Unity. That wouldn't be a big deal if that merely allowed them to read the telemetry. The problem is that they can change any settings as well.

This allows doing pretty nasty things. Imagine someone remapping your PPM settings and causing that you go full throttle when you merely want to slowly accelerate. While I can't see why anyone would do that intentionally (except maybe a very bad prank), I can imagine something similar happening accidentally on group rides when one person tries to change their riding profile and changes somebody else's instead.

The problem is of course not isolated to the Unity. Many people use generic BT modules connected to the VESC via UART, which is basically the same setup as Unity that has the same vulnerabilities.

I personally do like the convenience of being able to read the VESC telemetry over BT/UART. However, I don't really need to be able change my VESC settings in that way. **I actually don't even want that to be possible.**

The simplest solution I can think of is to create a custom VESC FW that ignores any potentially harmful commands received over UART, namely all write commands. I have never done any VESC FW hacking before, but looking at the code it seems this could be a very small change. I believe adding a condition [here](https://github.com/vedderb/bldc/blob/master/applications/app_uartcomm.c#L67) would do the job.

I'm considering something like:

```
if (data[0] == COMM_GET_VALUES)
    commands_process_packet(data, len, app_uartcomm_send_packet);
```

This should only process the `COMM_GET_VALUES` command, which is the request for the telemetry data and silently ignore any other received commands.

Of course other safe commands can be whitelisted the same way. This is just a example, but you get the idea.

Now, could anyone with some VESC FW hacking experience confirm this would work without breaking other critical functionality?
```

---
## \#2 Posted by: wafflejock Posted at: 2019-04-03T15:31:53.387Z Reads: 87

```
It looks like the right place to me after bouncing around some of the source but can't say I've actually had any hands on with tweaking things just building/uploading new firmware.

---

Side note the metr module does require pairing in the app which I guess is some level of security (someone would need to see the label on the bluetooth module for the pin).  I do like being able to set different modes on the fly for letting someone who has no experience try it out for a second.
```

---
## \#3 Posted by: Pimousse Posted at: 2019-04-03T15:39:10.495Z Reads: 86

```
Where do you want to apply this kind of "firewall" ?
I mean in which file of the FW ?

Touching only at commands.c will result in having VESC Tool being unable to change any parameter.
```

---
## \#4 Posted by: rpasichnyk Posted at: 2019-04-03T15:48:47.507Z Reads: 77

```
This hack will most likely work!
```

---
## \#5 Posted by: janpom Posted at: 2019-04-03T15:56:29.149Z Reads: 73

```
I know that Metr does have the pairing and IMO that's the only solution one should use if they want the VESC settings changed over BT. Doing the same with other BT modules is playing with fire. It may be convenient, but so is riding without a helmet.
```

---
## \#6 Posted by: janpom Posted at: 2019-04-03T15:57:39.648Z Reads: 75

```
[quote="Pimousse, post:3, topic:89240"]
Where do you want to apply this kind of “firewall” ? I mean in which file of the FW ?
[/quote]

[here](https://github.com/vedderb/bldc/blob/master/applications/app_uartcomm.c#L67) (the original post had the link)

[quote="Pimousse, post:3, topic:89240"]
Touching only at commands.c will result in having VESC Tool being unable to change any parameter.
[/quote]

Right. Of course not there.
```

---
## \#7 Posted by: wafflejock Posted at: 2019-04-03T16:41:34.727Z Reads: 65

```
I think it would take someone intentionally (seems unlikely, think helmet is more important but agree good to secure things and not have open connection that can change settings on the board is more ideal) doing this but if you go to meetups/group rides then likelihood of it happening accidentally definitely exists without pins.
```

---
## \#8 Posted by: Battosaii Posted at: 2019-04-03T17:15:48.254Z Reads: 57

```
I have 2 Unities one one build, and others in my group with unities so it can get a bit confusing. @Deodand says they are working to revamp the Bluetooth security and being able to configure it and change names.
```

---
## \#9 Posted by: Deodand Posted at: 2019-04-04T02:25:41.783Z Reads: 44

```
Yeah we have some incoming updates but are working on an easy to use infrastructure for over-the-air updates to BLE firmware, firmware side on the modules it's configured but need to add the feature to the phone app side (alongside release of iOS app as well) doing it through the unity firmware is a bit of a workaround that has some security holes anyway but I guess it could be used as a stop gap, but I'd rather just spend my time doing it properly. 

Proper naming and pin pairing is happening, sorry for the delay guys.
```

---
