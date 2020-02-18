# Solar panel power injection

### Replies: 2 Views: 116

## \#1 Posted by: JKFlipFlop Posted at: 2019-10-06T21:57:45.150Z Reads: 54

```
If someone wanted to connect solar panels to any type of E-board, how would you inject the power? I want my panels to supply their power to the ESC while the board is in use, and also charge the battery when the excess power is not needed.  For example, if the pack is 10S, that would mean the voltage between the battery pack and the ESC will vary from 42V charged to 30V discharged. 
Would it work, to use a diode to prevent power backfeeding into the solar panel (48V) and connect directly to the DC input lines on the ESC (in parallel with the battery pack). Keep in mind that their may be times when the voltage going to the ESC may be greater than the voltage on the panel.
Or would it work to instead use a solar panel charge controller and somehow fool it to charging a 10S pack. Another problem to consider with using a solar controller is I want the power to go to the ESC when needed as a priority, in order to be efficient as possible. It would be stupid to charge the battery for 500ms, and then 500ms later that power gets dumped to the motor. Also, I would need to come up with a strategy that would not overvoltage the BMS

Sorry, that is alot to digest
```

---
## \#2 Posted by: Nomad Posted at: 2019-10-07T00:04:42.872Z Reads: 36

```
There’s a bunch of threads on solar powered boards here. I couldn’t work out how to add a link. Sorry. Use the search function ⬆️. Good luck with your build. 🙃
```

---
