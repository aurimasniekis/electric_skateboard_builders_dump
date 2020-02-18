# VESC build from Github

### Replies: 7 Views: 1545

## \#1 Posted by: Weberp7593 Posted at: 2016-09-10T08:29:45.639Z Reads: 113

```
Hello Guys,
Firstly I want to introduce my self a little bit.
I am German, maybe you already noticed that :smiley: 

Now to the Project,
I want to build some VESCs with the information on Github! (Only want to build one, but i think it will be better to do more and maybe sell Oder sth)
But...I don't have any experience with it.
That's the bad point.

And another, but...
I have a lot of experience in electronics 
I learned it, I also make a second traineeship about it.
I have a LOT of equipment to work with!
-SMD Placing machine (Paraquda)
-SMD soldering paste printer 
-SMD Solder Oven
-Soldering irons normal and SMD
-And a lot of components 
-STM Programming Debuggers 
-STM controllers 8/32.......etc.

I also have good contacts where I can cheap circuits boards.

But I never orderd them with files like on Github (Gerber)...

So in that point I need help...
What would the first thing I should do?
Send the gerbers to my supplier?
And which one? There are so many files...


Would be really happy if somebody could help me...
Best regards!
```

---
## \#2 Posted by: JTAG Posted at: 2016-09-10T08:34:15.304Z Reads: 105

```
Just send a zipfile with all the gerbers you find to the fab, there is even a zip already in the repo if I am correct. The PCB fab will tell wether it is ok or not. And don't cheap out on PCB's, it is the core and body of the whole VESC.
```

---
## \#3 Posted by: lox897 Posted at: 2016-09-10T08:36:52.926Z Reads: 107

```
For the components:

Download this: https://github.com/vedderb/bldc-hardware/blob/master/design/BLDC4.12_BOM.ods

Use an online converter to convert it to xlsx such as this one: http://www.zamzar.com/convert/ods-to-xlsx/

Upload it into Mouser and walk through the setup. It will then give you a list of components. http://www.mouser.com/bomtool/

For the pcb:
https://oshpark.com/shared_projects/y0ye8b2o
Or just download the gerber files and upload the files that they ask (such as mask, silkscreen etc)

Hope this helps
```

---
## \#4 Posted by: Weberp7593 Posted at: 2016-09-10T08:40:18.948Z Reads: 95

```
Thanks :) sry I said that not right...
I mean i get them in very very good quality but cheap because I do all my orders (about 6000pcs/yr) there.

Ok thanks! So I will first send them the zip and will wait what they say.

<img src="/uploads/db1493/original/3X/8/2/824f998b1ae57ea81f3bf80805df015bb745171e.jpeg" width="450" height="500">

(You mean the last zip file is including all they need?)
```

---
## \#5 Posted by: susplus Posted at: 2016-09-10T08:45:06.284Z Reads: 72

```
i wanted to recommend you Danny :)) but you are to fast :slight_smile:
```

---
## \#6 Posted by: Weberp7593 Posted at: 2016-09-10T08:47:09.838Z Reads: 71

```
Haha :slight_smile:, 
And @lox897 all information, will help me.
Because I never done sth like that before.
Tanks!
```

---
## \#7 Posted by: JTAG Posted at: 2016-09-10T08:53:07.369Z Reads: 72

```
Haha thanks :p.

Yeah the bottom zip it is.

You order that many pcbs but never from gerber file? What other files do you send then? Eagle files?
```

---
