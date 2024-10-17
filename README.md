# TouchDesigner AudioExtraction

This TouchDesigner project uses an Audio File In operator to input a song, analyze its waveform, and extract significant audio punches or beats. The system processes the audio data, focusing on high-energy peaks (or “punches”) that can be used to drive visual elements or trigger other events in a performance.

## General information:

- Audio importation - Blue:
  Select your audio file into the audiofilein CHOP, if you want to hear your audio file press the arrow in the left column of      the audio device out CHOP.

- Audio punch - Green:
  Breaks down the waveform, identifying moments of intensity by tracking amplitude changes
  - The Lag CHOP is used to make a smoother transition between punches, u can change the intensity in the Lag tab.
  - The Math CHOP is used to take the signal and change its amplitude, this means u can go from a 0 to 1 amplitude to, for example -.8 to .8 which can make a nice effect in speed operators.

- Your visuals Annotate - Red:
  -  is meant for the user to put his own visuals into that use the outputs for the Math CHOP to make changes in the visuals.

- Beat - Pink:
  - If you want to use the beat or pulse, this can be used from the Beat Annotate to create a consistent beat or pulse.
  - you can change the pulse and beat speed by changing the tempo and T Sig from the TimeCode (down left of the screen).

## Sources 

- [Youtube.com](https://youtu.be/olhePB-r7I4?si=v_DGM0fbLOYHT51p) this was used for an example particlesGPU setup.
- [Youtube.com](https://youtu.be/rGoCbVmGtPE?si=qd2QvpIqjzrw-6Bq) this was used for the the creation of audio punch
- use of ChatGPT to make this readme [Chatgpt.com](https://chatgpt.com/share/67117db5-3780-800c-8f6d-8a9b47d47a9f).
- [Soundcload.com](https://soundcloud.com/klsr_b) Musiq from artist Klsr was used as an example song for this project.
  
