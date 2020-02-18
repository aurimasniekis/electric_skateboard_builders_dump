# eSk8 app UI help wanted

### Replies: 15 Views: 591

## \#1 Posted by: Esrapp21 Posted at: 2017-08-18T00:40:30.018Z Reads: 66

```
Hi everyone. This thread is a bit off topic from normal, but I figured I could try here because of all the great eSk8 apps. I’m currently working on an eSk8 analytics app (more info to come), and while I’m ok with the backend, I can’t deal with the UI for iOS. I was wondering if anyone had any experience with this. Please message me if you do, and I’ll explain a bit more of what needs to be done.
```

---
## \#2 Posted by: saul Posted at: 2017-08-18T03:17:56.576Z Reads: 59

```
lol ios ui designer is why i learned android :joy:
let me know when you get there
```

---
## \#3 Posted by: Esrapp21 Posted at: 2017-08-18T03:22:40.298Z Reads: 56

```
Believe me, iOS UI is hell on earth
```

---
## \#4 Posted by: saul Posted at: 2017-08-18T03:26:52.999Z Reads: 51

```
lol i'm sure.

i'm hoping the new android lang gets an ios export option so i never have to to back into that horrible thing....
```

---
## \#5 Posted by: catweazle Posted at: 2017-08-18T10:36:57.765Z Reads: 36

```
What about ionic framework. Could that be helpful ?
```

---
## \#6 Posted by: karma Posted at: 2017-08-18T11:02:27.131Z Reads: 30

```
I would recommend using React Native, facebooks java script framework for developing native applications for iOS and Android. You write in java script for both platforms at the same time.
```

---
## \#7 Posted by: Esrapp21 Posted at: 2017-08-18T11:26:54.225Z Reads: 32

```
The main issue I have is graphs. There I can’t find any frameworks or api for them. There are plenty for charts, but what I really need is a program where you put in a math equation, like y =ax^2 + bx + c or 
y = a log(b x) + c.
```

---
## \#8 Posted by: darkkevind Posted at: 2017-08-18T11:55:13.092Z Reads: 27

```
You should look in to Xmarin. One code set, multiple cross platform deployments... no hassle.
```

---
## \#9 Posted by: Bataleon Posted at: 2017-08-18T12:13:34.185Z Reads: 22

```
I agree with @karma, [React Native](https://facebook.github.io/react-native/) is fantastic. We have been using it at work for the last 11 months in combination with the [Victory Native](https://github.com/FormidableLabs/victory-native) charting package.

Apps are written in Javascript, which outputs 100% native (no `WebViews`, like Phonegap) iOS and Android apps from the same codebase.

You can give it a try [here](https://snack.expo.io/). Shout if you have any questions, I'd be happy to help.
```

---
## \#10 Posted by: Esrapp21 Posted at: 2017-08-18T12:18:59.602Z Reads: 20

```
Can the c# by any chance be used side by side with swift? It would be great to use C# for UI, but the backend is already half written in swift.
```

---
## \#11 Posted by: darkkevind Posted at: 2017-08-18T12:20:15.457Z Reads: 21

```
https://stackoverflow.com/questions/41821144/how-to-use-swift-in-xamarin-ios

https://stackoverflow.com/questions/37404386/using-swift-library-in-xamarin
```

---
## \#12 Posted by: Esrapp21 Posted at: 2017-08-18T12:22:39.019Z Reads: 19

```
I actually haven’t worked much with JavaScript in the last few years and I don’t think I’m very fluent. My main issue at the moment is the graphing, and I am primarily targeting iOS right now. I may make an android release in time, but for now I’m mainly just focusing on iOS.
```

---
## \#13 Posted by: Esrapp21 Posted at: 2017-08-18T12:25:20.950Z Reads: 19

```
Awesome, one more question. Can I use it on my pc or do I have to use my Mac desktop? One of my least favorite things about Xcode is it isn’t available on Windows.
```

---
## \#14 Posted by: darkkevind Posted at: 2017-08-18T12:25:47.063Z Reads: 19

```
You should look at d3.js for graphing etc.
```

---
## \#15 Posted by: darkkevind Posted at: 2017-08-18T12:26:32.178Z Reads: 19

```
PC definitely! A Mac is a toy computer, why on earth would you want to try and develop on a toy computer!? :confused:
```

---
