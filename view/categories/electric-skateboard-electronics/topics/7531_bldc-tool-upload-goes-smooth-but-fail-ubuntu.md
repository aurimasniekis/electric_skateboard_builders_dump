# BLDC Tool upload goes smooth but FAIL (Ubuntu)

### Replies: 5 Views: 411

## \#1 Posted by: ambrojohn Posted at: 2016-08-12T03:07:45.695Z Reads: 44

```
I have an odd behaviour in flashing the VESC (firmware version 2.18):

When I flash from the terminal, via stlink usb dongle, with 'make upload' I can see the changes I put in the code.
But
 when I flash from the bldc tool, via usb, although the process looks 
smooth and successful (I point the right bin file, click upload, and see
 the progress bar reaching 100%), what I have is a VESC with a sort of 
default firmware on it with no changes at all.

To be precise, as the bldc tool finishes to flash the VESC, the VESC does not reboot by itself as it should.

That's most likely a sign of failed flashing but...why is that and what can I try to fix it?
```

---
## \#2 Posted by: chaka Posted at: 2016-08-12T03:12:24.605Z Reads: 40

```
You should not have tried to flash the VESC. It came preloaded with the firmware and bootloader. You may have corrupted the bootloader if you didn't connect the st-link correctly.
```

---
## \#3 Posted by: ambrojohn Posted at: 2016-08-12T03:21:20.167Z Reads: 40

```
Well...I purchased the VESC explicitly to program it with some custom code so...

The VESC it's working. I just cannot flash it from the bldc tool. Only via stlink dongle from the terminal.
```

---
## \#4 Posted by: chaka Posted at: 2016-08-12T03:46:46.493Z Reads: 38

```
You may want to re-flash just the bootloader and see if it clears up.

Are these the commands you used when flashing the bootloader? Assuming you are on ubuntu.

mkdir BLDC
cd BLDC
git clone https://github.com/vedderb/bldc-bootloader.git bldc-bootloader
cd bldc-bootloader
make upload
```

---
## \#5 Posted by: ambrojohn Posted at: 2016-08-12T04:12:38.835Z Reads: 31

```
Oh yeah! It worked.
I totally missed that bit...somehow, because the progress bar was working, I assumed the bootloader to be present already.

Thanks for the hint!
```

---
