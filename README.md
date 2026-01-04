# MSC2OSC

A standalone macOS menu bar application that bridges MIDI Show Control (MSC) commands to Open Sound Control (OSC).

## Features

- Real-time MSC to OSC translation with sub-millisecond latency
- Configurable OSC path format with token substitution (`{command}`, `{cue}`, `{list}`, etc.)
- Per-command OSC name and argument format customization
- Menu bar service mode with status indicators
- MIDI source selection with auto-reconnect
- Live message log with filtering

## Installation

1. Download `MSC2OSC.dmg` from the [Releases](https://github.com/thekwallace/MSC2OSC/releases) page
2. Open the DMG and drag MSC2OSC to Applications
3. Launch MSC2OSC - it will appear in your menu bar

## Requirements

- macOS 14.0 (Sonoma) or later
- Apple Silicon or Intel Mac

## Usage

1. Select your MIDI input source in Settings (⌘,)
2. Configure the OSC output host and port
3. Customize command mappings if needed
4. The app will bridge all incoming MSC commands to OSC

### Available Tokens for Path/Argument Format

| Token | Description |
|-------|-------------|
| `{command}` | The MSC command name (go, stop, etc.) |
| `{cue}` | Cue number |
| `{list}` | Cue list number |
| `{path}` | Cue path |
| `{format}` | Command format (lighting, sound, etc.) |
| `{device}` | Device ID |

## License

Copyright © 2024. All rights reserved.
