# Smart BMS - Cell overvoltage

### Replies: 11 Views: 1844

## \#1 Posted by: hemulius Posted at: 2018-08-23T21:16:53.083Z Reads: 157

```
Hi!

Got a Smart BMS (one of those with and Android app)

https://www.lithiumbatterypcb.com/product/13s-48v-li-ion-battery-pcb-board-54-6v-lithium-bms-with-60a-discharge-current-for-electric-motorcycle-and-e-scooter-protection-2-2-3-2-2-2-2-2/

After connecting the BMS and changing the batteries I have a question.

I get a cell overvoltage message when changing. I have tried to dischange and charge a couble of times. Also changed some of the parameters (balance-turn-on-voltage reduced to 3.8 and tried with other than change-balance mode).

Can it be an error with the BMS? I thought it should handle a difference of 0.1-0.2V while changing. I have changed with 1.35 A. It's a 10S3P pack.
```

---
## \#2 Posted by: rey8801 Posted at: 2018-08-23T21:20:44.553Z Reads: 148

```
I think @bartroosen12 has the same one. Maybe he can help you.
```

---
## \#3 Posted by: bartroosen12 Posted at: 2018-08-24T07:19:24.824Z Reads: 117

```
Do you have a screenshot of your parameters from the app?
```

---
## \#4 Posted by: hemulius Posted at: 2018-08-24T07:37:19.314Z Reads: 116

```
![IMG_7204|375x500](upload://f5FgHNWsN0gbDsqRejFBE2vatWd.jpg)![IMG_7206|375x500](upload://7QjddTuj6CP3012ReWZtdiKVVfm.jpg)![IMG_7210|375x500](upload://43xddtr9lAx2GCKECAYwkYNLGc3.jpg)![IMG_7205|375x500](upload://odY4SmwM8XiVdvy43calbRD7ipF.jpg)

Here are some screenshoots.

After theese photos where taken I changed the mode into static, and let the battery rest for a couple of days. Still not balanced.
```

---
## \#5 Posted by: Andy87 Posted at: 2018-08-24T07:55:26.775Z Reads: 103

```
What batteries you use? Maybe it’s because you set your cycle cap to 8ah? 
With 3p 3ah cells it should be 9ah, no?
```

---
## \#6 Posted by: hemulius Posted at: 2018-08-24T08:14:57.809Z Reads: 100

```
Yes. Thats right. I use Samsung INR18650-30Q, so it's 9A in total.
I was a bit unsure what the difference in nominal and charging capacity is.

BTW: The battery pack had an BMS from BesTechPower (http://litechpower.com/product-detail/HCX-D528V1LI10S.html) that perfectly balanced the pack. But to save space i split it in two and accidentally cut the temperature wire. After soldering it back on the BesTechPower BMS worked a couple of times, but then it stopped working. I verified that the switch is OK. I guess it's the temperature sensor.
```

---
## \#7 Posted by: bartroosen12 Posted at: 2018-08-24T08:16:50.402Z Reads: 96

```
Is this a new pack? Or just and older unbalanced pack which has thr new smart bms now?
Put your overvoltage to 4.2V
And overvoltage release is fine.

You got balance mode on charge only so if you unplug the charger the batteries won't balance, so you need to select the other option if you want to balance when not connected to the charger.
Just put your Precision on 0.005 and plug your charger in and let it balance for a day.

My friend had the same thing with old cells and all the time 1 cell hits 4,2V but the bms will discharge that cell and when it's lower than 4,15V all cells start charging again until 1 cell hits 4,2V.
It's only the first time, if you buy new cells and if they are all the same voltage you won't have this issue.

The capacity doesn't matter, that's just used to calculate the range but won't affect charging batteries.
```

---
## \#8 Posted by: hemulius Posted at: 2018-08-24T09:21:00.988Z Reads: 91

```
It's a new pack.

Only charged one time with the BesTechPower BMS. Then I discharged it once without any BMS (only to 60-70%). Then it's charged with the new Smart BMS.

I have set the other charge mode (static) some days ago. The difference might have become less, but it seem like it will take many days to difference is less than 0.03v.

Should I balance it manually and see if that helps?
```

---
## \#9 Posted by: bartroosen12 Posted at: 2018-08-24T09:30:51.625Z Reads: 82

```
If your voltage is like 0,2V difference like you showed in the picture that's to much and it will take for weeks to balance that if you just leave your pack without a charger connected.

Just put balance on 'open'
Change the values like I said and plug in the charger. If you plug in the charger balancing will be much quicker.
Just leave it plugged in when you're at home and they will be perfectly balanced.
```

---
## \#10 Posted by: hemulius Posted at: 2018-08-24T09:32:35.190Z Reads: 79

```
OK thanks. I will give it a try.
```

---
## \#11 Posted by: bartroosen12 Posted at: 2018-08-24T11:42:06.440Z Reads: 74

```
These are my settings and info about my cells.
I've actually never had a overvoltage error.
![xiaoxiang|281x500](upload://zZJ22CoxVlfnhyVoUYpHs3f6aI1.png)
![xiaoxiang|281x500](upload://gCmtZ1Hgazt3YoiqKUuKGkSL5k9.png)
![xiaoxiang|281x500](upload://h2NvVOmeThNRj5RnDdaalNHWg46.png)
My charger is 41.5V so it will never go exceed 4.15V per cell.
Maybe because you got a 42V charger (or a bit more if you measure the charger output) you need some higher values
I should try to set overvoltage to 4.25V and overvoltage release to 4.22V, otherwise it's logic you will get a overvoltage notification.
I should measure your output of the charger first devide by 10 and set that value as you overvoltage release, maybe a tiny bit more +0.01V just to be sure.
```

---
