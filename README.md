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

### 1. Clone the repo
clone this repo to /boot/grub/themes with the one from this repo:   
"cd /boot/grub/themes"  
"git clone https://github.com/tylerjw22/coldforest-grubconfig.git"


### 2. Edit the default GRUB file
"sudo nano /etc/default/grub"
locate the "GRUB_BACKGROUND" and "GRUB_THEME" lines and replace them with:
GRUB_BACKGROUND="/boot/grub/themes/coldforest-grubconfig/coldforest.png"
GRUB_THEME="boot/grub/themes/coldforest-grubconfig/theme.txt"


### 3. Regenerate GRUB config
"sudo grub-mkconfig -o /boot/grub/grub.cfg"


### 4. Reboot
"sudo reboot now"

Your new GRUB configuration should now be active.

---

Enjoy!
