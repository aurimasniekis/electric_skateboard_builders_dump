# While riding motor suddenly started going backwards randomly, now &ldquo;Bad Detection&rdquo;

### Replies: 3 Views: 180

## \#1 Posted by: iamking Posted at: 2019-06-08T00:10:45.903Z Reads: 77

```
Hello everyone this is my first board and it recently stopped working,

I know there are quite a few threads on this already and I've tried following most of them with similar setups but it's still not working out. 

With these exact same numbers, I was able to previously get it to work already. I rode it for an entire 3 days but then suddenly it started stopping randomly. I continued riding it then suddenly it just completely stopped working. (When I checked the board, a wire was pulled out of the motor. When I tried plugging it back in, it still didn't work.

I used 60/-60/30/-12 as suggested by diyelectricskateboards.com
My battery is 12S2P with a BMS from @oriol360 
My motor is 6374-192KV Brushless Outrunner Motor. (Voltage: 10~12S Lipoly, RPM/V: 192KV, Internal resistance: 0.016 Ohm, Max Loading: 80A, Max Power: 4032W)

I tried rebooting it as @Tampaesk8er suggested. The VESC connects well and I get all the way up to the part where I need to test the motor and let it freely spin. When I click the button the VESC starts flashing red.

Below are photos of my setup.

![IMG_3363|375x500](upload://gHlyL4vRaR8iHqqp900SJJYjydl.jpeg) ![IMG_3365|375x500](upload://kedcdZoQTYHlpVJc1NXVVVeQZg3.jpeg) 

*P.S. There's a lot of duct tape because I was just testing it first before drilling everything in permanently.

Thanks everyone!

Debug Console:
2019-06-07 16:50:02: Status: MC configuration updated
2019-06-07 16:50:15: Status: MCCONF Write OK
2019-06-07 16:50:15: Status: MC configuration updated
2019-06-07 16:50:17: Status: MCCONF Write OK
2019-06-07 16:50:17: Status: MC configuration updated
2019-06-07 16:50:33: Status: Bad Detection Result Received

Terminal:
AULT_CODE_NONE


Here are screenshots of the setup:
![43%20AM|690x388](upload://djr6Q88QweChy9vFvN75BELfYDu.png) ![54%20AM|690x387](upload://zF1r99JLLlnWAJvutUPXFhiLnSI.png) ![27%20AM|690x391](upload://qq6PnzLkwBEQ48jjQj4ZDHmgoHc.png)
```

---
## \#2 Posted by: dareno Posted at: 2019-06-09T03:08:58.215Z Reads: 37

```
Don't do a re detect till you check your motor is good.  You'll potentially damage your vesc.  
Did you see any magic smoke from the motor?
You can check your windings very simply by hand.
Let’s say the phase wires on the motor are **A, B**, and **C**

**Disconnect them from the ESC**

Touch A+B together. Verify the motor has choppy brakes

Touch A+C together. Verify the motor has choppy brakes

Touch B+C together. Verify the motor has choppy brakes

Touch A+B+C together. Verify the motor has SMOOTH brakes that are much stronger

All the choppy brakes should feel the same. If one is weaker or stronger or if anything isn’t as described above, it means you might have winding issues.
```

---
## \#3 Posted by: iamking Posted at: 2019-06-09T04:13:12.891Z Reads: 29

```
@dareno thanks for the reply! 

Yes, all of them are exactly as you described. I did not see any smoke at all.
```

---
