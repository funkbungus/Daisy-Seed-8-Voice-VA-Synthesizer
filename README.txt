

This code is a modification of OscPocketD/VASynth, created by Staffan Melin, staffan.melin@oscillator.se.
It was later modified by (Steven @moonfriendsynth) to work with the Daisy Pod.
Christopher @Nettech15 modified it further to run on the Daisy Seed without the use of the Daisy Pod board.
Synth parameters are now controlled by a Miditech i2-61 midi keyboard.
Feel free to copy, modify, and improve this code to match your equipment and sound requirements.

I(Funkbungus) have modified the code further in order to achieve a few things, so far I've implimented the 
folowing:

-Modify the midi impimentation for easier use with generic midi devices, this includes the loop recorder
(everything is mapped from CC02 through CC25 as of now, loading and saving not implimented yet)

-Trim down exposed parameters and expose a couple that where hidden in order to be mappable to 8 pots
 and 9 sliders (like a nektar LX49+ has)

-modify the value ranges for the ADSR envelopes to make them useable in a wider set of use cases

Todo:

-add effects section, sampler and drum machine without needing external memory 

-impliment DIN/TRS Midi 

-Reduce noise that's being introduced through the usb connection 

-add HPF and bandpass filters 

-Add alternative synth engine(s)



Specifications:

- 8 voice polyphonic.
- Dual oscillator per voice.
- VCA per voice. 
- VCF (4-pole Resonant low-pass) per voice.
- Separate ADSR's for VCA and VCF
- MIDI Editable parameters. 
- Ten User-Programmable Patches using QSPI Flash memory storage.
- Waveform select for both oscillators; Triangle / Saw / Square(PWM) / Polyblep-Saw.
- Oscillator Mix. 
- Oscillator #2 De-tune. 
- Scale for Oscillator #2. 
- LFO for Pitch Modulation Wheel.
- LFO for Pulse Width Modulation #1.
- LFO for Pulse Width Modulation #2.
- LFO for VCA/VCF Modulation.
- Waveform select for VCF/VCA LFO.
- Keyboard follow for VCF and ENV.
- Keyboard velocity routable to VCA and/or VCF. 
- VCF envelope level. 
- Stereo simulation effect.
- Single-Track ScratchPad Sequencer.
