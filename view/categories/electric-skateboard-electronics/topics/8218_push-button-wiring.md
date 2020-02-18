# Push button wiring

### Replies: 2 Views: 492

## \#1 Posted by: ambrojohn Posted at: 2016-08-24T02:49:56.877Z Reads: 92

```
Hi
Initializing the TX_SDA pin of the VESC with

`palSetPadMode(HW_UART_TX_PORT, HW_UART_TX_PIN, PAL_MODE_INPUT_PULLDOWN);`

and checking it at runtime with:

`palReadPad(HW_UART_TX_PORT, HW_UART_TX_PIN)`

(as per http://vedder.se/2015/08/vesc-writing-custom-applications/)

What is the wiring for a push button and a resistor that I need to make?

I cannot make it work following the example (I can only read the potentiomenter value)...the push button reading is totally inconsistent/random.

Much appreciated!
```

---
## \#2 Posted by: ambrojohn Posted at: 2016-08-24T18:13:04.925Z Reads: 43

```
My mistake. First time I stupidly messed up with the wires connections.

But yes, the pulldown configuration of the TX pin makes my push button work the opposite way, i.e. pushed when it's not and viceversa. I will try to configure it as pullup(?) or not configure it at all if, as you said, it works as well.

At this point, I would need a very simple **bluetooth system** to eliminate the wires in interfacing 2 push buttons to the VESC.

Any ideas/hints would be greatly appreciated.

Thanks!
```

---
