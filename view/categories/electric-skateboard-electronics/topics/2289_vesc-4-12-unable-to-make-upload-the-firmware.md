# VESC 4.12 unable to &ldquo;make upload&rdquo; the firmware

### Replies: 3 Views: 1555

## \#1 Posted by: malik Posted at: 2016-04-11T18:15:26.527Z Reads: 76

```
Hello,

I just received a VESC 4.12, and i bought a discovery board to upload the firmware. 
So I have been advised to change a specific line in the Makefile of the firmware in order to have the Discoveryboard working, which I did:

"openocd -f board/stm32f4discovery.cfg -c "reset_config trst_only combined" -c "program build/$(PROJECT).elf verify reset exit" # For openocd 0.9"
By the way, in vedders' configuration guide, the OpenOCD that the command installs is a 0.7.0 version.

So after I change that line, the error i get when uploading looks like this:
"Info : The selected transport took over low-level target control. The results might differ compared to plain JTAG/SWD
adapter speed: 2000 kHz
adapter_nsrst_delay: 100
none separate
srst_only separate srst_nogate srst_open_drain connect_deassert_srst
trst_only combined trst_push_pull
Info : Unable to match requested speed 2000 kHz, using 1800 kHz
Info : Unable to match requested speed 2000 kHz, using 1800 kHz
Info : clock speed 1800 kHz
Error: open failed
in procedure 'program' 
in procedure 'init' called at file "embedded:startup.tcl", line 473
in procedure 'ocd_bouncer'
** OpenOCD init failed **
shutdown command invoked
make: *** [upload] Error 1
"
Sometimes I do not have that ocd_bouncer error though but the log I always get is:
"srst_only separate srst_nogate srst_open_drain connect_deassert_srst
trst_only combined trst_push_pull"


Can anyone please help? 
thank you !
```

---
## \#2 Posted by: Sharkface Posted at: 2016-04-13T01:00:39.356Z Reads: 55

```
I am certain somebody will end up asking you this, so ill just get it out of the way:

This board doesnt already have firmware on it correct? I know the VESC I had bought from @onloop already had firmware on it, so I could upload via USB and get around using the whole discovery board thing. 

otherwise, the line that you changed, was it line 473 of startup.tcl?
Never done this before, but I have been programming enough to read an error output, and that error output complaigns about line 473, so whatever the solution is here has something to do with that line of the file startup.tcl. 

Will follow this as I am curious. Good luck buddy!
```

---
## \#3 Posted by: malik Posted at: 2016-04-13T16:30:40.689Z Reads: 44

```
Alright I will have a look at it and keep you up to date. It might also be an error caused by the Discovery board I have. I am still investigating all potential causes. 
I ll work on it tonight and see how it goes.
Thank you !
```

---
