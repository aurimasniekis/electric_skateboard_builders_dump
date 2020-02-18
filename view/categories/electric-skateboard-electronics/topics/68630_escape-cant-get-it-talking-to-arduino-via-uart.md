# ESCape: Can&rsquo;t get it talking to Arduino via UART

### Replies: 9 Views: 366

## \#1 Posted by: janpom Posted at: 2018-09-20T10:05:09.624Z Reads: 99

```
I'm struggling getting the Arduino talk to my ESCape. Here's my setup:

- Two ESCapes connected via CANBUS and powered off 12s battery.
- VESC Tool config:
  - PPM and UART
  - 115200 UART baud rate
- pin out
  ESCAPE - Arduino
  5V - Vin
  GND - GND
  TX - RX
  RX - TX

I tried to narrow down the problem as much as possible. Here's the code I'm using:
https://gist.github.com/janpom/d63029bfb47ff34a6d7833eda9d52731

Code dependencies are minimal -- only [datatypes.h](https://github.com/vedderb/bldc_uart_comm_stm32f4_discovery/blob/master/datatypes.h) [crc.h](https://github.com/vedderb/bldc_uart_comm_stm32f4_discovery/blob/master/crc.h) from Vedders UART library.

The send_packet function I copied and slightly modified from [ESP8266VESC lib](https://github.com/bastianraschke/ESP8266VESC/blob/master/ESP8266VESC.cpp#L278).

Then I merely count the received bytes and indicate the status using the Arduino's builtin LED. If at least one byte is received, there should be one long blink. Otherwise, there are three short blinks.

The RX/TX LEDs on the Arduino do not blink at all, so I suppose this is a HW problem rather? I have read through the discussion [here](https://www.electric-skateboard.builders/t/hw6-4-based-esc-escape/37579/890?u=janpom), but it didn't help me.

As I understood, the TX/RX on the ESCape is 3.3V and thus it may be necessary to use a voltage divider for the RX. On the other hand, @stewii said that "most IO pins on the STM are 5V tolerant" so the voltage divider is not necessary.

Here's a quick vid showing how things are wired up and how LEDs blink (or not):
https://www.youtube.com/watch?v=-gwqe_cFzsw

Any help, please?

@stewii @Pimousse @Manu39

Update: It apparently takes writing a long post for one to figure out the problem himself. I'm not updating the `count` variable in my [`received_bytes_count`](https://gist.github.com/janpom/d63029bfb47ff34a6d7833eda9d52731#file-vesc_uart_test-ino-L85) function. :scream:

After fixing that bug, I'm getting long LED blinks now. Looks like I'm getting somewhere.
```

---
## \#2 Posted by: Pimousse Posted at: 2018-09-20T10:21:16.372Z Reads: 88

```
Hi !
[quote="janpom, post:1, topic:68630"]
The RX/TX LEDs on the Arduino do not blink at all, so I suppose this is a HW problem rather? I have read through the discussion [here](https://www.electric-skateboard.builders/t/hw6-4-based-esc-escape/37579/890?u=janpom), but it didn’t help me.
[/quote]
We solved this issue by removing the voltage divider. As @stewii mentioned, STM32 pins are 5V tolerant.

What FW are you using on your ESCape ?
```

---
## \#3 Posted by: janpom Posted at: 2018-09-20T10:31:22.129Z Reads: 87

```
Hi @Pimousse, thanks for chiming in. I believe I have the latest FW on my ESCape. I updated it this week.

As I already mentioned in the update, I have probably figured out the problem. I had a bug in my code so it was reporting the communication status incorrectly.

It's a bit strange since I've been struggling to get the UART communication working for a few hours, using both the [ESP8266VESC](https://github.com/bastianraschke/ESP8266VESC/) and [VescUartControl](https://github.com/RollingGecko/VescUartControl) libraries with no luck. So I've been stripping my code sample off as many dependencies as possible to make sure there's no bug in those libraries. It finally seems to be working now. I still don't know what I have been doing wrong all the time.
```

---
## \#4 Posted by: Pimousse Posted at: 2018-09-20T10:57:49.966Z Reads: 77

```
Make sure of the FW version.
Since 3.40, packet length of COMM_GET_VALUES exceeds Arduino buffer size.
There is a workaround which consists into increasing Arduino bufer size, but it s a bit tricky.
@solidgeek wrote a custom library to get rid of this limitation. ;)
```

---
## \#5 Posted by: janpom Posted at: 2018-09-20T11:48:00.765Z Reads: 70

```
Good to know. Thanks. Looking at it now. Vedder has [added controller ID](https://github.com/vedderb/bldc/commit/43c3bbaf91f5052a35b75c2ff17b5fe99fad94d1#diff-1d1d8abd942693caea3af1832df0ef4c) to the message. And yes, I do have FW 3.40. That explains why I had no luck getting the VESC data using the [ESP8266VESC](https://github.com/bastianraschke/ESP8266VESC/) and [VescUartControl](https://github.com/RollingGecko/VescUartControl) libs. I should be able to figure it out now. This is super helpful. Thanks a lot.
```

---
## \#6 Posted by: Pimousse Posted at: 2018-09-20T12:01:00.658Z Reads: 66

```
I opened an issue on Vedder's Github for it.
You can follow how it is going : https://github.com/vedderb/bldc/issues/63
```

---
## \#7 Posted by: janpom Posted at: 2018-10-29T22:01:07.169Z Reads: 39

```
@Pimousse Just FYI, I ended up creating my own minimalistic lib for reading data from VESC. It doesn't require messing up with the Arduino buffer size and it still works with the VESC FW v3.40. I simply ignore the last received byte, which is the termination byte. https://github.com/janpom/davega/blob/master/vesc_comm.cpp
```

---
## \#8 Posted by: Pimousse Posted at: 2018-10-29T22:15:38.391Z Reads: 33

```
Thank you !
However, I think it can't work although you don't CRC check the payload.
Moreover, this is not sustainable if in a near future, more datas are added.
@solidgeek 's library seems to work with 3.40.
I didn't tested it yet, I'm adding more stuff to it like FW checking.

Maybe you coule have a look at it ;)
```

---
## \#9 Posted by: janpom Posted at: 2018-10-29T22:45:23.880Z Reads: 29

```
[quote="Pimousse, post:8, topic:68630"]
However, I think it can’t work although you don’t CRC check the payload.
[/quote]

What do you mean? I do [CRC check the payload](https://github.com/janpom/davega/blob/master/vesc_comm.cpp#L146). We'll see regarding sustainability. Maybe Vedder does something about it following your issue.

I had a quick look at [@solidgeek's library](https://github.com/SolidGeek/VescUart/). It seems to be doing the same trick = it just doesn't check the termination byte. So I believe it has the same sustainability problem as my lib.

My version is more memory efficient since it parses data from the received packet on demand and thus it doesn't need a `struct` to copy all the parsed data into. It also has less features though. Only reading from VESC. There's no writing into VESC.
```

---
