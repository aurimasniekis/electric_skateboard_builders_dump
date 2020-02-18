# Bluetooth development guide

### Replies: 9 Views: 548

## \#1 Posted by: Acklavidian Posted at: 2018-05-24T12:19:01.069Z Reads: 127

```
I was considering making a JavaScript app for vesc configuration and monitoring over Bluetooth. I don't have much experience with bluetooth/serial interfaces. However I have successfully connected to the vesc but I don't know what instructions I can send. Where could I find this documentation?
```

---
## \#2 Posted by: egzplicit Posted at: 2018-05-24T12:42:10.441Z Reads: 116

```
What platform?
```

---
## \#3 Posted by: Acklavidian Posted at: 2018-05-24T13:06:55.758Z Reads: 107

```
I guess I would start off by aiming for browser. Then explore node and nativescript if that didn't work out.
```

---
## \#4 Posted by: Acklavidian Posted at: 2018-05-24T16:20:00.319Z Reads: 86

```
It seems that some people may not be taking me seriously as they think my assumption that Bluetooth from a browser means is idiotic and is reflective of my lacking in ability. So it may come as a surprise to some developers but the browser is capable of a Bluetooth connection. However, I can't say for sure if it's as sophisticated as we might need. Nodejs has libraries for Bluetooth connection as well so that was my second choice. Also Nativescript has some tools Bluetooth as well but also some swift/java/objective c bindings could be used. However I would say that I would prefer desktop access. 
Potential tools/technologies:
* https://webbluetoothcg.github.io/web-bluetooth/#device-discovery
* https://github.com/song940/node-bluetooth/blob/master/README.md
* https://github.com/charto/nbind
* https://nodejs.org/api/addons.html
```

---
## \#5 Posted by: Acklavidian Posted at: 2018-05-24T16:27:51.155Z Reads: 76

```
My goal would be to create a tool that:
 1. Works for me over Bluetooth. As right now neither desktop app works over Bluetooth. And I have the latest Android which seems to break alot of the mobile apps available for the Android platform. 
2. Create an app with a more maintainable code base via expanding it's developer accessibility through easier technologies like JavaScript and reduce duplication of efforts by using code once run anywhere tech. Eg. No more desktop/mobile split.
```

---
## \#6 Posted by: Acklavidian Posted at: 2018-05-24T16:28:48.289Z Reads: 76

```
@Ackmaniac any insight would be greatly appreciated.
```

---
## \#7 Posted by: Mathias Posted at: 2018-05-24T17:38:22.129Z Reads: 71

```
The VESC tool itself works via Bluetooth. 
https://vesc-project.com/node/234
I'm already using nrf to connect VESC tool to both my FOCboxes (it can connect to the other controllers via CAN) from both my laptop and my phone. Works like a charm. It's available on Benjamins github: 
https://github.com/vedderb/nrf51_vesc
What it still misses is switching between configuration modes, and a decent realtime data display. But the job you're describing is already 95% done.
```

---
## \#8 Posted by: cryo Posted at: 2018-05-24T19:00:34.441Z Reads: 58

```
The vesc communicates through UART interface. 

Have a look at this for what commands to send:
https://github.com/vedderb/bldc/blob/master/commands.c
```

---
## \#9 Posted by: lock Posted at: 2018-05-25T02:44:40.770Z Reads: 42

```
[quote="Acklavidian, post:4, topic:56591"]
It seems that some people may not be taking me seriously as they think my assumption that Bluetooth from a browser means is idiotic and is reflective of my lacking in ability.
[/quote]

Noooo, surely not :grimacing::wink: . Ok on first reading kinda yes, but then I remembered browsers have access to pretty much everything else (mic, camera, accelerometer, GPS) these days so it sounded entirely plausible.

Web-bluetooth support seems limited to Bluetooth LE which is fine, but it also seems somewhat [restricted to Chrome](https://caniuse.com/#feat=web-bluetooth). Not great, but Chrome has decent market share these days. Knowing Apple, I'm not sure you could ever expect to see support implemented in mobile Safari.

The link that cryo posted includes the implementation/definition of the 'higher level' (payload) VESC communication protocol. It's important to note this may change in any firmware update. The lower level is described in [one of Vedder's blog posts](http://vedder.se/2015/10/communicating-with-the-vesc-using-uart/). It's quite elegant in its simplicity.

> - One Start byte (value 2 for short packets and 3 for long packets)
> - One or two bytes specifying the packet length
> - The payload of the packet
> - Two bytes with a CRC checksum on the payload
> - One stop byte (value 3)

I don't think you need justification for doing this; if you want to do it, then do it :+1: . But I can see several  advantages in addition to what you've already listed.

- Given the choice between a browser based tool, and a desktop tool, I'd probably go for the browser these days. Mainly just convenience.
- If you reimplemented (not port, proper cleanroom implementation) the VESC communication protocol you'd probably be ok to release it under a less restrictive license (MIT, etc).
- Could be good for a remote support tool. I understand Enertion diagnose problems via a remote desktop tool (urgh).
```

---
