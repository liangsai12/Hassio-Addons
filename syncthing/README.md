# Syncthing Addon

[Syncthing](https://syncthing.net/) wrapped inside a Homeassistant supervisor addon.

Syncthing is a continuous file synchronization program. It synchronizes files between two or more computers in real time, safely protected from prying eyes. Your data is your data alone and you deserve to choose where it is stored, whether it is shared with some third party, and how it's transmitted over the internet.

![Addon Stage][stage-badge]
![Supports aarch64 Architecture][aarch64-badge]
![Supports amd64 Architecture][amd64-badge]
![Supports armhf Architecture][armhf-badge]
![Supports armv7 Architecture][armv7-badge]
![Supports i386 Architecture][i386-badge]

[![Install on my Home Assistant][install-badge]][install-url]
[![Donate][donation-badge]][donation-url]

# Folders available

When using this addon to permanently hold your data, put the synced folder inside `/data`. Otherwise it will be deleted on container restart. Note that this folder and its contents will be included in each backup of the addon.

Also the `/share`, `/confg`, `/backup`, `/addons` and `/ssl` folders are mapped inside. You can use them as persistant storage. Some of those are not included in backups of the hassio configuration by default.

Syncing those folders can also be used to backup the Home Assistant backups, for example. 

# Configuration

The configuration is done via the web ui. Start the addon and configure it there.


[aarch64-badge]: https://img.shields.io/badge/aarch64-yes-green.svg?style=for-the-badge
[amd64-badge]: https://img.shields.io/badge/amd64-yes-green.svg?style=for-the-badge
[armhf-badge]: https://img.shields.io/badge/armhf-yes-green.svg?style=for-the-badge
[armv7-badge]: https://img.shields.io/badge/armv7-yes-green.svg?style=for-the-badge
[i386-badge]: https://img.shields.io/badge/i386-yes-green.svg?style=for-the-badge
[install-url]: https://my.home-assistant.io/redirect/supervisor_addon?addon=243ffc37_syncthing
[stage-badge]: https://img.shields.io/badge/Addon%20stage-stable-green.svg?style=for-the-badge

[install-badge]: https://img.shields.io/badge/Install%20on%20my-Home%20Assistant-41BDF5?logo=home-assistant&style=for-the-badge
[donation-badge]: https://img.shields.io/badge/Buy%20me%20a%20coffee-%23d32f2f?logo=buy-me-a-coffee&style=for-the-badge&logoColor=white
[donation-url]: https://www.buymeacoffee.com/Poeschl
