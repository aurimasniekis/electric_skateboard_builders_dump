# Manage VESC settings through UART

### Replies: 4 Views: 130

## \#1 Posted by: Jamie42 Posted at: 2019-07-08T11:01:43.671Z Reads: 39

```
Hi,

I want to control my VESC settings through UART. So, for example, being able to set motor max current and battery max current. 

I'm currently using [this library](https://github.com/SolidGeek/VescUart) to read telemetry, control speed and set cruise but it doesn't allow changing VESC settings. 

Anyone who can help me with this?
```

---
## \#2 Posted by: Jamie42 Posted at: 2019-07-20T18:59:40.445Z Reads: 21

```
Bump, anyone??
```

---
## \#3 Posted by: mutantbass Posted at: 2019-07-20T19:58:54.003Z Reads: 20

```
why dont you just get a nrf bluetooth module and then use the official app on android? no need to faff about opening enclosures and such.
```

---
## \#4 Posted by: Jamie42 Posted at: 2019-07-20T20:23:30.067Z Reads: 18

```
Because I want to implement different modes into my Firefly Nano remote. With different amp settings. That also means my uart port is already occupied.
```

---
