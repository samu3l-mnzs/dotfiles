My Dotfiles 🐧

Personal configuration files for my Fedora Linux environment.

📂 Structure
text
dotfiles/
├── hypr/
│   └── hyprland.lua
├── kitty/
│   └── kitty.conf
├── waybar/
│   ├── config.jsonc
│   └── style.css
└── README.md

⚙️ Configurations
Component	Description
Hyprland	Window manager configuration
Kitty	Terminal emulator configuration
Waybar	Status bar configuration
🚀 Installation

Clone the repository:

bash
git clone git@github.com:samu3l-mnzs/dotfiles.git
cd dotfiles


Copy the configuration files to their respective directories:

bash
mkdir -p ~/.config/hypr ~/.config/kitty ~/.config/waybar

cp hypr/hyprland.lua ~/.config/hypr/
cp kitty/kitty.conf ~/.config/kitty/
cp waybar/config.jsonc ~/.config/waybar/
cp waybar/style.css ~/.config/waybar/


Note: Back up your existing configurations before copying these files.

💻 Environment
OS: Fedora Linux
Window Manager: Hyprland
Terminal: Kitty
Status Bar: Waybar
📝 Notes

These are my personal configuration files. Feel free to explore, adapt, and use them as inspiration for your own Linux setup.

Made with ❤️ on Fedora Linux.
