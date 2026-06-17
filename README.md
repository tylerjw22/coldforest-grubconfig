# Custom GRUB Configuration

This repository contains a custom GRUB configuration for theming and boot menu customization.

It replaces your current GRUB config and updates the bootloader so the changes appear at startup.

This install is for Arch based systems.

---

## What this does
- Applies custom GRUB settings / theme
- Updates boot menu appearance
- Regenerates GRUB configuration

---

## Installation

### 1. Backup your current GRUB theme (recommended)
"sudo cp /boot/grub/themes/your_theme /boot/grub/themes/your_theme.backup"


### 2. Clone the repo
clone this repo to /boot/grub/themes with the one from this repo:   
"cd /boot/grub/themes"  
"git clone https://github.com/tylerjw22/coldforest-grubconfig.git"


### 3. Edit the default GRUB file
"sudo nano /etc/default/grub"
locate the "GRUB_BACKGROUND" and "GRUB_THEME" lines and replace them with:
GRUB_BACKGROUND="/boot/grub/themes/coldforest/coldforest.png"
GRUB_THEME="boot/grub/themes/coldforest"


### 4. Regenerate GRUB config
"sudo grub-mkconfig -o /boot/grub/grub.cfg"


### 5. Reboot
"sudo reboot now"

Your new GRUB configuration should now be active.

---

Enjoy!
