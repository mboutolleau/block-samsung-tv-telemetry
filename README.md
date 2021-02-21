# Block Samsung Smart TV Telemetry

## Context

Samsung Smart TV sends data about the device usage back to the manufacturer.
This telemetry data can be an annoyance to one's privacy.

Tweaking the TV's configuration only have some limited effects.
An effective solution is to disable the telemetry by blocking the domain names used to send data back to Samsung.

Sources :

- Samsung Privacy Policy - https://www.samsung.com/us/account/privacy-policy/
- Perflyst's Smart-TV Blocklist for Pi-hole, https://github.com/Perflyst/PiHoleBlocklist/blob/master/SmartTV.txt
- MattCASmith, Setting up Pi-hole to rein in an extremely noisy Samsung Smart TV - https://mattcasmith.net/2020/02/15/pi-hole-samsung-smart-tv/

## Domain names and blocklist

The file `samsung_tv_telemetry_urls.txt` contains a list of domain names used by Samsung Smart TV for telemetry purposes.

A blocklist for [Unbound](https://nlnetlabs.nl/projects/unbound/about/) is also provided, see the file `samsung_tv_telemetry_blocklist.conf`.
