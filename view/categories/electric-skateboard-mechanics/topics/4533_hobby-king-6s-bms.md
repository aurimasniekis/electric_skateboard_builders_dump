# Hobby King 6s BMS?

### Replies: 5 Views: 1759

## \#1 Posted by: adamm Posted at: 2016-06-11T00:17:22.271Z Reads: 146

```
Found this BMS on hobbyking and im wondering if anyone knows if it would be good for my 6s build?. I dont think the discharge of 10a is high enough though so im just checking 

http://www.hobbyking.com/hobbyking/store/__98294__BMS_Battery_Management_System_6S_LiPoly_4A_Charge_10A_Discharge.html
```

---
## \#2 Posted by: barajabali Posted at: 2016-06-11T00:22:54.694Z Reads: 144

```
No Bueno too low discharge just go to battery supports.com
```

---
## \#3 Posted by: sl33py Posted at: 2016-06-11T00:23:34.682Z Reads: 142

```
Unfortunately your answer is right in the title of the BMS:
[quote]BMS Battery Management System 6S (LiPoly) 4A Charge / 10A Discharge[/quote]

10A Discharge - no bueno for any e-board i know.  While you don't likely need a 100A discharge, you definitely need more than 10A.  My dual 5065 setup showed a consistent peak of 40-45A iirc.

HTH - GL!
```

---
## \#4 Posted by: adamm Posted at: 2016-06-11T00:48:12.723Z Reads: 127

```
Yeah thats what I was expecting thanks though
```

---
## \#5 Posted by: laurnts Posted at: 2016-06-11T04:41:00.411Z Reads: 108

```
You can use it for charging purpose but not for discharge purpose, its too low Amps. You need about 30A minimum with a better stability at around 80A discharge. If you plan to use it however anyway, better to connect the ESC / VESC from the battery directly.
```

---
