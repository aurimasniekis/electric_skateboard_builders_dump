# Powering a NodeMCU development board from 10S battery pack

### Replies: 1 Views: 153

## \#1 Posted by: janpom Posted at: 2019-02-26T21:08:21.185Z Reads: 38

```
My custom external BMS charger ([picture here](https://www.electric-skateboard.builders/t/no-words-just-pictures-delete-words/2992/9748)) is controlled by the NodeMCU. It can take up to 10V of input voltage. So far I've been powering it up from a 5V USB adapter, but that's clunky since I have two things to plug into the wall socket (5V adapter and li-ion charger). I'd like to power it up from the 10S battery pack / li-ion charger using a buck converter. I'll need one that can bring 42V down to ~8V, which should be safe for the NodeMCU.

I have already done one such attempt with [this buck converter](https://www.aliexpress.com/item/10A-DC-DC-6-5-60V-to-1-25-30V-Adjustable-Buck-Converter-Step-Down-Module/32861200188.html). I got magic smoke in about 2 secs after connecting the battery pack. :( After that I ordered new buck converters, which arrived today, so I'm doing more testing and being more careful this time. The buck converters are [these ones](https://www.aliexpress.com/item/LM2596HVS-LM2596-HV-LM2596HV-DC-DC-Adjustable-Step-Down-Buck-Converter-Power-Module-4-5-50V/32878065864.html).

https://ae01.alicdn.com/kf/HTB1DOvkLXXXXXaPXpXXq6xXFXXXO/LM2596HVS-LM2596HV-DC-DC-Adjustable-Step-Down-Buck-Converter-Power-Module-4-5-50V-to-3.jpg_640x640.jpg

This time I first tested the buck converter with a lower input voltage. I set up 8V output and tested that it remains stable when varying the input voltage. It worked fine. Then I connected my 42V charger (rather than the li-ion pack). Still worked fine. The only problem was that I got some sparks when connecting the charger. The charger can only do 2A. I'm worried that there could be more sparks when connecting the battery pack.

One idea was to connect a resistor in series with the buck converter. I tried a 150 Ohm resistor and that seems to have worked pretty well. No sparks. I got 6V of voltage drop across the resistor, so the input voltage for the buck converter got reduced to 36V, which should be even more within the safe range.

I wonder if the resistor is a bad idea though. I guess it could be a problem should the load increase significantly. The 6V at 150 Ohm implies 40 mA of input current and 1.44W (40mA @ 36V) buck converter input power. For example, if the load doubled, the input power would have to (roughly) double as well. However, with increasing current, the voltage drop across the resistor would also increase, reducing the buck converter input voltage and forcing the input current to go even higher. For 2.88W of input power, 120 mA of input current would be needed (18V drop across resistor; 24V at buck converter input; 24V * 120 mA = 2.88W). That's probably still OK as long as the resistor can withstand 2.16W, but it's already close to getting out of hands.

On the other hand, I don't expect significant changes in the load. During my quick experiments it remained pretty stable around 1.1W (135mA @ 8V). Also, a lower resistance resistor (100 Ohm? 50 Ohm?) would probably still prevent sparks and it would allow higher input power should it be needed.

Any ideas, suggestions, and words of caution would be highly appreciated.
```

---
