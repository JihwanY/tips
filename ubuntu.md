# ubuntu 16.04
## Display resolution becomes low and cannot change
```
sudo mv /etc/X11/xorg.conf /etc/X11/xorg.conf.old
sudo touch /etc/X11/xorg.conf
sudo reboot
```

## Setting Korean Keyborads
### install
'''
sudo apt-get install fcitx-hangul
'''
System Settings > Language Support
Keyboard input method system to 'fcitx'
reboot
### set shortcut
AllSettings > Keyboard > Shortcuts Tab > Typing
Disabled 'Switch to Next source, Switch to Previous sourc, Compose Key, Alternative Characters Key' (backspace)
Compose Key to Right Alt by clicking Disabled long
fcitx on the right top menu bar and choose Configure Current Input Method
Add Hangul by clicking '+'  (Uncheck “Only Show Current Language”)
Global Config > change Trigger Input Method as Multikey by pressing 한/영키. Disable Extrakey for trigger input method
Global Config tap > Program > Share State Among Window > All
### test
Log out and Log in
Test
