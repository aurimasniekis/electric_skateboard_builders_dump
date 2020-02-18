# Ackmaniac Android App not showing data, hardware or software issue?

### Replies: 1 Views: 161

## \#1 Posted by: Spyro Posted at: 2019-02-01T16:13:41.412Z Reads: 37

```
Hi guys, I recently had some issues with the Ackmaniac android app not showing data / shows data periodically.
So basically I was using adc+uart on my e-bike. I decided to use an arduino to convert the adc input to ppm input so I could change modes on the android app. This was prior to the 3.103 update which allowed mode change on adc.
I accidentally swapped tx rx for 5v and gnd. Then when I swapped it back to the correct position, the android app stopped showing data. All I did was change to ppm+uart from adc+uart. Everything else was the same. The vesc worked fine, no issues with performance at all. The bluetooth data just didnt show. I changed a bluetooth module and got it to work for 5 minutes. Then it just stopped working again. I took it out for a ride and it worked, I could change modes and everything. Then it just stopped again.
I thought that I could have damaged my vesc by my mistake of swapping tx rx with 5v and gnd. So I tried to solder jumper wires to pin 28/29 on the microcontroller on the vesc itself after reading about someone having same issues as me (intermittent connections) and having success connecting 28/29 directly to the bluetooth modules, bypassing the traces on the pcb of the vesc. I ended up fucking that up and that was the end of my vesc.

So I bought another one, and the same issue happened.
I doubt it’s software since it’s intermittent, it’s not weak signal, I put my phone right next to the module and it still didn’t work. I doubt its hardware since I changed to a whole new vesc.

Whenever I unplug the vesc, the data suddenly shows up on the android app. Like for a split second it sends data before I unplug it completely. This is what shows up during the unplugging process.
![44bfb202ebebdcfb1f5cab0c66a0cb82b47316ed_1_281x500|281x500](upload://p4S0q0hC8XXA9a9wPtbCQT3xPAF.jpeg) 
I honestly don’t know what could be the problem, I reinstalled everything, factory resetting my phone as well, trying with another phone, same issue.
If anyone could provide some insight into this I would be very thankful.
```

---
