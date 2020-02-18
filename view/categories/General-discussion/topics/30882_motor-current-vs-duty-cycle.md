# Motor current vs duty cycle

### Replies: 4 Views: 487

## \#1 Posted by: Esrapp21 Posted at: 2017-08-17T14:07:47.735Z Reads: 102

```
I have a project in the works and I need a way to tell how much the motor is working at a given time. Would motor current or duty cycle be a better representation of this?
```

---
## \#2 Posted by: onepunchboard Posted at: 2017-08-17T18:15:52.700Z Reads: 88

```
power= V x Amp. connect vesc via Bluetooth download app phone and see how much motor draws
```

---
## \#3 Posted by: wafflejock Posted at: 2017-08-17T18:44:09.804Z Reads: 77

```
You can check this in the BLDC tool (activate sampling for real time data) only problem with doing that mobile is keeping a cord plugged in while you ride the board under load (you could use a laptop in a backpack but keeping the USB wire free from getting tangled might be tricky).   The http://metr.at module is totally worth it, got it sent to the US in about a week and is almost plug and play (few setup steps required but went smooth for me).
```

---
## \#4 Posted by: Esrapp21 Posted at: 2017-08-17T18:57:26.399Z Reads: 70

```
I actually have the metr.at device. I decided motor current would probably be my best bet
```

---
