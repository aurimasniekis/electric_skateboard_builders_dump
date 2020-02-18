# Full brake on 3.40 firmware

### Replies: 4 Views: 254

## \#1 Posted by: 12meterkuk Posted at: 2018-08-24T18:23:02.290Z Reads: 118

```
Hey guys, how do I get the vesc to short the phase wire under a certain erpm? I can’t find the settings in the new vesc tool. I’ve set motor min to -100 and the brakes are still too weak at low speeds. Thanks
```

---
## \#2 Posted by: trampa Posted at: 2018-08-25T21:25:13.206Z Reads: 78

```
Whatsapp ist yourself Battery min? What  motor, gering, wheel diameter? That all has an impact on the brakes.
```

---
## \#3 Posted by: 12meterkuk Posted at: 2018-08-26T05:06:16.683Z Reads: 67

```
@trampa motor min is -100, batt min is -16,  gearing is 18/36 with 97mm wheels, motor kv is 100, with a top speed of a hair over 30kmph.
```

---
## \#4 Posted by: trampa Posted at: 2018-08-26T07:38:50.447Z Reads: 56

```
Your settings are not really perfect. Pretty long gearing and batt min is very low. Batt min defines braking power at speed while motor min is more dominant at lower speed. However, both values need to be in a reasonable range. 
Best linear braking behavior is achieved when both values are similar. Try -30A for both values to see what I mean. Your Battery needs to be able to cope with the currents! Usually braking currents happen for a short period of time only, which helps the battery to stay healthy. The biggest issue for a battery are long runs down a big hill with high brake current injection over a longer period of time. A short 25A to 30A injection is usually fine for a 3 to 4P cell pack with 20A rated cells. BTW, the VESC doesn't short phases. There is no such option available in the software.
```

---
