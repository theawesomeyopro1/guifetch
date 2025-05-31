## 🚀 guifetch v1.0 – A Beautiful System Info GUI
A GUI fetch tool written in Flutter.


**guifetch** is a minimalist, GUI-based system info tool built with Flutter.  
Think of it as a modern, graphical alternative to tools like `neofetch` or `pfetch`.

---

### ✨ Features

- ⚡ Fast and lightweight  
- 🎨 Beautiful, clean Flutter UI  
- 🧠 Shows system info like OS, kernel, uptime, CPU, memory, and more  
- 🐧 Designed for Linux desktops (especially for window managers like Hyprland (specifically end-4's dotfiles, also known as illogical-impulse))  
- 🖼️ Comes with a `.desktop` file and icon support for app menus, but the logo looks ugly not gonna lie

## Development
Works, but you'll probably want to edit the `lib/info.dart` file for information to be correct like `neofetch`. (If you do so, please PR)

---

### 📦 Download

Grab the latest AppImage here:

👉 **[guifetch-v1.0-x86_64.AppImage](https://github.com/theawesomeyopro1/guifetch/releases/tag/guifetch#:~:text=Skip%20to%20content,guifetch%20%C2%B7%20theawesomeyopro1/guifetch)**

Make it executable:

```bash
chmod +x guifetch-v1.0-x86_64.AppImage
```

(Optional) Move it to your local `bin` to run from anywhere:

```bash
mv guifetch-v1.0-x86_64.AppImage ~/.local/bin/guifetch
```

---

### 🔧 Hyprland Keybind (Optional)

Add this to your `hyprland.conf` (or `~/.config/hypr/custom/keybinds.conf` on illogical-impulse):

```ini
bind = SUPER, G, exec, ~/.local/bin/guifetch
```

---

### 🐛 Known Issues

- Flutter-based apps may take a moment to launch the first time. (Also its based on a flutter verion (3.0.0) might update it to the latest version)

---

### ❤️ Credits

- Built by [FlafyDev](https://github.com/FlafyDev/guifetch/) but i made it better :)
- Inspired by the simplicity of `neofetch` and the power of Flutter

## Config
Located at `~/.config/guifetch/guifetch.toml`.
- `background_color` = Background color : `0xAARRGGBB`
- `os_id` = Which os id's image to display : `string`
- `os_image` = Override the image with an absolute path to an image file : `string`

## Building
1. Install Flutter (3.0.0)
2. Clone this repository and cd into it
3. Run `flutter build linux --release`
4. Launch the executable generated in `./build/linux/x64/release/bundle/guifetch`
