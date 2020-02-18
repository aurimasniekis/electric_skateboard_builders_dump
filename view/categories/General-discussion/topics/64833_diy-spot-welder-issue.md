# Diy spot welder issue

### Replies: 14 Views: 573

## \#1 Posted by: Becker33 Posted at: 2018-08-14T13:04:36.191Z Reads: 116

```
Built a spot welder to avoid the cost of buying one but it won’t work. It makes a sound when the button is pressed and the wood burns underneath but no weld. The battery is second hand and was very cheap.
![image|375x500](upload://pDBVimqEBejjrKjFiDOX14ALnNX.jpeg)

Any help would be amazing
```

---
## \#2 Posted by: sztamas Posted at: 2018-08-14T13:31:48.239Z Reads: 108

```
It is hard to weld nickel to nickel.
What is the material of the electordes? It should be copper. And the contact points should be small. If the contact points are too big, the current has more diameter to pass through the material, and the momentary heat will not be sufficient.
```

---
## \#3 Posted by: Quezacotl Posted at: 2018-08-14T13:55:46.423Z Reads: 104

```
The key thing here is that you have second hand cheap battery, which is propably not good enough.
You need about 400A current minimum(that i recall). More is better.
```

---
## \#4 Posted by: cryo Posted at: 2018-08-14T19:45:19.415Z Reads: 84

```
@darkkevind uses a 200A battery with no problems in one of his vids
```

---
## \#5 Posted by: Becker33 Posted at: 2018-08-15T07:02:01.373Z Reads: 72

```
The electrodes are made out of brass. Thanks for the help, I will try with another battery today.
```

---
## \#6 Posted by: darkkevind Posted at: 2018-08-15T10:54:32.253Z Reads: 59

```
Your electrodes should be copper. I link to some copper roofing nails in one of my videos on YouTube.
The guage of your main wire might want to be a little heavier. I've found that jumper cable is not adequate.
Be sure to make sure both electrodes are seated on your nickel before clicking your button.
Make sure you literally just press your button for a split second, otherwise it's too much time and you could blow a hole in your nickel or battery.
```

---
## \#7 Posted by: Becker33 Posted at: 2018-08-17T15:44:25.489Z Reads: 35

```
so I have tried a new battery and it works... ish. It now blows a hole straight through the nickel strip. I have cobbled together a arduino relay with a spare nano I had but am now having troubles making the code work.
```

---
## \#8 Posted by: Becker33 Posted at: 2018-08-17T15:46:13.808Z Reads: 35

```
![image|374x500](upload://zpgtGnEJmRXPsLHp2FP5SkQITsh.jpeg)
```

---
## \#9 Posted by: legend27 Posted at: 2018-08-17T16:03:31.380Z Reads: 31

```
Set the pulse time in the arduino lower. Pretty sure @rey8801 has a code he might want to share?
```

---
## \#10 Posted by: rey8801 Posted at: 2018-08-17T16:06:37.497Z Reads: 31

```
Sure as long you won't laugh about how simple it is :joy: I learnt in a couple of ours from YouTube the basic to adapt the preset led script available in Arduino IDE to my purpose. Wait that I look for it
```

---
## \#11 Posted by: rey8801 Posted at: 2018-08-17T16:11:00.212Z Reads: 30

```
void setup() {
 
  pinMode (LED_BUILTIN, OUTPUT);
  pinMode(2, INPUT);
  
}

void loop() {
// the loop function runs over and over again forever void loop() {
    digitalWrite(LED_BUILTIN, LOW);
  if (not digitalRead(2)){
    //pulse 1
    digitalWrite(LED_BUILTIN, HIGH);
    delay(**50)**;
    digitalWrite(LED_BUILTIN, LOW);
    //delay
    delay(450);
    //pulse 2
    digitalWrite(LED_BUILTIN, HIGH);
    delay(**100**);
   digitalWrite(LED_BUILTIN, LOW);
    delay(2000);
    }
 
}

https://www.dropbox.com/s/fgwdmxmynzobqbh/sketch_spot_welder.ino?dl=0

Bold numbers are the stimuli duration. So if you read from the top you have the first stimulus of 50 msec, then 450 msec delay, second stimulus of 100 msec and 2 sec delay to prevent that the cycle start again. So you will need to press the button again to run it. 
I used double stimuli because I read of a lot of spot welder that works like that, the first stimulus heats up the nickel strips enough to get a perfect contact with the underneath surface and then the second one welds. So you will need to change those two value based on your system power. I would say start to modify the second, the first one is to get the good contact. Ah and press firmly the tips welding tips against the nickel strips and battery.
```

---
## \#12 Posted by: Becker33 Posted at: 2018-08-17T16:40:49.044Z Reads: 26

```
Here is the code I have been using but without much success yet, I can’t see anything wrong with it though.

const uint8_t BUTTON_PIN = 2;
const uint8_t RELAY_PIN = 3;
const uint8_t LED_PIN = 4;
 
void setup() {
    pinMode(BUTTON_PIN, INPUT_PULLUP);
    pinMode(RELAY_PIN, OUTPUT);
    pinMode(LED_PIN, OUTPUT);
    digitalWrite(RELAY_PIN, HIGH);
}
 
void loop() {
    if (digitalRead(BUTTON_PIN) == LOW) {      // button pressed
        digitalWrite(RELAY_PIN, LOW);        // RELAY on
        digitalWrite(LED_PIN, HIGH);           //LED on
        delay(20);                            // wait
        digitalWrite(RELAY_PIN, HIGH);        // RELAY off
        digitalWrite(LED_PIN, LOW);           // LED off
    }
}
```

---
## \#13 Posted by: rey8801 Posted at: 2018-08-17T16:48:08.971Z Reads: 22

```
yeh I am not expert in coding, sorry. Anyhow use a nickel strips and a cutter blade to simulate the battery metal part. On the related forum they suggest it as a good way to simulate the real situation with battery. The secret is to deliver a lot of current in really short time, so you have to be sure that your battery can delivery it.
```

---
## \#14 Posted by: Becker33 Posted at: 2018-08-17T16:49:31.817Z Reads: 20

```
Thank you for your help, I’ll try your code! I think I’ve fried my solenoid so I can practice my coding until the new one arrives :joy:
```

---
