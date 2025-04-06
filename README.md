# miniModularSynth
![image](https://github.com/user-attachments/assets/43e60d6d-3de6-4cbe-aabd-5aeecd0bb9f6)![image](https://github.com/user-attachments/assets/eb2c0d51-f5ec-4262-a54c-119b0abcf2e9)

Many tiny open source hardware synth modules (miniLFO, MiniVCA, MiniMix, MiniVCF, MiniEnv, miniPower) combine to make a tiny modular.
STILL A WORK IN PROGRESS,  I will be uploading Kicad schematics and PCB's over the first half of April 2025

So far we have built and verified:
- miniMCU v2,
- miniAudioMixer,
- miniVCA v3.0

Unverified but completed schematic (PCB layout happening as we speak)
- miniLFO
- miniVCF
- miniAdder
- miniPower
- miniEnv
- miniMux
- miniS&H
- miniLogic
- miniBinaryCounter

 Each of these sub-modules is a building block that contributes to the functionality of the Analog Switch Mini. Explore the individual notes for detailed design and technical aspects.

- ### Mini Modules Overview  
#### • [[miniLFO]]  
  - • A low-frequency oscillator module that generates modulation signals for other modules in the system.  
  - • It may include a submodule (as noted by the “MiniLED Indicator”), which can serve as a visual element or part of its modulation feedback.

#### • [[MiniVCA]]  
  - • A compact voltage-controlled amplifier designed to modulate signal amplitudes.  
  - • The module is built to be part of a system where “clean” versus “distorted” VCA characteristics can be explored for different sound textures.

#### • MiniMix (often referred to as [[TinyMix]] in your query)  
  - • A small mixer module used for blending multiple audio signals.  
  - • This module is meant to work in tandem with the other tiny modules, ensuring that various elements (oscillators, filters, VCAs, etc.) can be combined seamlessly.

#### • MiniVCF / [[VCFMini]]  
  - • A voltage-controlled filter module responsible for shaping frequency content.  
  - • It integrates with the rest of the system to allow for creative filter responses, drawing design ideas from several filter architectures described in related notes.

#### • [[MiniEnv]]  
  - • An envelope (or trigger) module (aliased as MiniEnv) that defines the amplitude or modulation contours over time.  
  - • This module adds dynamic evolution to the sounds produced by the synthesizer.

#### • [[miniPower]]  
  -
  - • It is designed to transform USB 5V power into a ±10V supply, which is essential for biasing and powering the analog circuits used by the other modules.

- ## - 2. The Overall Project  
### • Core Concept  
  - • The project entails building a compact, modular synthesizer system based on a MiniPCB (or miniMCU).  
  - • It is designed to integrate multiple tiny modules (miniLFO, MiniVCA, MiniMix, MiniVCF, MiniEnv, miniPower) into one coherent unit, providing functions from oscillation and filtering to amplification, mixing, and power regulation.

### • Integration and Modular Flexibility  
  - • The MiniPCB serves as the base platform to which each module attaches, creating a versatile and reconfigurable Eurorack-compatible synthesizer system.  
  - • The design allows for different “flavors” of sound (e.g. clean versus distorted outputs) by offering variant modules such as the MiniVCA.
