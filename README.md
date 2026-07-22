# fluxbox-dots
dotfiles for my minimal fluxbox setup
<img width="1920" height="1200" alt="2026-07-21_19-57" src="https://github.com/user-attachments/assets/8f929ece-93fb-40d7-8efc-464801ae9301" />
<img width="1920" height="1200" alt="2026-07-21_19-51" src="https://github.com/user-attachments/assets/27ca06b4-6548-4467-8406-d2957ce36494" />
<img width="1920" height="1200" alt="2026-07-21_19-49" src="https://github.com/user-attachments/assets/f7637b43-2a20-493c-aff2-f02f0809ba0d" />

### Fluxbox Theming
The majority of components in this setup are themed to match the [Just Dark](https://github.com/whoami212/fluxbox-dots/tree/c7f8497ef38eedbf8f0075537829ced543d1201f/Just%20Dark) fluxbox style. To install this style, copy [Just Dark](https://github.com/whoami212/fluxbox-dots/tree/c7f8497ef38eedbf8f0075537829ced543d1201f/Just%20Dark) to your ~/.fluxbox/styles/ folder, and select it in User Styles. 
### Fonts
Tewi is used on the toolbar and window titlebars, IBM Plex Mono is used on alttab and bemenu.
### Conky
My [conky.conf](https://github.com/whoami212/fluxbox-dots/blob/73d21c97151566093add02228c940eaedd3734c1/conky.conf) is nearly identical to the default conky config, the only changes are the color (to match Just Dark) and a few added/edited modules.
### Kitty Theme
[fog.conf](https://github.com/whoami212/fluxbox-dots/blob/73d21c97151566093add02228c940eaedd3734c1/fog.conf) is colored to match [forestwallpaper.jpg](https://github.com/whoami212/fluxbox-dots/blob/39b6b54b00b9950ce3c043abde9161d047c34b85/forestwallpaper.jpg).
### alttab
The only thing I changed in the source code was a few things in src/gui.c to allow for more of a "list" view and some other small things to accommodate those changes. To install my patch, you can either clone [alttab](https://github.com/sagb/alttab.git) and replace src/gui.c with [mine](https://github.com/whoami212/fluxbox-dots/blob/39b6b54b00b9950ce3c043abde9161d047c34b85/alttab/src/gui.c), or clone my [alttab file](https://github.com/whoami212/fluxbox-dots/tree/39b6b54b00b9950ce3c043abde9161d047c34b85/alttab). Compile and install with make. 
Next, copy my alttab [launcher script](https://github.com/whoami212/fluxbox-dots/blob/39b6b54b00b9950ce3c043abde9161d047c34b85/alttab-flags) to ~/.local/bin/, and make it executable. In ~/.fluxbox/startup, add ""$HOME/.local/bin/alttab" &" anywhere before "exec fluxbox". This is how I did it, but any other method of executing the file at startup works. 
