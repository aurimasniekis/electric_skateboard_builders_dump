# Help with math problem on Openoffice Calc

### Replies: 6 Views: 442

## \#1 Posted by: Brad Posted at: 2018-04-08T12:47:15.110Z Reads: 64

```
Hello

I'm having problems making my own e-skate spreadsheet.

As you can see, I'm working on this middle equation about power required to go up an incline.
![Screenshot-2018-3-5 Electric Longboard Gear Ratio|506x500](upload://mAJ92lMENhPqYlte02lTnbj0FjQ.png)

Now, I can get the correct answer via my iPad calculator as seen below which would round up to 502 watts. See my calculations in the history box at the bottom left.....
![Calculater|666x500](upload://iJZ2fwriVf4P1jHjHYyZ40A601x.jpg)

For some reason I just cannot get the damn equation to work in Openoffice Calc (Excel) as you can see below. 1km/h is 0.277778 meters a second, so I multiply by speed.
![Math problem|690x92](upload://bcl3gP8YBrvs6Ch76B2YWZni9Ca.PNG)

Have not done any math for ages now and am just about to give up after trying to fix this for about an hour. Google was great to find SIN and Power functions, but still....

Any pointers?
```

---
## \#2 Posted by: lock Posted at: 2018-04-08T14:40:21.346Z Reads: 48

```
Fairly sure the `sin` function is expecting radians. Try replacing `sin(n4)` with `sin(radians(n4))`.
```

---
## \#3 Posted by: Brad Posted at: 2018-04-08T14:52:33.686Z Reads: 44

```
[quote="lock, post:2, topic:51576"]
sin(radians(n4))
[/quote]

Well, shit. That did it. Was sure it was something so simple. It off by 0.5 but that is close enough for me.  :slight_smile: 

Thanks, really enjoying learning how to do Excel.
```

---
## \#4 Posted by: Brad Posted at: 2018-04-08T16:54:22.494Z Reads: 34

```
Having trouble finding cube 3. I'm sure Openoffice Calc does not have that feature. 

I read somewhere that cube 3 is the same as 1^1/3, but when I use that, I get an entirely different number. :sweat:

EDIT: Never mind, managed to find the solution [here](http://misapuntes.info/FuncionesOpenOfficeCalcIngles/POWER_Function_OpenOffice_org_Calc_3.htm). Solution was =POWER((K3/(0.5*1.225*1*0.9));1/3)*3.6 to calculate km/h speed for equation at the top of quick analysis image :rofl: 

Forum bugged out "*" in some places....
```

---
## \#5 Posted by: faithfulpuppy Posted at: 2018-04-08T17:43:48.069Z Reads: 20

```
use 1^(1/3)
```

---
## \#6 Posted by: oyta Posted at: 2018-04-08T17:48:15.941Z Reads: 19

```
a^(1/3) = cuberoot( a )
```

---
