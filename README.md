```
  _                         _____                                  _ 
 | |                   _   / ____|                                | |
 | |     _____   _____(_) | (___   ___ _ ____   _____ _ __ ___  __| |
 | |    / _ \ \ / / _ \    \___ \ / _ \ '__\ \ / / _ \ '__/ _ \/ _` |
 | |___| (_) \ V /  __/_   ____) |  __/ |   \ V /  __/ | |  __/ (_| |
 |______\___/ \_/ \___(_) |_____/ \___|_|    \_/ \___|_|  \___|\__,_|

```
A fork of LOVE2D for server-side Lua scripting.  
Strips away graphics, audio, input, and other client-only APIs when run with `--server`.

## 🔧 Features

- `--server` mode: run LOVE without graphics/audio/input
- Headless-friendly (runs on servers, containers, etc.)

## 🚀 Usage

### Server mode
```bash
./love --server thing.love
```

### Normal mode
```bash
./love thing.love
```

In `--server` mode, the following modules are disabled:

- `love.graphics`
- `love.audio`
- `love.keyboard`
- `love.joystick`
- `love.mouse`
- `love.touch`
- `love.window`
- `love.video`
- `love.image`
- `love.system.vibrate`

## 🛠️ Build (Linux)

```bash
./platform/unix/automagic
./configure
make
```

## ⚠️ Status

**UNSTABLE / EXPERIMENTAL**  
Things might break. PRs welcome.

## 📜 License

Same as LOVE2D (zlib/libpng)

## Notes
- Only linux is supported for now
- Based on LOVE 11.5
- Meow
