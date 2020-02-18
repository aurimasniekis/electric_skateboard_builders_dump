# VESC CAN Message Structure

### Replies: 6 Views: 628

## \#1 Posted by: ZFreaky Posted at: 2019-07-09T00:14:19.448Z Reads: 99

```
Does anyone have a well detailed write-up on the VESC CAN message structure? I've tried reverse engineering the code but it's not making a whole lot of sense compared to what's broadcast. I've found out that vedder seems to be using extended message IDs, and laid a bit of J1939 thinking in that the node id is essentially the source address in the status broadcast message. The last 2 bytes appear to be the commanded duty cycle in tenths of percent. I've yet to attempt commanding or intercepting command messages yet but I'll be continuing this and if I map out the whole message structure, I'll share my findings cause CAN is a very robust communication system that more of us should be using for safety.

Bit of an update,
I've got the status broadcast message mostly solved, mostly meaning I'm not sure what increments the current is getting sent in. btw I'm using an arduino with a can bus module using the MCP_CAN library to run these tests. Also keep in mind that if your CAN bus is connected to more than 2 vescs, you need to mind the terminating resistors, probably will need to desolder them from the other vescs.

The ID is an extended ID: 0x00000900

The 9 is the message type, in this case it's the status broadcast, the zeros after the 9 are what node it's being sent from, in this case node 0, kinda like a J1939 source address. With my experiments so far, this is pretty much how you format the messages for transmitting them. In the case of transmission, the node number to the vesc you want to command, and the message type to what parameter you want to command.
The message types are as follows:
* Duty Cycle Set:             0
* Current Set:                  1
* Current Set Brake:        2
* RPM Set:                      3
* Pos(ition?) Set:             4
* 5-8 have something to do with rx buffers, haven't messed with it yet.
* and status which is 9 as I said earlier.

The status message payload is organized as follows:
* bytes 1-4 are the current RPM as a whole number, from most significant byte to least significant, respectively.
* bytes 5 and 6 are the current current, most to least, but I'm not sure what units yet.
* bytes 7 and 6 are the current dutycycle in 10ths of a percent, from most to least.

I'm still looking into making coherent commands, for some reason commanding rpm or current at 1 causes it to max out, and has a tendency to overflow repeatedly, think it's a datatype packing issue, might make a library when I figure it out.
```

---
## \#2 Posted by: walleywalker Posted at: 2019-07-15T04:44:19.261Z Reads: 72

```
Looking forward to more updates.
```

---
## \#3 Posted by: ZFreaky Posted at: 2019-07-17T00:27:39.493Z Reads: 66

```
Aight, so I've been wrestling with the current (message 1, 4 bytes, 32 bit int cast of float multiplied by 1000) control over CAN, and I finally got it to work, it was datatype flopping around. Dutycycle (message 0, 4 bytes, 0-100) and RPM (message 3, didn't analyze it thoroughly enough) commands do work, I'm gonna try seeing what the rx buffer commands do, as I want to get voltage readings.

The way I'm reporting this is indeed very disorganized, but I do have a spreadsheet that's coming together nicely.

Update: Okay so this parts getting complicated, message types 0-4 are direct command messages as I've outlined, very similar in what you would find in automotive applications, 5-8 however get a bit weird, and I've not run into this communication protocol before but I knew it was doable. Basically, instead of the messages being tied to a specific parameter, its a couple messages running a bunch of parameters, in this case the whole configuration and live data can be retrieved from specific vescs in any given CAN network, so long as they've been set with unique node IDs. 8 (CAN_PACKET_PROCESS_SHORT_BUFFER) seems to tell the vesc in the network what you want and passes along a flag in the 3rd byte to commands_process_packet to figure it out. I think vedder did this cause he already made a message processor for the serial, so why not just adapt it for the CAN? There's a boat load of commands to comb through manually, I'm probably gonna stop when I get the essentials relating to power consumption and tachometer.
```

---
## \#4 Posted by: ZFreaky Posted at: 2019-07-21T04:27:55.189Z Reads: 45

```
I think I cracked it, slightly inept coding skills kept me from seeing something obvious. Anyway, you can pretty much get any data you want from message 8, or rather the response on message 5 depending what you ask, you can completely configure a vesc via CAN. Now, something to note is I started experiencing speed issues regarding the response on message 5. You see, when message 5 sends back more than 8 bytes, it'll chop up the message into multiple message 5s, with the first byte of each signalling where in the byte order message 5 is broadcasting. The speed issue comes in when you don't have a way of pulling all messages out of the MCP2515 fast enough, it'll start overwriting messages if it goes over 2. If you're writing serial after every single message received, it introduces significant delay to the point where you'll miss those messages coming in one after another, and for the running data, it's 8 messages that need to be read pretty much as soon as they come in, and the vesc is sending them end to end. Adding an interrupt routine that has additional rx buffers to empty the MCP2515 before reporting to serial works, but they might not come in in the right order, which is fine cause byte 1 acts as your index. Asking for the config status is a few orders of magnitude more data that is outside the scope of what I want to investigate, and will likely need an mcu with integrated CAN drivers to handle properly. I'll clean up my spreadsheet and come up with something neat, in the meantime, here's a sneak peak.[removed cause it was wrong]
 hope ya'll enjoy reading so far, I've learned a good chunk. It'll take a while for the clean spread sheet and a possible arduino library, if you don't wanna wait, the source code's been extremely helpful in figuring it out, probably difficult to read for newbies, but hey, strike while the iron's hot. Notepad++ is your friend.
```

---
## \#5 Posted by: ZFreaky Posted at: 2019-07-28T16:11:50.500Z Reads: 24

```
Aight, so I'm releasing the basic messages here, I'm not sure when I'll get around to a library as CAN bus is something you want to be directly controlling. I think effort is better spent on a tutorial for CAN bus specifically for esk8. Plus I've got other things that are taking priority atm. There's other messages that I've not tested yet, you can do all the app configuration through CAN, that's how the BLDC tool does it with CAN forwarding. Happy hacking!![image|690x262](upload://pNFvgcpc5P3iwXcke5mBeNMCZb8.png)
```

---
## \#6 Posted by: Miaopasi Posted at: 2019-09-24T04:45:17.952Z Reads: 17

```
Thanks a lot for your instructions!! I can control my VESC through CAN now.
```

---
