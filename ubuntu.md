# ubuntu 16.04
## Display resolution becomes low and cannot change
```
sudo mv /etc/X11/xorg.conf /etc/X11/xorg.conf.old
sudo touch /etc/X11/xorg.conf
sudo reboot
```

## Setting Korean Keyborads
### install
```
sudo apt-get install fcitx-hangul
```
- System Settings > Language Support
- Keyboard input method system to 'fcitx'
- reboot
### set shortcut
- System Settings > Keyboard > Shortcuts Tab > Typing
- Disabled _Switch to Next source_, _Switch to Previous source_, _Compose Key_, _Alternative Characters Key_' (backspace)
- Set _compose Key_ to Right Alt by clicking Disabled long
- Click fcitx on the right top menu bar and choose _Configure Current Input Method_
- Add Hangul by clicking '+'  (Uncheck “Only Show Current Language”)
- Global Config > change _Trigger Input Method_ as Multikey by pressing 한/영키. Disable Extrakey for trigger input method
- Global Config tap > Program > Share State Among Window > All
### test
- Log out and Log in
- Test
