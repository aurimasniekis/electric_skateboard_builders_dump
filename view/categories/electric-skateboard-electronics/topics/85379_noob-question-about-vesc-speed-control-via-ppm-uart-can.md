# Noob question about VESC speed control via PPM, UART, CAN

### Replies: 4 Views: 472

## \#1 Posted by: SeVeSeventyOne Posted at: 2019-02-25T18:09:17.694Z Reads: 114

```
HI there.
Building a remote controller(wired) and I wonder, is VESC working as well with PWM receivers/signal, or strictly PPM?
Is there a protocol documentation how to control VESC via UART or CAN, and is the protocol included with address and CRC?

Thanks.
```

---
## \#2 Posted by: mynamesmatt Posted at: 2019-02-26T00:07:54.564Z Reads: 96

```
i believe everything you need to know is on Benjamin vedders Page (or Blog or whatever).

Also I recall someone saying that it is actually pwm and not ppm that vesc can take
```

---
## \#3 Posted by: angeljmm Posted at: 2019-02-26T14:45:56.684Z Reads: 77

```
Hello,
you can also use ADCinput (resistance variation) as a wired input. Easy to setup (3,3v, GND and ADC)
```

---
## \#4 Posted by: SeVeSeventyOne Posted at: 2019-03-04T12:48:50.597Z Reads: 62

```
On many sites VESC is said to use PPM signal as one of the alternatives to control the output of the drive. However some sites say VESC uses PWM refered as "servo signal". Servo signal itself is 1-2ms pulse repeated every 20mS. I find it bit odd that VESC would only accept PPM as it is only developed to simplify wiring between receiver and some quad FC to pack multiple signals to one single wire. VESC only uses one signal channel as throttle why would it accept only PPM in that case?. Or is the VESC adaptive accepting both PWM and PPM as they include the same information?
```

---
