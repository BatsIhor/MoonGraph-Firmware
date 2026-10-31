# MoonGraph Firmware

Update images for MoonGraph e-paper moon displays. Devices download them from
this repository's releases automatically.

Each release carries one pair of files per board:

- `<board>-firmware.ota` — application firmware
- `<board>-spiffs.ota` — web interface and settings filesystem

The images are encrypted and signed. A device installs only images signed for
it, and they cannot be flashed directly to an ESP32.

To install one by hand, open `http://<device-ip>/update` on the same network
as the device and upload the `.ota` file for your board.
