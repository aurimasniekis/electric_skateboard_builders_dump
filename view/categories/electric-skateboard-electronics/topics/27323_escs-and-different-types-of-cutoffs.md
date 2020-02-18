# ESCs and different types of cutoffs

### Replies: 3 Views: 396

## \#1 Posted by: eldars Posted at: 2017-07-11T09:04:45.579Z Reads: 60

```
I have a battery/ESC related issue, that I am trying to debug for some time, I guess some of you had something similar, so could share some advice. 

I have 6S4P and 6S5P Li-Ion Panasonic NCR 18650B battery packs that I am using on my boards with 1 and 2 ESCs for 1 and 2 motors. Here is the ESC I use: https://www.aliexpress.com/item/Electric-skateboard-longboard-sensored-ESC-100A/32571133664.html?spm=2114.13010608.0.0.eNRKGa
The description states, that is is 100A ESC, so this should be enough for my battery pack.

I experience cut-offs since I started using this ESC and they happen quite often during the start or when I press full gas on the remote. With fully charged batteries the cut-offs are less often, but happen from time to time as well. I have tried to set "low voltage cut-off" setting to "to cut-off" on ESC to avoid these peremature cut-offs, because I have BMS installed anyway. However in this setting ESC just restarts and the cut-offs happen anyway.

When the battery has 50% of capacity left (anywhere from 21 to 22V out of 25),  then the cut-offs happen much more often, so it is not possible to use the board. I have also noticed, that the charge level indicator shows that the charge level is lower, when I press full gas on the remote. 

ESC manual says, that Low Voltage Cutoff can happen, when ESC detects one cell voltage below 3V of some manual setting (that I set to no cut-off), however I dont get, why I get these cutoffs with a fully charge battery? 

Aliexpress seller wrote me the following "According to your description,it is high current cut off,push full gas on the remote ,the current is probably over 100A,so the ESC cut off to protect the setup". Could that be the case with my 6S4P battery pack? As I calculated the burst current of my battery pack should be 12A x 4 = 48A (btw did I calculate it correctly?) that is twice less than the 100A, that ESC could handle.

Maybe these ESC are just no good, could you advice some other good and tested ESCs in the price range of 50-100$ besides VESC? Or is VESC the only way to go?
```

---
## \#2 Posted by: eldars Posted at: 2017-07-11T09:08:36.046Z Reads: 55

```
Just one more idea came to my mind. When I pressed full gas on my remote, ESC started to blink. ESC seller explained, that this blinking LED means of over-current protection. Could that be, that 100A ESC is just not enough for 6S4P 24 cell Panasonic NCR 18650b Li-Ion battery pack? I tried to use 120A ESC before and everything worked just fine with it.
```

---
## \#3 Posted by: Okami Posted at: 2017-07-11T15:15:01.861Z Reads: 33

```
Hard to tell what is happening but it looks like your esc is acting up. Im not sure who has the same esc to help you out.. maybe on reddit or elsewhere there are people who have tried it?

I think besides esc you can also try FVT 120 6s but the brake force / acceleration smoothness wont be the same and it looks like there are people who still manage to burn these.
```

---
