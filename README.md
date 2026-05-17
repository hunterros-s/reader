# CrossPoint (fork)

Personal fork of [CrossPoint Reader](https://github.com/crosspoint-reader/crosspoint-reader) v1.3.0.

A desktop simulator was added for local testing — runs natively on macOS with SDL2. No device required.

## Setup

```bash
brew install sdl2
pip install platformio
```

```bash
git clone --recursive <this-repo>
cd crosspoint-1.3.0
```

## Test locally (simulator)

```bash
pio run -e simulator -t run_simulator
```

Drop `.epub` files into `fs_/books/` — they appear at `/books` in the simulator.

| Key | Action |
|-----|--------|
| ↑/↓ | Page back/forward |
| ←/→ | Front buttons |
| Return | Confirm |
| Escape | Back |
| P | Power |
| S | Sleep |

## Flash to device

```bash
pio run --target upload
```
