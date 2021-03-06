# FlatStudio-Eighties
A recolored version of FlatStudio GTK theme with Base16 Eighties/Tomorrow Night Eighties colorscheme in mind.

Just clone the repo, drop the folder on /usr/share/themes and use a program to change the theme(I recommend xfce-theme-manager).

## Screenshot
![alt text](screenshot.png "Thunar, htop, mps-youtube, Sublime Text and XFCE's Whisker Menu")

## Tip
Some applications doesn't work quite well with dark gtk themes(Firefox, Thunderbird, Liferea, Monodevelop to name a few) so it's highly recommended to override your current GTK theme and make the application load another gtk theme, if you use XFCE you can modify the launchers through menulibre like this(or mannualy edit the launchers at ~/.local/share/applications/):

#### This example is assuming that you have the Numix GTK theme installed.

### GTK3 Applications:
```
zsh -c "GTK_THEME=/usr/share/themes/Numix/gtk-3.0/gtk.css firefox %u"

zsh -c "GTK_THEME=/usr/share/themes/Numix/gtk-3.0/gtk.css thunderbird %u"
```

### GTK2 Applications:
```
zsh -c "GTK2_RC_FILES=/usr/share/themes/Numix/gtk-2.0/gtkrc libreoffice5.0"
```

If you use bash, just change "zsh -c" to "bash -c".

## Attribution

### FlatStudio
Author: Rafa Cobreros<br>
License: GPL<br>
http://gnome-look.org/content/show.php/FlatStudio?content=154296<br>

### Base16 and Tomorrow Theme
Author: Chris Kempson<br>
License: MIT<br>
https://github.com/chriskempson/base16<br>
https://github.com/chriskempson/tomorrow-theme<br>