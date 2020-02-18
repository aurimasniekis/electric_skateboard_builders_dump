# VESC On Chip Debugging

### Replies: 1 Views: 853

## \#1 Posted by: ambrojohn Posted at: 2016-08-08T04:28:27.483Z Reads: 63

```
Hi

I have been trying to have the on-chip debugger in Eclipse 4.6 (Neon) working with no success.

I have tried to follow these two web pages, although out dated:
http://vedder.se/2012/07/get-started-wi ... ntu-linux/
http://vedder.se/2012/12/debugging-the- ... d-eclipse/ (zylincdt eclipse plugin is no longer available)

Hence,
 I am using the last openocd release (0.10) and the last 
gcc-arm-none-eabi toolchain (5.4) through the ARM GNU Eclipse plugin:
http://gnuarmeclipse.github.io/

I have tried:
- a lot of gdb commands combinations (also searching on internet) through the eclipse "Debug Configuration" window and tabs
- a lot of ticks/unticks on the eclipse "Debug Configuration" window and tabs
- gdb version 4.9 and 5.4 toolchains

Outcomes:

1
 - [ECLIPSE ONLY] When I use eclipse only, the response when I launch 
"Debug" is not always the same (sometime gdb fails to connect), I'd say 
random (inconsistency of the stlink_v2 usb dongle? It's this one: http://www.ebay.com/itm/222120784635?_t ... EBIDX%3AIT)
1.1
 - Those times that eclipse manages to connect and start writing the 
image, there is a strange timeout that make gbd terminate with exit 
value: -1

2 - [NO ECLIPSE] When I do not use eclipse, I can 
SUCCESSFULLY connect the debugger and start debugging when I launch 
openocd server and gdb client from the terminals!

3 - [HYBRID] 
When I launch openocd server from the terminal and leave eclipse run the
 gdb client, those times that eclipse manages to connect and start 
writing the image, there is a strange timeout that make gbd terminate 
with exit value: -1
3.1 - I tried to use "set remotetimeout 5" (default is 2 sec) and "set remotetimeout unlimited" with no effect.

My question is: what's the problem with eclipse?


This is the output of gdb in the best case:
/*************************************************/
stm32f4x.cpu: target state: halted
target halted due to debug-request, current mode: Handler HardFault
xPSR: 0x01000003 pc: 0xfffffffe msp: 0xffffffd8
Info : dropped 'gdb' connection
Info : accepting 'gdb' connection on tcp/3333
Error: address + size wrapped(0xfffffffe, 0x00000004)
stm32f4x.cpu: target state: halted
target halted due to debug-request, current mode: Handler HardFault
xPSR: 0x01000003 pc: 0xfffffffe msp: 0xffffffd8
cleared protection for sectors 0 through 11 on flash bank 0
auto erase enabled
Info : Padding image section 0 with 48704 bytes
/*************************************************/

This
 is the script that I am using in the "Debug Configuration" window, 
"Startup" tab, "Initialization Commands" pane (the rest I kept default, 
although I tried a lot of combinations as I said above)
/*************************************************/
target remote localhost:3333
monitor reset
monitor halt
monitor flash protect 0 0 11 off
monitor flash write_image erase "/absolute/path/to/eclipse/project/build/BLDC_4_ChibiOS.elf"
monitor reset
monitor halt
/*************************************************/
```

---
