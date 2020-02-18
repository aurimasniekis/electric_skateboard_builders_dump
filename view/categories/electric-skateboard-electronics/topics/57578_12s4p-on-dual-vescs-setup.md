# 12s4p on dual vescs setup

### Replies: 20 Views: 637

## \#1 Posted by: JImmy2 Posted at: 2018-06-02T19:03:14.209Z Reads: 150

```
hey guys 
im building my own eboard but this time with vescs 4.12 
i have done one before but when i ride it the motors get hot and the vescs also
i burned them
 
can anyone help me with configure my new vescs ? 
i have ,
12s 8.8mAh battery 
max discharge current 158,4

270kv each 1400watt motors 
dual 2800watt 
can anyone please help me configure the vescs ??
```

---
## \#2 Posted by: Sender Posted at: 2018-06-02T19:22:16.813Z Reads: 145

```
That is a high KV for 12s
```

---
## \#3 Posted by: strattos Posted at: 2018-06-02T19:24:49.941Z Reads: 141

```
Yup motor kv is insanely high for 12s highest I've ever seen anyone run a 12s is with a 190kv and even then you might hit the erpm limits.
```

---
## \#4 Posted by: JImmy2 Posted at: 2018-06-02T19:34:30.981Z Reads: 128

```
Yes that’s right but those are the motors I got 
Can’t I configure it with a vesc ?
```

---
## \#5 Posted by: Kug3lis Posted at: 2018-06-02T20:07:27.453Z Reads: 120

```
VESC doesn't change motor mechanical properties ;)
```

---
## \#6 Posted by: JImmy2 Posted at: 2018-06-02T20:16:11.485Z Reads: 117

```
Yes but I want to know how many amps should I give the motor 
?
```

---
## \#7 Posted by: Kug3lis Posted at: 2018-06-02T20:17:34.745Z Reads: 107

```
Amperage will not change the fact your motors will spin too fast and with little torque to do anything much...
```

---
## \#8 Posted by: JImmy2 Posted at: 2018-06-02T20:30:39.805Z Reads: 106

```
Yes I know that but I mean how much amps should I give the motors so they doesn’t get hot or over current 
I know the kv is too high and they would spin so fast but It’s okay for me 
I want them to work for now then I can get others next month
```

---
## \#9 Posted by: rey8801 Posted at: 2018-06-02T20:40:12.253Z Reads: 105

```
I think what the other guys are saying is that the main problem with such high kv you will pass the 60000erpm limit on the VESC http://calc.esk8.today/
As result you will fry your vesc. The vesc as the feature to limit the max erpm number. I would enable this function but since you will limit the spin of your motor you are going to use them with a reduced performance.
```

---
## \#10 Posted by: Blitz Posted at: 2018-06-02T20:42:08.135Z Reads: 101

```
@moderators Doesn't Foc-mode not have Erpm?
or are there more factors to considered like RPM?
```

---
## \#11 Posted by: JImmy2 Posted at: 2018-06-02T20:55:46.335Z Reads: 97

```
Ahh okay wow then that’s why my old two vescs burned 
Then I should get other motors with a lower kv ?
```

---
## \#12 Posted by: rey8801 Posted at: 2018-06-02T20:57:26.601Z Reads: 93

```
yes, that's probably why. 170-190KV are perfect for 12s use the calculator to see if you are within the 60000erpm http://calc.esk8.today/
```

---
## \#13 Posted by: JImmy2 Posted at: 2018-06-02T21:03:10.468Z Reads: 93

```
oh yes true its 83916 erpm

thank you
```

---
## \#14 Posted by: rey8801 Posted at: 2018-06-02T21:06:22.001Z Reads: 92

```
You are welcome...with dual 170KV motor you will have an insane torque, go for 6355 or 6374 (if you want to fly :smile: )
```

---
## \#15 Posted by: rey8801 Posted at: 2018-06-02T21:10:12.413Z Reads: 89

```
I see you are using 4.12 VESC so if it is not FOCBOX probably is TB or Maytech. Since for such high discharge current you are running LiPo, remember to set the battery max on each vesc not higher of 30A if you are using these types of VESC. Ah and do not run FOC with them. Motor max can be set at max current the motor can handle (you can find it on the motor datasheet)
```

---
## \#16 Posted by: JImmy2 Posted at: 2018-06-02T21:15:01.754Z Reads: 83

```
yes im using the 4,12 VESCS and lithium battery samsung cells

actually i dont want to fry two others vescs so imma put everything together when i buy the new motors 
hah vescs are really expensive 
dont want to burn them again :smile: haha
```

---
## \#17 Posted by: rey8801 Posted at: 2018-06-02T21:19:23.816Z Reads: 80

```
ah ok so you are using Liion battery. Then it's more important the constant discharge current, because they are weaker than LiPo so it's important to use high quality cells otherwise you will notice strong voltage sag. Good luck with your build and show us the result!
```

---
## \#18 Posted by: JImmy2 Posted at: 2018-06-02T21:23:00.358Z Reads: 75

```
thank you so much for the help 
and of course i will post some pics when i finish it
```

---
## \#19 Posted by: rey8801 Posted at: 2018-06-02T21:27:14.123Z Reads: 77

```
My pleasure
```

---
## \#20 Posted by: rey8801 Posted at: 2018-06-02T21:32:24.660Z Reads: 79

```
To save some money check in the forum market...for instance
if you are in US http://www.electric-skateboard.builders/t/2-new-maytech-190kv-6355-motors-for-160-00-shipped-to-us/57257
EU http://www.electric-skateboard.builders/t/for-sale-2x-tb-6374-190kv-motors-sensored-eu-nl/56964
```

---
