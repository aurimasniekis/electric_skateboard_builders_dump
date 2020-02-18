# \[HELP\] Can&rsquo;t get my hm-10 bluetooth to connect to the Flipsky VESC

### Replies: 2 Views: 307

## \#1 Posted by: gee Posted at: 2019-03-24T04:56:23.519Z Reads: 79

```
**READ EDIT2**

So I bought this [HM-10](https://www.aliexpress.com/item/Free-Shipping-1pc-HM-10-transparent-serial-port-Bluetooth-4-0-module-with-logic-level-translator/1910330434.html?spm=a2g0s.9042311.0.0.1d4a4c4dsyfXsn) module from AliExpress and plug it into Arduino to check the firmware. I got this **OK**
**OK+Get:0**
**HMSoft V606**. When I plug the module to the VESC and try to configure it. The **only** app that recognize the HM-10 module is EleSk8 on iOS (I've bough any apps since I don't even know if it works). 

![IMG_2437|281x499](upload://gOVEgjxBeHn0kYit7IJKQyQFZf0.png) 

I don't understand how this app can detect the module but can't get it too work. I've set the baud rate on VESC TOOL to 9600 bps and PPM and UART, it still wouldn't run. 
![IMG_2438|281x499](upload://aRV02deEkcEt3U8j2n5W8HIR8bR.png) 

Prove that it connects.

![IMG_2439|375x500](upload://6RTHoVFFI0g26j01IhTQFS8LehN.jpeg) 

Try to plug it in Arduino and confirm the firmware and baud rate. The **DI0,0,90.0** is when it connects to the EleSk8 app and when I throttle it through the app, the Arduino can detect the signal. But somehow the VESC doesn't. 
YES I've tried to switch the RX and TX around and it still didn't work. **CAN SOMEONE PLEASE HELP**.

EDIT: additional info
![Screenshot%20(148)|690x459](upload://2zmT6z5RBzQ3j4qcQOpctRlyHjA.png) ![Screenshot%20(149)|690x459](upload://8PVj7rvXdCySiN653RZVYguHGfY.png) 

BAUD rate set to 9600 and PPM and UART select

**EDIT2**: So I read up that the iPhone bluetooth setting page can't detect the HM-10 due to some hardware reason that explain why I was trying to find it and no success. I installed a bunch of free electric skateboard app but none of them works except the EleSk8 Remote, but it doesn't actually turn the motor. So all these time I tried to get these free apps to recognize my HM-10 but upon a lot of reading I found out most of them if not all of them use different bluetooth modules. So I decided to buy Xmatic app on a whim hoping it would work and it did. Recognize it instantly. THANKS THE ESK8 community for the help...
```

---
## \#2 Posted by: cherryflavouredpez Posted at: 2019-05-03T23:08:52.508Z Reads: 38

```
which version flipsky do you have? I have the FSESC 6.6 dual, and want to get bluetooth on IOS too
```

---
