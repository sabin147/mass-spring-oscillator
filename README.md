# Mass-Spring Oscillator — Simulation & Experiment

**Type:** Academic Lab Project  
**Institution:** Roskilde University  
**Course:** BK2: Physics — Oscillations  
**Author:** Sabin Ghimire  
**Year:** 2025

## Overview

Two-part project combining numerical simulation of a classical mass-spring
system with a real physical experiment measuring resonance in an LC circuit.

## Part 1 — Numerical Simulation

Implemented the Leap-Frog integration method to simulate oscillatory motion.

**Key result:** Empirically derived the theoretical relationship T = 2π√(m/k)
through power-law regression on randomised simulation data.
The fit returned y = 6.285 · x^0.499 ≈ 2π · x, confirming the theory.

Also simulated **resonance** by adding a perturbation force Fe = 0.01·cos(2πt/Te)
and swept Te to find the resonance peak matching the natural period.

## Part 2 — Physical Experiment (LC Circuit)

Measured voltage and current across an LC circuit using an oscilloscope
across frequencies from 2 kHz to 20 kHz.

**Red inductor resonance:** 8.7722 kHz  
**Pink inductor resonance:** 12.94 kHz

Resonance identified by minimising phase angle between U1 and U2.

## Methods

- Leap-Frog numerical integration
- Power-law regression (log-log fitting)
- Zero-crossing period detection
- Oscilloscope measurements
- LC circuit resonance analysis

## Run It
```bash
pip install numpy matplotlib jupyter
jupyter notebook mass-spring-oscillator.ipynb
```

## License

MIT License — Copyright (c) 2025 Sabin Ghimire
```

---

Copyright (c) 2025 Sabin Ghimire

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

