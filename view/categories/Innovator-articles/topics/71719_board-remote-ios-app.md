# Board Remote ios app

### Replies: 4 Views: 566

## \#1 Posted by: ArtSp Posted at: 2018-10-19T14:06:28.770Z Reads: 111

```
Hello guys,
throw away your remotes and check out my new project!
    
https://itunes.apple.com/lv/app/board-remote/id1435062075?mt=8

App requires Arduino or Raspberry Pi board with Bluetooth Low Energy support.

Raspberry/Arduino will send PWM signal to your VESC and will communicate with iOS app.

Maybe it will be a bit difficult to program IoT device if you have no experience in programming, but app contains a working example written with NodeJs, just follow the tutorial (available in the app) and you will be good to go.
Arduino example will become available in future versions.
    
You can contact me here or from the app it self (from tutorial section) if you have any questions.
Hope you will enjoy it.
    
If you have any ideas about what can be added to the app, just let me know, I'll do my best.
    
Here is a video link:
https://www.youtube.com/watch?time_continue=22&v=_Gl4KU6JcQk

PS: Always use guided access guard, it may save your life one day =)
```

---
## \#2 Posted by: Jc06505n Posted at: 2018-10-19T14:12:02.138Z Reads: 97

```
Awesome! While I personally wouldn't use it since I'm lazy and Would never risk a $1000 phone , I can see this being used as a emergency case where your remote dies and you have a cheap android phone for programming purposes. You would just need to put the necessary receiver components on the Slave vesc (Looking into password locking the Arduino/PI should be done so that not anyone can control your board.
```

---
## \#4 Posted by: Kal-El_basically Posted at: 2018-11-05T23:17:29.482Z Reads: 52

```
I'm so glad I found this, but I want to ask a few questions before I get my hopes up. I am using an arduino right now for my project, how does the wiring go in order for the app to connect. Right now I have the HM-10 BLE module TX>Arduino RX, HM-10 RX>Arduino TX, HM-10 VCC>Arduino 3.3V, and Gnd to Gnd. Then I have the arduino connected TX to RX and RX to TX on the VESC UART port. The only problem is that the app isn't picking up the arduino. I have a Raspberry Pi available but I'm not familiar with the programming or hardware of them.
```

---
## \#5 Posted by: Paulycnotes Posted at: 2019-09-14T22:20:12.552Z Reads: 14

```
Can you or someone please explain to me what is this Arduino which I keep hearing about??
```

---
