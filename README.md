#### Post script installation

This is my personal script used after a fresh arch linux installation.

- **Bootstrap script**
```
  - $ sudo pacman -S git
  - $ git clone https://github.com/hoaxdream/bootstrap
  - $ cd bootstrap
  - $ ./pkgsinstall
  - $ reboot
  - $ ./dotsetup
  - $ sudo ./partcore   # Run only for fresh disk
  - $ sudo ./partdata   # Run only for fresh disk
  - $ sudo ./postinstall
  - $ reboot
  - $ sudo -E systemctl edit --full systemd-fsck-root.service
  - $ sudo -E systemctl edit --full systemd-fsck@.service
  - $ reboot
  - $ ./fmanager
  - $ reboot
```
