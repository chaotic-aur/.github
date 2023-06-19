### How to use it?

- First, install the primary key - it can then be used to install our keyring and mirrorlist:
  - `# pacman-key --recv-key 3056513887B78AEB --keyserver keyserver.ubuntu.com`
  - `# pacman-key --lsign-key 3056513887B78AEB`
  - `# pacman -U 'https://cdn-mirror.chaotic.cx/chaotic-aur/chaotic-keyring.pkg.tar.zst' 'https://cdn-mirror.chaotic.cx/chaotic-aur/chaotic-mirrorlist.pkg.tar.zst'`
- Append (adding to the **end** of the file) to `/etc/pacman.conf`:
  - `[chaotic-aur]`
  - `Include = /etc/pacman.d/chaotic-mirrorlist`

### About

- Most packages available in this repo are automatically built from their respective AUR source package. However, there are a few exceptions, check out the [packages repo](https://github.com/chaotic-aur/packages) to find out which ones.
- The primary building cluster is a node in UFSCar's datacenter which is hosted in São Carlos, São Paulo, Brazil.

### Some handy links

- Telegram channel with news and updates: [@chaotic_aur](https://t.me/s/chaotic_aur)
- Community group for on- and offtopics: [@chaotic_aur_sac](https://t.me/s/chaotic_aur_sac) - feel free to come by! 😊
- Package list: [Pkgs.org](https://archlinux.pkgs.org/rolling/chaotic-aur-x86_64/)
- Status page: [Status monitoring](https://status.chaotic.cx/)
- Latest logs: [Logfiles](https://builds.garudalinux.org/repos/chaotic-aur/logs/)
- Chaotic keys: [Keyring](https://aur.chaotic.cx/chaotic.gpg)
