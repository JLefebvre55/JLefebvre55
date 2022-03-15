# Project Ideas

> Outstanding (not yet attempted or started) project ideas.

## Trebuchet

A mathematically optimized trebuchet build using classical woodworking techniques. See `./trebuchet/` for references.

1. Simulation - genetic algorithm for various *types* of designs, optimization of each type;
2. Design - woodworking techniques and framing, structural analysis and simulation;
3. Construction

## Railgun

A high-powered, low-cost, safe, portable handheld electromagnetic propulsion device. See `./railgun/`.

1. Calculation - design total capacitor charge for projectile mass and target exit velocity;
2. Design - BoM, circuit diagrams/schematics, CADs;
3. Simulation - circuit simulation;
4. Prototyping - parts purchase and assembly
5. Manufacturing - PCB and body, user interface;
6. Testing - distance;

## Harmonizer (a la Collier)

An audio device that allows a musician to harmonize a monophonic audio signal with transpositions of itself, live.

Input: Audio signal (source), MIDI (transposition targets)
Output: Audio signal (transposed)
Controls: Mix (input vs. output), FX (on transposed signal)

1. Monophonic pitch detection (sample-averaged FFT) detects fundamental frequency
2. Each sample, the source signal is repitched to match frequencies with MIDI and added to the output signal