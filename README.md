# SID-Synthesizer
A simple SID ADSR Synthesizer

This will let you create an instrument or sound that you can export into another program to play, although I've also included a basic keyboard so you can test it out.

Those that remember the Commodore 64, you may have played with the Sound Interface Device (SID chip). 
The envelope shapes the sound using these 4 characteristics (in sequence). Attack is how fast the sound is heard. Decay is how the sound retreats from the attack. Sustain is how long the sound is heard relating to the key press. Release is how long the sound is heard regardless of the key being held down.

You can chose up to 3 oscillators to create the sound, as well as changing waveforms.

The basic workflow is:

```text
 OSC 1 ──┐
         │
 OSC 2 ──┼──► MIXER ──► FILTER ──► ADSR ──► MASTER
         │
 OSC 3 ──┘
```
