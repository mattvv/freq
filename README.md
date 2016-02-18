# Frequency Recognizer
An example of using Frequencies to pass messages along using Web Audio API.

The idea behind this is pretty simple, but the execution is a little harder. What if you wanted to pass a message a long an audio stream at human inaudible frequencies but have the computer able to recognize these frequencies.

To do this, I use WebAPI's oscillator to create a sine wave at a particular frequency, and then I can examine the FFT bins to determine if sound is broadcasting on this particular frequency.

I have an example working in index.html of a basic demo that creates an oscillator to create the tone, and an analyser to listen to the TTS to determine what tone could be played.

You can use WebAudioAPI to then break the parts up any way you like. You could have the tone played from one computers speakers and another computers microphone listen to it and determine what tone is being played.
