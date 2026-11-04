# PocketBench

A browser-based electronics lab bench simulator, built for practising first-year electrical-engineering lab sessions without the real instruments.

It reproduces the front panels of the bench instruments and a Hirschmann breadboard, and simulates the circuit you wire up:

- **Oscilloscope** HAMEG HMO2024 / HMO724: channel menus, VOLTS/DIV, TIME/DIV, trigger (level, slope, source, filter, auto/normal/single), AUTOSET, cursors, AUTO MEASURE, QUICK VIEW, MATH, REF, FFT, XY, ZOOM, acquisition modes, screenshots.
- **Function generator** HAMEG HMF2550 / HMF2525: sine, square, triangle, pulse, arbitrary; keypad and knob entry; OFFSET, INVERT, 50 Ω output, High-Z / 50 Ω load; MOD, SWEEP, BURST.
- **Power supply** HAMEG HMP2030: three floating channels, CV/CC with current limit, electronic fuse, tracking, store/recall.
- **2 × multimeter** HAMEG HMC8012: DC/AC voltage and current, resistance, capacitance, continuity, diode, ranges, 2nd function, statistics, limits, NULL, HOLD.
- **Hirschmann breadboard** with resistors, capacitors, inductors, diodes, LEDs, Zener, µA741 op-amp and potentiometer, coloured jumper wires, banana leads, BNC coaxial cables and BNC-to-banana adapters.

The simulation includes real-world effects: 50 Ω generator output resistance, power-supply current limiting, meter shunts and input impedances, AC bandwidth of the multimeter, common earth of the oscilloscope and generator, quantisation, noise and pickup on unshielded leads. An "ideal instruments" setting turns these off.

## Use

Open `index.html` in a desktop browser. Projects are autosaved in the browser, can be saved under a name, and exported/imported as `.pbench` files that restore the bench exactly.

Light and dark themes, French and English interface.

## Hosting

Single self-contained file — put `index.html` at the root of a GitHub Pages repository.
