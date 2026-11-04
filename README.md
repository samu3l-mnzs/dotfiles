
# 🐧 My Dotfiles

Personal configuration files for my **Arch Linux** desktop environment, focused on customization, productivity, and a clean workflow.

These dotfiles contain my preferred configurations and tools for building my daily Linux desktop experience.

## 📸 Overview

My desktop environment is built around:

- **OS:** Arch Linux
- **Window Manager:** Hyprland
- **Terminal Emulator:** Kitty
- **Terminal Emulator:** Alacritty
- **Status Bar:** Waybar
- **Application Launcher:** Wofi

## 📂 Repository Structure

```text
dotfiles/
├── alacritty/
├── hypr/
├── kitty/
├── waybar/
├── wofi/
└── README.md
```

## ⚙️ Configurations

| Component | Description |
|---|---|
| Hyprland | Wayland dynamic tiling window manager |
| Kitty | GPU-accelerated terminal emulator |
| Alacritty | GPU-accelerated terminal emulator |
| Waybar | Customizable status bar |
| Wofi | Application launcher for Wayland |

## 🚀 Installation

### 1. Clone the repository

```bash
git clone git@github.com:samu3l-mnzs/dotfiles.git
cd dotfiles
```

### 2. Back up existing configurations

```bash
mkdir -p ~/.config-backup

for dir in alacritty hypr kitty waybar wofi; do
    if [ -d "$HOME/.config/$dir" ]; then
        cp -r "$HOME/.config/$dir" \
            "$HOME/.config-backup/${dir}-$(date +%Y%m%d-%H%M%S)"
    fi
done
```

### 3. Install configurations

```bash
mkdir -p ~/.config

cp -r alacritty hypr kitty waybar wofi ~/.config/
```

**Note:** Review the configurations before copying them, especially if you already have customized settings.

## 🔄 Updating

To update your local dotfiles:

```bash
cd ~/dotfiles
git pull
```

To upload your modifications:

```bash
git add .
git commit -m "Update dotfiles"
git push origin main
```

## 📝 Notes

- These configurations are designed primarily for my personal Arch Linux setup.
- Some configurations may require additional packages or dependencies.
- Feel free to explore, adapt, and use these files as inspiration for your own setup.

## 🤝 Contributions

Suggestions and improvements are always welcome!

Feel free to fork this repository and customize it according to your needs.

---

<p align="center">
  Made with ❤️ on Arch Linux
</p>

