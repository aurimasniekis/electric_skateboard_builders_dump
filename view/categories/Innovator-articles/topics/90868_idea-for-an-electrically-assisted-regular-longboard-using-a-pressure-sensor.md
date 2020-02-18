# Idea for an electrically assisted &ldquo;regular&rdquo; longboard using a pressure sensor

### Replies: 10 Views: 433

## \#1 Posted by: rusins Posted at: 2019-04-17T14:05:36.233Z Reads: 104

```
Maybe someone has thought of this before me (would love to see a working version if so), but here's my idea:

Remote-less electric boards are a thing, but the only ones I've seen are the type that gradually become slower and slower until you have to push again. My idea is to use a pressure sensor (similar to the one on Onewheels) at the back of the board to detect when you have your back foot on. If your back foot is on, the board will maintain your current speed using a battery and motor as usual, but if your foot is off, it will go into free-roll mode. This way, the board goes only as fast as you push, but you don't have to keep pushing constantly to maintain your speed, and breaking works just like on a regular board.

I could see something like this being a direct replacement to usual free-ride longboards. Disadvantages are the usual of course: no regenerative breaking, no going faster than cars (unless you have super-human pushing strength :stuck_out_tongue: )

Would it be possible to make something like this by simply reprogramming a VESC? 
What do you guys think?
```

---
## \#2 Posted by: Andy87 Posted at: 2019-04-17T14:11:20.823Z Reads: 97

```
There is one prebuilt which works like that. I forgot the name. Need to google it...
```

---
## \#3 Posted by: Andy87 Posted at: 2019-04-17T14:13:07.399Z Reads: 97

```
Don’t blame me for that link...you asked about it 😂
https://starkmobility.com/products/starkboard


Not sure if that would be easy to implement on a vesc thou.
```

---
## \#4 Posted by: rusins Posted at: 2019-04-17T14:13:55.211Z Reads: 93

```
Oh, is this the one Braille Skateboarding did a video on? It seemed like a death-trap :smiley:

Edit: Yes, it is
```

---
## \#5 Posted by: Andy87 Posted at: 2019-04-17T14:15:19.282Z Reads: 91

```
I have no clue about it. Just know it exists. If working well or not 💁‍♂️😂
```

---
## \#6 Posted by: rusins Posted at: 2019-04-17T14:16:04.100Z Reads: 91

```
Yes, well, it's a similar concept, but my idea relies on the pressure sensor just as an on/off switch :)
```

---
## \#7 Posted by: ZachTetra Posted at: 2019-04-17T14:31:05.889Z Reads: 84

```
You could do it with a raspberry pi or Arduino...read the speed values off the VESC via UART and implement a PID loop to maintain that speed while a transducer reads some positive voltage by generating a PWM value to feed the VESC receiver channel...and drop the signal to a neutral if the transducer reads zero

That mod would cost about the same as a remote
```

---
## \#8 Posted by: rusins Posted at: 2019-04-17T14:57:36.803Z Reads: 71

```
Hmm, a negative feedback loop from an arduino could really work now that I think about it. Thanks!

Hopefully Swissboards release their reverse kingpin direct drive sometime soon, because I'd want the free-roll to be as good as possible.
```

---
## \#9 Posted by: rusins Posted at: 2019-04-17T15:00:16.017Z Reads: 72

```
Hmm, if the system works reliably enough, I could even add a pressure sensor at the front that would make the board brake in case the rider jumps off in case of an emergency. I can't count how many times I've had my board fly away from me because I was messing around ;P
```

---
## \#10 Posted by: chaiseboard Posted at: 2019-11-06T01:37:06.106Z Reads: 19

```
Hi rusins!

I have made a prototype of a pressure sensored electric longboard using the FSR 406 pressure sensor and controlled the esc with a PIC18F4520 microcontroller. But i am curently developping a new version where i will be using an arduino with a PID regulation because the first prototype is not smooth enough. In my plans for the new proto i think i gonna use the velostat pressure material by 3M.

Do not hesitate if you have any questions.
```

---
