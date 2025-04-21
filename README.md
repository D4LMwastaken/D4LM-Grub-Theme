# D4LM Grub Theme
A GRUB2 Theme for Framework laptops forked now for D4LM's use

## Installation (**For Fedora**)
1. Clones the repository
```bash
git clone https://github.com/D4LMwastaken/D4LM-Grub-Theme.git
```

Copy the folders to `/boot/grub/themes/`:
```bash
sudo cp -r D4LM-Grub-Theme/D4LM-Theme /usr/share/grub/themes

```

Change the GRUB theme by setting `GRUB_THEME` in `/etc/default/grub` :
```bash
sudo nano /etc/default/grub # Technically use Zed but for non-Zed users
```

```
GRUB_THEME="/usr/share/themes/D4LM-Theme/theme.txt"
```

Rebuild the `grub.cfg`:
```bash
sudo grub2-mkconfig -o /etc/grub2.cfg 
```

Reboot to see the changes:
```bash
reboot
```

## Editing
Feel free to fork or use...
