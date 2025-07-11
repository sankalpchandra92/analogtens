# Analog TENS Circuit
This project is based on a TENS (Transcutaneous Electrical Nerve Stimulation) unit, which is used to temporarily treat chronic or acute pain by delivering low-voltage electrical currents to the affected area through the skin.
## Waveform Generation
An astable 555 timer circuit was first designed to generate a pulse train with the desired frequency.
This signal was used to trigger a monostable 555 timer, configured to produce a pulse of the desired width on each falling edge.
A differentiator circuit was then used to extract the falling edge of the monostable output, which was used to trigger a second monostable timer, producing an equal-width pulse.
## Signal Conditioning
The output signal from the first monostable timer is fed into a non-inverting operational amplifier to buffer and isolate the waveform.
The signal from the second monostable timer is passed through an inverting operational amplifier to produce a polarity-reversed pulse.
Both amplifier outputs are routed through current-limiting resistors to ensure safe delivery of the stimulation pulses.
