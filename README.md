<h1>HYPRLAND WM o'rnatish uchun kichik qo'llanma</h1>

<p>Kerakli insturimentlarni paru | yay orqali o'rnatib olamiz</p>
```
yay -S gdb ninja gcc cmake libxcb xcb-proto xcb-util xcb-util-keysyms libxfixes libx11 libxcomposite xorg-xinput libxrender pixman wayland-protocols cairo pango seatd libxkbcommon xcb-util-wm xorg-xwayland
```

<p>va pacman orqali Meson utilitini o'rnatamiz</p>
```
sudo pacman -S meson
```

<p>Hyprland WM Wayland Session bo'lgani uchun SDDM login managerni o'rnatamiz<p>
```
sudo pacman -S sddm
```

<p>va SDDM servisni yoqamiz, agarda boshqa login manager yoqilgan bo'lsa uni o'chirish lozim</p>
```
sudo systemctl disable lightdm | lxdm
```

```
sudo systemctl enable sddm
```

<p>GitHub dan Hyprland WM manbasini olamiz</p>
```
git clone --recursive https://github.com/hyprwm/hyprland
```

<p>yuklab olingan manba papkasiga kiramiz</p>
```
cd hyprland
```

<p>va Hyprland WM ni o'rnatamiz</p>
```
sudo make install
```

<p>agar .config papka ichida hypr papkasi bo'lmasa yaratish lozim</p>
```bash
mkdir ~/.config/hypr
```

<p>Hyprland WM o'rnatilgandan so'ng Hyprland tomonidan tuzilgan konfigni yoki uchinchi tomon konfig fayllarni ishlatishingiz mumkin</p>
```
cp -r example/hyprland.conf ~/.config/hypr/
```

<p>va shulardan so'ng Hyprland WM ishlatishga tayyor, faqat reboot qilish qoldi halos :)</p>

#### Agarda repositoriyada hatoliklar yoki takliflar bo'lsa PR tashlashiz mumkin

#### English version - Coming Soon
#### Russian version - Coming Soon