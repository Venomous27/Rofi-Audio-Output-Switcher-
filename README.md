# 🎧 Rofi Audio Output Selector

A simple Rofi menu for switching your default PulseAudio output device.

It displays **friendly device names** (Speakers, HDMI, Headphones, etc.) instead of PulseAudio's internal device names, making it quick and easy to switch outputs.

---

<img width="800" height="450" alt="2026-07-0816-55-37online-video-cutter com-ezgif com-video-to-gif-converter" src="https://github.com/user-attachments/assets/f440c5da-a8ee-40ba-bc0a-40b4fb2f140d" />

---
## Features

* 🎵 Switch default PulseAudio output device
* 🔍 Search devices with Rofi
* ✨ Friendly device descriptions
* 🎨 Custom Rasi theme support
* ⚡ Lightweight Bash script

---

## Requirements

Make sure you have the following installed:

* **PulseAudio**
* **Rofi (Wayland build recommended for Wayland users)**

### Arch / CachyOS

```bash
sudo pacman -S rofi-wayland pulseaudio
```

> If you're using another distribution, install the equivalent packages using your package manager.

---

## Installation

1. Copy `audio-output.sh` somewhere in your `$PATH`, for example:

```text
~/dotfiles/rofi/.config/rofi/scripts/audio-output.sh
```

2. Copy `audio-output.rasi` to your Rofi themes directory, for example:

```text
~/dotfiles/rofi/.config/rofi/themes/audio-output.rasi
```

3. Open `audio-output.sh` and change the Rasi theme path to wherever you placed your theme.

Example:

```bash
-theme ~/dotfiles/rofi/.config/rofi/themes/audio-output.rasi
```

4. Make the script executable:

```bash
chmod +x ~/dotfiles/rofi/.config/rofi/scripts/audio-output.sh
```

---

## Hyprland Keybind

Add the following to your `hyprland.conf`:

```ini
bind = SUPER, ALT_L, exec, ~/dotfiles/rofi/.config/rofi/scripts/audio-output.sh
```

If you keep the script somewhere else, update the path accordingly.

> Not using Hyprland? Simply launch the script however your desktop environment or window manager handles keybindings.

---

## Credits

Script written with the help of **ChatGPT (OpenAI GPT-5.5)**.

---

## License

Feel free to modify, improve, and share this script.

