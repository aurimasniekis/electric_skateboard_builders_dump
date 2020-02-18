# VESC PPM connection problems

### Replies: 1 Views: 208

## \#1 Posted by: xilw3r Posted at: 2018-05-15T10:21:56.067Z Reads: 51

```
Hello people.

I guess many are using UART and what not to connect thir VESCS, but I am a simple man and I tried just to use an arduino with servo library to give 1 - 2 ms pulse to the vesc for control. Wireless communication happens through NRF24 modules.

I set everything up, codes seem to work fine, I connect stuff up and when I start up VESC tool input wizzard for PPM I get some weird stuff...

It just hovers (very slightly fluctuating) around 1.7ms and does not respond to anything I do with the potentiometer on the transmiter side, If i connect another pin from the arduino (one not set up for servo output)I get nothing at all. I tried switching servo output pins, same result. I also tried switching the arduinos themselves (receiver became transmitter), then its pretty much the same, but I got a slight hovering around 1.6 ms with the other duino...

VESC tool terminal does not show any bugs with the "faults" command.

Anyone have any idea what this might be caused by? I am affraid my VESC has some hardware problems. But I dont know how to check for that.

Thanks a bunch..
```

---
