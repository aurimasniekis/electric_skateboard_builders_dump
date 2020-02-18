# Esk8 VESC issues, goodbye for a while esk8 :(

### Replies: 24 Views: 1273

## \#1 Posted by: westonbe Posted at: 2018-01-15T20:38:22.110Z Reads: 215

```
I'm about to give up esk8ing for a while :(. Just blew up my 2nd DRV chip from the same issue as my first vesc. A small rock got caught in the motor, it started stalling and blew it up. There was a burn mark of the plastic on the shrink wrap over the drv chip. I unfortunately don't have the $$ for another vesc and won't have any for another year until university ends. :(. I have everything set conservatively on my bldc and was wondering what causes the drv chip to blow up? This is extremely frustrating considering the amount of time and energy I've put into this board for me to be limited by this. I am extremely bummed out by this. Thank you guys for your time, and I appreciate the help the esk8 community has given over the past year. If anyone is in the socal area and knows how to replace a drv chip let me know. If not, goodbye for now everyone, love you guys
```

---
## \#2 Posted by: Martinsp Posted at: 2018-01-15T20:52:57.102Z Reads: 203

```
That is sad to hear :/ I can fix it for you for the cost of shipping to me and back. I am located in Slovakia. Where are you from?
```

---
## \#3 Posted by: Jammeslu Posted at: 2018-01-15T21:05:04.815Z Reads: 199

```
Sorry to hear, completely get the limited economy during university
```

---
## \#4 Posted by: Okami Posted at: 2018-01-15T21:05:52.366Z Reads: 195

```
If you are low on cash u might as well just replace it with 'ebay substitute' esc.. though might be in similar price as the repair..

---
https://drvwizard.com/repairs-services

if ure in usa, then probably might be a bit cheaper than send to Eu.. though compare the deal then

EDIT: @Jasonkj3217 thanks for correction ;)
```

---
## \#5 Posted by: Jasonkj3217 Posted at: 2018-01-15T21:09:21.989Z Reads: 180

```
Sorry, but that’s actually @JohnnyMeduse website. He’s located in Montreal, Canada
```

---
## \#6 Posted by: bimmer Posted at: 2018-01-15T21:13:48.132Z Reads: 177

```
I'll fix it for shipping cost located in AZ.
```

---
## \#7 Posted by: westonbe Posted at: 2018-01-16T01:12:26.154Z Reads: 149

```
Hey Bimmer, I'll take you up on that. Also, to ensure this doesn't happen a third time, do you guys see anything wrong with this bldc configuration for current settings from my batteries to the motor?
SPECS: 12S (two 6S in series), 6k mAh, 25-50C, 2750W 192 kv 6374 turnigy motor. From what I've read and heard, my settings on the vesc are conservative when it comes to current draw... It cuts of when the voltage levels are at about 3.3V per cell. Thank you guys for the replies and your time, I appreciate it.

![jpegvescissue1|690x438](upload://iOVxrR0i2Jam8GaEidiOPheqzer.png)
```

---
## \#8 Posted by: westonbe Posted at: 2018-01-16T01:13:31.134Z Reads: 144

```
Woops, absolute current draw is set at 130 A/ always has been just messed with the setting but changed it back right away.
```

---
## \#9 Posted by: chuttney1 Posted at: 2018-01-16T01:29:20.750Z Reads: 136

```
Who's the maker of the VESC you have?
```

---
## \#10 Posted by: laurnts Posted at: 2018-01-16T01:35:49.917Z Reads: 138

```
Sorry to hear that mate, but again VESC quality vendor makes hige difference here. I have my VESC first from enertion, they totally destroyed after 15min. However I think the new FOCBOX didnt have this issue anymore as Ive read less complaints. Personally I have my VESC from chaka, its been 2 years they are still very solid.
```

---
## \#11 Posted by: westonbe Posted at: 2018-01-16T02:29:27.627Z Reads: 129

```
My first vesc was ollin board, and my battery current draw was set too high @65A, and found it troubling that their factory service warranty was not described on their site(did not cover anything on my vesc or any kind of repair), which is why I paid extra $$ for it. I accepted that pretty quick. My second vesc was a random guy from ebay, who had the current ramp step set at 4 instead of 0.04. But @chaka said, after testing various current ramp settings, that max current ramp had little to do with faulty drv's and he had yet to fail a vesc cause of it. I honestly have no idea if that  was the cause of this vesc failure.
```

---
## \#12 Posted by: b264 Posted at: 2018-01-16T02:32:27.237Z Reads: 121

```
What number are you talking about when you say current ramp
```

---
## \#13 Posted by: westonbe Posted at: 2018-01-16T02:36:58.798Z Reads: 121

```
The max current ramp step (@ 1 kHz), should be set to 0.04 from the default settings
```

---
## \#14 Posted by: b264 Posted at: 2018-01-16T02:39:10.478Z Reads: 120

```
What screen is that on in the BLDC Tool; what steps would someone take to see the number you're describing?


edit: oh, I see it's in the `Motor Configuration > Advanced > Backoff and ramping (DC and BLDC only) > Max current ramp step (at 1kHz)`
```

---
## \#15 Posted by: westonbe Posted at: 2018-01-16T02:57:44.498Z Reads: 116

```
Yup, that's it
```

---
## \#16 Posted by: ATLesk8 Posted at: 2018-01-16T03:01:15.470Z Reads: 112

```
What does that function even do? I’ve yet to make it that deep in the bldc tool
```

---
## \#17 Posted by: mmaner Posted at: 2018-01-16T03:06:44.783Z Reads: 112

```
In an older version if the firmware there was a bug that would cause the value to multiply when you open the config...or something like that.

I think it was @caustin that found it?
```

---
## \#18 Posted by: westonbe Posted at: 2018-01-16T03:08:17.792Z Reads: 116

```
@mmaner  Yea it was version 2.17-2.18, which was the vesc I was sold on ebay. The current bldc version is 4.xx something yea? I'm confused, do the vesc version and bldc version numbers match each other? Or the vescs are in the 4.xx digits and the bldc tool is still in the 2.xx digits?
```

---
## \#19 Posted by: b264 Posted at: 2018-01-16T03:25:58.354Z Reads: 105

```
To be clear, there are 4 versions

hardware (VESC) version, like 4.12 or 6.4
firmware version
BLDC Tool version
VESC Tool version
```

---
## \#20 Posted by: westonbe Posted at: 2018-01-16T05:20:16.608Z Reads: 100

```
Gotcha. @chaka said "Well I repaired your VESC and promptly fried it during load testing! I wish you had told me you messed with the max current ramp settings. I am going to have to send you a completely rebuilt VESC but you are on notice for being click happy with the settings. :wink: If you blow another one I am going to have to charge you little for the repair service." So now I'm not sure if max current ramp affects the drv chip.
```

---
## \#21 Posted by: Namasaki Posted at: 2018-01-16T05:45:48.611Z Reads: 93

```
The absolute max amp setting is a last resort protection in case the soft back off strategy fails. 
It should be set between 130a and 150a
I run mine at 140a. 
This info along with definitions of other Vesc settings is available on Vedder’s website.
```

---
## \#22 Posted by: caustin Posted at: 2018-01-16T06:01:02.510Z Reads: 89

```
Credit @Jinra

 http://www.electric-skateboard.builders/t/psa-remember-to-reset-your-max-current-ramp-step-when-programming-your-vesc/6262
```

---
## \#23 Posted by: Nordle Posted at: 2018-01-16T07:23:37.093Z Reads: 78

```
A vesc is 100bucks you can earn that much in 1 to 2 working days, unless you live in bangladesh.
```

---
## \#24 Posted by: Eboosted Posted at: 2018-01-16T07:34:33.164Z Reads: 77

```
Do not buy cheap parts, that's false economy, save money and start over again, don't get frustrated, it's not worth it, learn from it and make it again, this time better, later in life, after you graduate and get a good job you will realize that.
```

---
