# Sweet-Arise

This is a modified theme heavily based on the [Sweet Dark Theme](https://www.gnome-look.org/p/1253385) and loosely on the color scheme in [Solo Leveling](https://en.wikipedia.org/wiki/Solo_Leveling).

> Note that this is my first time using custom css for gnome and second time using css as a whole so I'm really bad at this :'). The theme might (_will_) be broken or look not as intended on a different setup or a different configuration. I have given as much info about my setup as I can as a result.

## Required Extensions:

|   Extensions   |                               |
|----------------|-------------------------------|
|[AppIndicator/KStatusNotifierItem](https://extensions.gnome.org/extension/615/appindicator-support/) | Adds app indicators to the top bar (for apps like discord).
|[Aylur's Widgets](https://extensions.gnome.org/extension/5338/aylurs-widgets/)| Useful Widgets like the dashboard, quick settings menu and the media player. |
|[Dash to Panel](https://extensions.gnome.org/extension/1160/dash-to-panel/)| Needed for the taskbar in the center left of the top bar and resizing the bar to make it larger |
|[Extension List](https://extensions.gnome.org/extension/3088/extension-list/)| Gives an easy way to access the list of all extensions installed on the device and a way to toggle them on/off too. |
| [Rounded Window Corners](https://extensions.gnome.org/extension/5237/rounded-window-corners/)| Bitch magnet|
| [Useless Gaps](https://extensions.gnome.org/extension/4684/useless-gaps/)| Super Bitch magnet|
| [User Themes](https://extensions.gnome.org/extension/19/user-themes/)| Allows changing of the shell theme to a  custom one (must have for the theme to even work) |

## Install Instructions:

### Get the Setup without the terminal:
1. Get the Required Extensions
2. Get the Sweet Dark Theme and GNOME Tweaks and your preferred icon and cursor themes.
3. Go to `~/.themes/Sweet-Dark-v40/gnome-shell` and duplicate the `gnome-shell.css` file and rename it to something else.
4. Either download the raw `gnome-shell.css` file from this repo and replace it or just use any text editor to copy and replace the text in the file.
5. Refresh the theme using GNOME Tweaks (or <kbd>Alt</kbd> + <kbd>F2</kbd> and enter `r` if you're in an Xorg session).
The theme should have worked and will not look like mine since I'm terrible at CSS.

### Get the terminal theme:
1. Get `zsh` and `oh-my-posh` for the theming and do their default setup.
2. Download `tablets.omp.json` from this repo into your local system.
3. If you didn't use `easy-zsh-config`, [follow these steps](https://ohmyposh.dev/docs/installation/customize). If you did use it, with root access, change `PATH_OF_THE_THEME` variable to the path of the downloaded file in `/etc/zsh/zshrc`.


## Config Details:

| Configs  | |
|----------|-|
|[Tela Circle Purple](https://www.gnome-look.org/p/1359276)| Icon Theme|
|[Qogir Dark](https://www.gnome-look.org/p/1366182)| Cursor Theme|
| #8500f7 | Color for the borders (use this to set the window borders in the rounded window corner extension)|
|zsh | My default shell|
| [easy-zsh-config](https://aur.archlinux.org/packages/easy-zsh-config)|An AUR package that sets up zsh with some nifty plugins and [oh-my-posh](https://ohmyposh.dev/) with the atomic theme as the default.|
|[Gradience](https://flathub.org/apps/details/com.github.GradienceTeam.Gradience)| Change the look of the Adwaita apps to match the color scheme of the shell theme.|
|Aylur's Widgets| Turn on dashboard, date menu tweaks, media player and quick settings tweaks. Refer to the section about the Widgets for more detailed stuff.|
|Dash to panel| 46px panel thickness and date menu in the monitor center (can cause bugs on wayland (in my experience) -> date menu becomes invisible), left box above the date menu and stacked to the right.|
| [Neofetch Theme](https://github.com/chick2d/neofetch-themes/blob/main/normal/acenoster.conf) | The neofetch config I used.|
| Wallpaper | [Thank u/Niel_MDR!](https://www.reddit.com/r/sololeveling/comments/e5z0ck/just_created_a_reddit_acc_so_i_can_post_this/)|

### Aylur's Widget Fine-tuning:
- Dash Board (on):
    - Enable Panel Button:
        - Position : Left 0
        - Show Icon (optional)
        - Label (optional)
    - X Align: Center
    - Y Align: Center
    - X Offset: 0
    - Y Offset: 0
    - Darken Background (optional)
    - Widgets (optional)
- Date Menu Tweaks (most likely to break):
    > Tip: If you aren't super interested in the Date Menu being in the monitor center and the taskbar style, do not use the Dash to Panel extension. Stuff should work well without it. The following hierarchical list is just my setup that I based the modifications of the theme on. Feel free to appropriate as you wish.
    - Hide notifications (on)
    - Hide Stock Mpris (on)
    - Enable Custom Menu (**OFF**)
    - Position: Center 0
    - Remove Padding (on)
    - Indicator Position: Right
    - Format: `%b %e  %I:%M %p`
- Other settings can be whatever