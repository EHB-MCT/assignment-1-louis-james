# TouchDesigner Audio_Extraction

This TouchDesigner project uses an Audio File In operator to input a song, analyze its waveforms, and extract significant audio punches or beats. The system processes the audio data, focusing on high-energy peaks (or “punches”) that can be used to drive visual elements or trigger other events in a performance.

## Getting Started:

- **Audio importation - Blue:**
  - Select your audio file into the audiofilein CHOP, if you want to hear your audio file press the arrow in the left column of      the audio device out CHOP.

- **Audio punch - Green:**
  - Breaks down the waveform, identifying moments of intensity by tracking amplitude changes
  - The Lag CHOP is used to make a smoother transition between punches, u can change the intensity in the Lag tab.
  - The Math CHOP is used to take the signal and change its amplitude, this means u can go from a 0 to 1 amplitude to, for example -.8 to .8 which can make a nice effect in speed operators. You can change these values to      your own preferences

- **Changable - Light Blue:**
  - You can unable or disable the lag if you're not looking for smooth transitions, press the arrow button on the left side of the OP.

- **Speed - Pink:**
  - Is meant for the user to put his own visuals into that use the outputs for the Math CHOP to make changes in the visuals.


- **Your visuals - Red:**
  -  Open the visuals container, in there you can drag and drop your visuals or start the making of your visuals, use the different inputs to link them to your visuals.
  -  after the visuals are done you can connect them to the Out OP, this will link the visuals to a visuals Null OP that is linked to the MovieFileOut.
 
- **Beat and Pulse - Pink:**
  - If you want to use the beat or pulse, this can be used from the Beat Annotate to create a consistent beat or pulse.
  - you can change the pulse and beat speed by changing the tempo and T Sig from the TimeCode (down left of the screen).

- **Render Setup (Optional) - Black:**
  - Use this if you're working with 3D visuals.

- **Exporting - Orange:**
  - Switch between Visuals and Render_Input in the Switch OP by changing the Index between 0 (Visuals) and 1 (Rendering Setup)
  - Small ReadMe explaining how to export video/images to your local device with or without audio.

## Sources 

- [Make Anything Audio Reactive – TouchDesigner Tips, Tricks and FAQs 12](https://youtu.be/rGoCbVmGtPE?si=qd2QvpIqjzrw-6Bq) this was used for the the creation of audio punch
- use of ChatGPT to make this readme [Chatgpt.com](https://chatgpt.com/share/67117db5-3780-800c-8f6d-8a9b47d47a9f).
- [Soundcload.com](https://soundcloud.com/klsr_b) Musiq from artist Klsr was used as an example song for this project.
- [GITHUB & EXTERNAL TOXES FOR INTERMEDIATE](https://derivative.ca/community-post/tutorial/github-external-toxes/61020) Use GitHub with TouchDesigner
  
