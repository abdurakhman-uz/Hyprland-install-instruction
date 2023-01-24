<h1>HYPRLAND WM o'rnatish uchun kichik qo'llanma</h1>

Kerakli insturimentlarni paru | yay orqali o'rnatib olamiz
```
yay -S gdb ninja gcc cmake libxcb xcb-proto xcb-util xcb-util-keysyms libxfixes libx11 libxcomposite xorg-xinput libxrender pixman wayland-protocols cairo pango seatd libxkbcommon xcb-util-wm xorg-xwayland
```

va pacman orqali Meson utilitini o'rnatamiz
```
sudo pacman -S meson
```

Hyprland WM Wayland Session bo'lgani uchun SDDM login managerni o'rnatamiz
```
sudo pacman -S sddm
```

va SDDM servisni yoqamiz, agarda boshqa login manager yoqilgan bo'lsa uni o'chirish lozim<
```
sudo systemctl disable lightdm | lxdm
```

```
sudo systemctl enable sddm
```

GitHub dan Hyprland WM manbasini olamiz
```
git clone --recursive https://github.com/hyprwm/hyprland
```

yuklab olingan manba papkasiga kiramiz
```
cd hyprland
```

va Hyprland WM ni o'rnatamiz
```
sudo make install
```

agar .config papka ichida hypr papkasi bo'lmasa yaratish lozim
```
mkdir ~/.config/hypr
```

Hyprland WM o'rnatilgandan so'ng Hyprland tomonidan tuzilgan konfigni yoki uchinchi tomon konfig fayllarni ishlatishingiz mumkin
```
cp -r example/hyprland.conf ~/.config/hypr/
```

va shulardan so'ng Hyprland WM ishlatishga tayyor, faqat reboot qilish qoldi halos :)

#### Agarda repositoriyada hatoliklar yoki takliflar bo'lsa PR tashlashiz mumkin

#### English version - Coming Soon
#### Russian version - Coming Soon