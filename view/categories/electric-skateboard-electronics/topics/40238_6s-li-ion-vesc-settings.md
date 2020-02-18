# 6s Li-ion VESC Settings

### Replies: 1 Views: 393

## \#1 Posted by: kyletrainy Posted at: 2017-12-06T00:25:13.799Z Reads: 55

```
I'm a noob and I would really appreciate if someone could check over my vesc settings. I really don't want to fry anything when I actually set up the vesc. I tired to provide as much info below about the battery as possible. Anything that I should change? I feel semi-confident that the settings below will work.

6s4p liion battery pack from diy w/ Panasonic NCR18650PF cells 
Nominal Voltage: 3.6-3.7V

BMS rated for 30A continuous output, 80A peak output
The batteries are rated for 10A continuous discharge so 40A total continuous discharge but the BMS can only handle constant 30A.

I have the torqueboards 6355 260kv motor and receiving a focbox in the coming weeks. There aren’t many hills in my area and the black friday deal made the pack and enclosure only $185, so I couldn’t resist as I also have a tight budget. 

Current Limits
Motor max: 60A
Motor min (regen): -40A
Bat max: 30A
Technically I think I can increase bat max to around 40A or 50A and be under the peak output, but I’m afraid of stressing the bms with too much current...
Bat min(regen): -12A
Absolute max: 130A
Voltage Limits
Min input voltage: 8V
Max input voltage: 57V
Battery cutoff start: 18.6V (3.1V)
Battery cutoff end: 17.4 (2.9V, minimum is 2.5V but I want to keep it a little higher)
```

---
