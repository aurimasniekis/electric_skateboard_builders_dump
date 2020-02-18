# VESC turns on for 3 seconds, then turns off. (Help wanted)

### Replies: 2 Views: 92

## \#1 Posted by: VECTOR.xyz Posted at: 2019-07-28T01:02:55.357Z Reads: 23

```
Here's another post about a broken vesc:

I had purchased a flipsky 50a fsesc (the one with a CNC'd case), and it was running perfectly for a couple of days in my 10s board with a torqueboards 6374. I decided to take apart my skateboard to do some more padding, and after I was finished with the padding, I plugged my motor in again and decided to test if the motor would spin in the desired direction. To my surprise, when I pulled the trigger on the PWM remote, the motor did not move. Turns out that I forgot to plug in the motor sensors. I turned the vesc off, plugged in the sensors, and turned the vesc back on. After about 3 seconds, the vesc turned off (the blue led shut off) along with the PWM receiver. Now, when I plug the vesc in, all it does is turn on the led for 3 seconds, and then turn off. If the vesc stays plugged in, the DRV and the other chip on the board get warm. For some reason, when I connect the vesc to my 30v power supply, it stays on, cant drive my motors, can't connect to USB, and the chips on the front of the board get really hot. I've ruled out the BMS as the source of the error.

I need help troubleshooting my vesc because I really don't want to buy another one as this is my second broken vesc (first one, a torqueboards vesc, broke for diagnosed reasons) and I don't want to wait for half a century for my vesc to come from overseas.

**Edit**: I have discovered the the chip on the vesc which is not the DRV overheats in 3 seconds and shuts off. Still no idea what is causing this, still need help
```

---
## \#2 Posted by: AlanZhou Posted at: 2019-07-28T01:18:18.271Z Reads: 18

```
Could either be the MCU or the canbus chip
```

---
