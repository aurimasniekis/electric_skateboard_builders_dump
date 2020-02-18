# (asknig for views / Recomindations) are my Dual Vesc&rsquo;s sutups correct?

### Replies: 7 Views: 230

## \#1 Posted by: ciscotory Posted at: 2018-11-15T16:22:07.144Z Reads: 63

```
guys would like your views / recomindations on what i've set for Dual vesc's suing BLDC tool beofing testing out, are they correct or do i need to adjusct anything? 

my duild is
10s3p / 36v / 60amp bms / Samsung 30Q
two 190 kv motors 
two vesce fw 2.18

here are some pics:
**for master vesc config**

master Motor config
![1%20master%20Motor%20configs|690x352](upload://cvc1lNsmmATVncJhDyOAwQfJO0q.jpeg) 

qusiton is the Batt max  40.00A above picter repsonsible for top speed? setting it up to 40 insted of 60 will reduce top speed is that correct? 


master bldc config
![2%20master%20bldc%20config|690x354](upload://9ifhCcQWP6nBHFsHhC3VPI5nPov.jpeg) 

master app general config
![3%20master%20app%20general%20config|690x355](upload://woCxatEfrexln20TelZe5BlexCF.jpeg) 

master app Uart config
![4%20master%20app%20Uart%20config|690x353](upload://4NOLCmM2XnMP3Dv460K48KsJ0XK.jpeg) 

master app Nunchuk config
![5%20master%20app%20Nunchuk%20config|690x359](upload://wSKMpmRSifaeNrAfTffHYRlyWMc.jpeg)

and for Salve:

Slave motor config
![1%20Slave%20motor%20config|690x347](upload://ze7vLu5qfotpjHarlwpH60JYfdG.jpeg)  

Slave BLDC config
![2%20Slave%20BLDC%20config|690x357](upload://ea7ExDaD6iLyqTbYwjZEVtonCGK.jpeg) 

 Slave app gneral config
![3%20Slave%20app%20gneral%20config|690x353](upload://nXP6cFQEFCMbu5n81HsMhEvyx1k.jpeg) 

Slave Uart config
![4%20Slave%20Uart%20config|690x353](upload://hJR2aF4egNi6InLiKYdvrfCld3e.jpeg) 

Slave app Nunchuk config
![5%20Slave%20app%20Nunchuk%20config|690x354](upload://wECA525mZ5mAvHFWzaCzvGNmTTV.jpeg) 


thank you all in advance
```

---
## \#2 Posted by: Trdolan03 Posted at: 2018-11-15T16:28:10.686Z Reads: 49

```
It will only reduce speed in hills theoretically. You will have no problems at 49 but if you want more “punch” up it to 60.
```

---
## \#3 Posted by: ciscotory Posted at: 2018-11-16T02:25:03.154Z Reads: 42

```
aha!! alright, reason wanted to redusce top speed cus wanted to make jurny less exrteem XD around 20kh 
( as in theory, the board setup would reach around 55kph which is 40 ish in real life according to esk8 calculature)
 and abit more efficent with range ( for the battary  in my build )
thanks a lot man,
```

---
## \#6 Posted by: skatardude10 Posted at: 2018-11-16T02:46:43.963Z Reads: 36

```
I would set your battery max to 30A for each vesc to be within your BMS limit of 60A total, and 20A per cell for 30Qs. 

Additionally I would set your battery min to -6 to -8 on each vesc to be 4A charge per cell or a tad bit more for stronger breaking when you need it.
```

---
## \#7 Posted by: ciscotory Posted at: 2018-11-16T03:40:47.299Z Reads: 34

```
oh!! great point man, for matching battaery max to 30A for both, i just rememberd I've read it a while back and forgot i,  brilliant :+1: 
so battery max 30A and  battery min  ( -6 or -8 ) for each VES, okey got it :v:

quistion: which part / section in Motor tab i need to change 20A for per cell of the battary?
thanks a lot man!!
```

---
## \#8 Posted by: skatardude10 Posted at: 2018-11-16T14:30:34.570Z Reads: 24

```
You don't have to change any of the settings to 20A, just think of however many P you have multiplied by 20, then split that across your vescs for battery max (3P * 20A = 60A / 2 vescs = 30A per vesc). I hope this clears up any confusion. 

If you want to be a bit more conservative since 30Q cells are really only rated for 15A (they seem to do fine up to 20A per cell though), you can do  22.5A per vesc to equal out to 45A total (3P * 15A = 45A across both vescs / 2 vescs = 22.5A per vesc batt max)
```

---
## \#9 Posted by: ciscotory Posted at: 2018-11-17T16:07:14.550Z Reads: 17

```
Fantastic while searching and reading Ur reply
I understand now ✌️
Very helpful
Thanks very much..
```

---
