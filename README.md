# AudioDSP-Oscillator

This repository contains an implementation of a **Bandlimited Impulse Train (BLIT) Oscillator** for audio synthesis.

## Features
- Generates a sinc pulse every `period` samples.
- Supports frequency modulation (vibrato, pitch bend, glide).
- Includes square wave generation using phase shifting.

## Usage
Include `Oscillator.h` in your project:
```cpp
#include "Oscillator.h"

# Then create an instance:

Oscillator osc;
osc.period = 44100.0f / 440.0f; // A4 pitch
float sample = osc.nextSample();
