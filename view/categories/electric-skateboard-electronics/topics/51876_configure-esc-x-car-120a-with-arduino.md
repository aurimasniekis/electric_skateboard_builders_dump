# Configure ESC X-CAR 120a with Arduino?

### Replies: 2 Views: 595

## \#1 Posted by: Waiboard Posted at: 2018-04-10T21:32:12.454Z Reads: 46

```
Hi, I'm going to describe my problem:

A few days ago my GT2B broke down (with Sparkle mod). I am from Argentina and unfortunately it is not so usual for my country to use control radios with a rechargeable battery like the Flysky GT2B. So I would have to replace it with one with AAA batteries adding weight and discomfort since I would not enter the Sparkle mod.

Buy 1 remote nano TorqueBoards 2.4ghz but when braking it does it very violently. If I try to brake again, only the reverse gear is activated. Brake only if I do not release the trigger. If I release it, the second time the reverse gear is activated.
I know that I have to configure my ESC or easier to buy a VESC. But in my country the programmer card is not obtained and I already spent my budget to buy one of the two abroad.
My longboard uses 1 ESC X-CAR 120a, does anyone know how to configure it using Arduino?

P.D: I am building the control of @twinsen since it is thinking to be used with ESC instead of VESC.
But I'm afraid it will not work properly as the GT2B did because I can not configure the ESC.

Thank you very much!
```

---
## \#2 Posted by: Twinsen Posted at: 2018-04-13T15:35:47.313Z Reads: 20

```
You will need to configure the ESC to not use reverse gear, only brake.
I think you can configure yours with the beeps. See the uploads section of https://hobbyking.com/en_us/hobbykingr-x-car-120a-brushless-car-esc-sensored-sensorless.html?___store=en_us
See the diagram in the manual. 

But be careful since it's easy to make mistakes, also your esc might map the settings differently, so double check everything you change.
```

---
