# Dual 6S vs Single 8S-12S

### Replies: 7 Views: 2096

## \#1 Posted by: NickTheDude Posted at: 2016-05-31T20:45:56.693Z Reads: 180

```
Hey I'm trying to build an electric longboard as cheaply as possible, but would like the option to upgrade in the future, so my current plan is to have 2 [3S 5000mAh 25C batteries](http://www.hobbyking.com/hobbyking/store/uh_listCategoriesAndProducts.asp?idCategory=235&LiPoConfig=3&sortlist=&CatSortOrder=desc) in series, a [6354 260kV](http://www.hobbyking.com/hobbyking/store/__18127__Turnigy_Aerodrive_SK3_6354_260kv_Brushless_Outrunner_Motor.html) motor, and [this ESC](http://www.hobbyking.com/hobbyking/store/__77144__HobbyKing_174_8482_X_Car_Beast_Series_ESC_1_8_Scale_120A.html). I will also use a 36:16 gear ratio. If my calculations are correct this should give me a top speed of around 18mph with relatively little torque.

In the future I would like to get another motor/ESC and go dual drive, at this point I think I would change the gear ratio to something like 36:20. This would raise my top speed significantly at the expense of torque, but from what I understand that loss would be easily outweighed by the gained torque from dual motors. Is this correct? Is there anything wrong with running this kind of gear ratio?

I'm trying to keep an 6S setup since ordering a VESC will cost me about 150$ and the one from hobbyking is a third of the price, on top of that I get to pay less for batteries. I figure if I can achieve a top speed of 20-25 mph with a single motor 6S setup at the sacrifice of torque, I could fix that by adding another motor and I would be able to build a dual motor 6S board for the same price if not cheaper than something using 8-12S. So I guess the question is, should I save up and go for a higher voltage build? Or will my current plan suit my needs?
```

---
## \#2 Posted by: Jinra Posted at: 2016-05-31T20:51:18.926Z Reads: 173

```
You might want to go for a lower kv 637x motor for additional torque on a single motor setup. Also, SK3's have been on backorder for a while so it may take some time to get one of those. Ollinboard's motor seems pretty promising (5065) so you can look into that, should be shipping tomorrow.
```

---
## \#3 Posted by: NickTheDude Posted at: 2016-05-31T20:59:40.134Z Reads: 172

```
The issue with longer motors is that I'm not sure if I'd be able to fit 2 64mm or 74mm motors beside each other on my 180mm paris trucks if I wanted to upgrade. However if I went with a single motor 8-12S setup then I'd definitly use something bigger.
```

---
## \#4 Posted by: Jinra Posted at: 2016-05-31T21:09:44.789Z Reads: 157

```
Yea they probably won't fit on 180mm trucks. You could try longer Paris trucks, or run them in a dual diag configuration which I'll be doing. You can also still run a dual rear setup if you have one motor in front of the rear axle and one motor behind.
```

---
## \#5 Posted by: NickTheDude Posted at: 2016-06-01T01:14:47.839Z Reads: 128

```
Ahhhh I hadn't considered using a dual diagonal setup that's a good point. If I used 2 192kV 6374 motors with 6S batteries would I still be able to get to 20mph on 83mm wheels?
```

---
## \#6 Posted by: Jinra Posted at: 2016-06-01T01:18:29.153Z Reads: 122

```
on 6s, you're looking at about 18mph at 100% efficiency. Realistically closer to 12-13mph depending on weight and environment. See below

https://toddy616.blogspot.com/2013/07/electric-skateboard-calculator.html?m=1
```

---
## \#7 Posted by: NickTheDude Posted at: 2016-06-01T01:21:59.549Z Reads: 112

```
Oh damn that's a great link, so I figure it would probably be better to stick to a high kV motor and tall gearing to get a decent top speed with low torque, then add another motor in the future when it fits the budget. Thanks!
```

---
