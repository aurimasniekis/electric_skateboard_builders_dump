# Everything blew up

### Replies: 11 Views: 457

## \#1 Posted by: xatonic Posted at: 2019-06-19T00:39:29.860Z Reads: 218

```
Hey guys! Sad post here, so I've been heavily been working on my board to get it working before school gets out (tomorrow) I had finished everything and all I was doing was troubleshooting my Firefly remote system because it wasn't binding so I pulled out my laptop set it next to the board and then I must have moved something? And a big spark came out of my loop key while it was already in. That scared the sh*t out of me so I unplugged everything and started to look through everything, one of the receiver wires got disconnected at the solder join, and there was black sut on the uart ground pin area of the foc box. Now the receiver screen won't turn on even when I plug it in to my laptop and I can't connect with the focbox, there's not even a light when the power is connected although it is outputting power on other pins in the uart other than the 3.3v![IMG_20190618_175503|236x500](upload://ArIkKgNSw98HCCK8Df97jvTQZnd.jpeg) ![IMG_20190618_175452|236x500](upload://bmyxAmBSvkXqmDQMDNYDkSXFs8u.jpeg) ![IMG_20190618_175433|236x500](upload://4uVcvY3GCxe5GO1ksHR8vMySP4P.jpeg) ![IMG_20190618_175413|236x500](upload://jpbKrSbP2lDKpmkFD6zCnFyJAL.jpeg)
```

---
## \#2 Posted by: AgressivStreetLamp Posted at: 2019-06-19T00:52:09.595Z Reads: 192

```
Gonna need pictures and mazbe post on https://forum./
```

---
## \#3 Posted by: xatonic Posted at: 2019-06-19T01:17:43.683Z Reads: 179

```
Just did both😃
```

---
## \#4 Posted by: xatonic Posted at: 2019-06-19T02:12:30.093Z Reads: 172

```
I believe I have found the issue with closer inspection I've found sut on the receiver's antenna
![15609100003333557079810933123309|236x500](upload://8Nx3DEk7bR7lFwZAeEDMLMQ4HVQ.jpeg) and during the receiver troubleshooting I had pulled it out to see if it would get better reception and when I moved around a bit the base of the antenna made contact with the positive loop key and created a surge through the receiver up through the ground wire (had been unsoldered and the clear heatshrink was black with sut) and into the board where the final amount of sut has been found. So my question is is the focbox recoverable? @JohnnyMeduse
```

---
## \#5 Posted by: JohnnyMeduse Posted at: 2019-06-19T02:56:13.237Z Reads: 135

```
Focbox should be fine. Best way to know is to open it and check it.
```

---
## \#6 Posted by: xatonic Posted at: 2019-06-19T03:08:01.995Z Reads: 134

```
Everything is physically ok from observation inside but I only have .4 volts out of the 3.3v pin and I can't connect it to the computer
```

---
## \#7 Posted by: JohnnyMeduse Posted at: 2019-06-19T03:36:06.774Z Reads: 128

```
There is probably some that as blown on the 3.3V circuit, but it should be salvageable. 

My guess are:
MCU, Can Transceiver or 3.3V regulator.
```

---
## \#8 Posted by: xatonic Posted at: 2019-06-19T03:39:29.055Z Reads: 124

```
So I sent you a message through your website, this repair is way over my head😂, what's your average turnaround time btw?
```

---
## \#9 Posted by: Richcan Posted at: 2019-06-19T22:57:56.214Z Reads: 77

```
When connecting all these wires is there not a fuse that needs to be installed?
```

---
## \#10 Posted by: xatonic Posted at: 2019-06-20T00:04:19.619Z Reads: 66

```
It's all one system so I would need a 60a fuse which wouldn't do anything in this case because you normally don't fuse your receiver but I am planning on it in the future
```

---
## \#11 Posted by: JohnnyMeduse Posted at: 2019-06-20T00:14:50.981Z Reads: 60

```
Check your email

but usually 2-3 days
```

---
