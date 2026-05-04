# SubLoop

SubLoop is a professional MIDI bassline sequencer for underground electronic music producers.

It generates and mutates MIDI bass patterns for:

- Tech House
- Techno
- Deep Tech
- Minimal Deep Tech

SubLoop does not generate audio. It generates MIDI that can be routed into synths such as Ableton Operator, Serum, Sylenth, Vital, Diva, Pigments and other instruments.

## Product positioning

Most producers already have great synthesizers. The hard part is writing basslines that groove.

SubLoop focuses on:

- Rhythm
- Groove
- Note movement
- Style-based MIDI generation
- Controlled variation
- Fast creative workflow

## MVP goals

- 16-step MIDI sequencer
- DAW transport sync
- MIDI output only
- Style presets
- Root note and scale selection
- Pattern generation
- Pattern mutation
- Velocity, accent, gate and probability per step

## Tech stack

- C++17
- JUCE 7/8
- CMake
- VST3 first
- AU later for macOS
- GitHub Actions for basic validation
- JSON preset files

## Local development requirements

Install:

- Git
- CMake 3.22+
- A C++ compiler
  - Windows: Visual Studio 2022 with Desktop development with C++
  - macOS: Xcode command line tools
  - Linux: GCC/Clang
- JUCE

Recommended DAWs for testing:

- Ableton Live
- FL Studio
- Reaper
- Bitwig Studio

## Build concept

This repository is initialized as a professional project skeleton. The actual JUCE module can be added as a submodule, vendored dependency, or linked through a local JUCE installation.

## Database

No database is required for the plugin MVP. Audio plugins should work offline and avoid network dependency during production sessions.

Neon/Postgres may be useful later for:

- User accounts
- Cloud preset packs
- License management
- Analytics dashboard
- Community preset sharing

Those systems should live outside the plugin in a separate web/backend service.

## Repository structure

```txt
.
├── CMakeLists.txt
├── README.md
├── docs/
├── presets/
├── src/
├── tests/
└── tools/
```

## Status

Early product architecture and MVP foundation.
