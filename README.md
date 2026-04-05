README.md
Adaptive Breath Switch — What It Does
This is a standalone breath-controlled MIDI trigger, part of the Jamboxx Infinite accessibility project. Its one core job is simple: you blow into your microphone, and it sends a MIDI note on/off signal — turning your breath into a musical switch. It's designed for people with limited hand mobility who can't press keys or buttons.

The Breath Engine
When you click Start Engine, the app accesses your microphone and runs the audio through a lowpass filter set to 30Hz — this isolates the slow, low-frequency energy of a breath or blow, ignoring speech and background noise. It measures the amplitude of that filtered signal and displays it as a bar meter on screen. When the level crosses the red threshold line, a MIDI Note On fires. When your breath drops back below the threshold (after a short hold-off delay to prevent flickering), a Note Off fires.

The Controls
A compact panel lets you tune four things: Gain (how sensitive the mic is), Threshold (how hard you need to blow to trigger), Velocity (how loud the MIDI note is), and Note-off Delay (how long it waits after you stop blowing before cutting the note — useful for holding notes smoothly).

The Keyboard
At the bottom sits a 3D-perspective piano keyboard. You can click or tap keys to send notes manually. There's also a Hover Mode — when switched on, simply moving your mouse over a key plays it, no clicking needed. You can set how many octaves are shown and which note it starts from.

MIDI Output
Like the other tools in this suite, it connects to a virtual MIDI port via the Web MIDI API, routing notes to your DAW or any software synth. There's a port selector, a rescan button, and a PANIC button that kills all sound on all channels instantly.

The Latency Strip
A small row of readouts shows trigger latency, note-on latency, and round-trip time in milliseconds — useful for fine-tuning your threshold to get the fastest possible response between breath and sound.Sonnet 4.6
