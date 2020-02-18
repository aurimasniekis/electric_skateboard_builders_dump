# Where to find a 12S UBEV to 12V

### Replies: 10 Views: 629

## \#1 Posted by: karma Posted at: 2017-07-26T12:22:42.513Z Reads: 79

```
Like the title says, where could I find a suitable 12S voltage regulator/buck converter/UBEC that steps down the voltage to 12V? The reason I need it is because of a 12V DC to AC inverter for EL-wire.
I can't find any rated for such a high voltage, all i find is 40V max input.
```

---
## \#2 Posted by: vap Posted at: 2017-07-26T12:40:05.869Z Reads: 78

```
I've used this for cooling fans and leds:
https://www.banggood.com/3Pcs-5V-60V-To-1_25V-30V-LM2576HV-DC-DC-Step-Down-Module-p-1066628.html?rmmds=myorder
Haven't exploded on 12s
```

---
## \#3 Posted by: Stefan Posted at: 2017-07-26T12:51:11.583Z Reads: 70

```
Be sure the buck converter you are going to buy is rated for the amount of current you want to draw from it.
The suggested one by @vap is capable of 3A, but i would not draw more than 2A continous if i were you. If you need more then buy a bigger one.
```

---
## \#4 Posted by: Cobber Posted at: 2017-07-26T13:02:38.011Z Reads: 62

```
I'm using one of [these](https://hobbyking.com/en_us/yep-20a-hv-2-12s-sbec-w-selectable-voltage-output.html) in my current build :)
```

---
## \#5 Posted by: vap Posted at: 2017-07-26T13:15:02.438Z Reads: 59

```
Right, at 12V i wouldn't recommend more than 1A on LM2576. Still enough for couple of leds.
```

---
## \#6 Posted by: longhairedboy Posted at: 2017-07-26T13:17:47.642Z Reads: 59

```
https://www.amazon.com/gp/product/B01J5M84FG/ref=oh_aui_detailpage_o02_s00?ie=UTF8&psc=1
```

---
## \#7 Posted by: longhairedboy Posted at: 2017-07-26T13:19:05.453Z Reads: 52

```
I've cooked a couple of these when running 12v LED lights off of them for extended periods of time such as for bright underlighting. They get really hot.
```

---
## \#8 Posted by: karma Posted at: 2017-07-26T13:26:28.229Z Reads: 49

```
Seems a little too small to handle the job I want to do. It probably works great for smaller applications though.
```

---
## \#9 Posted by: karma Posted at: 2017-07-26T13:26:54.926Z Reads: 51

```
That's some good current capabilities but the highest output voltage is only 9V. :(
```

---
## \#10 Posted by: karma Posted at: 2017-07-26T13:27:40.966Z Reads: 49

```
@longhairedboy That should work, thanks!
```

---
