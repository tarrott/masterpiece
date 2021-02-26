---
title: "System Administration"
date: 2021-01-31T18:22:10-05:00
draft: false
---

## Service & Systemctl
Add `service` command to path: `export PATH="$PATH:/usr/sbin"`

## Automatic updates
- Debian: `apt install unattended-upgrades`
    - conf file: `/etc/apt/apt.conf.d/50unattended-upgrades`

## Hard Drive monitoring
- `apt install smartmontools`
    - `smartctl -V`


## Release Upgrade

### Ubuntu
1. `apt update && apt upgrade`
2. `do-release-upgrade`
    - if it fails `apt dist-upgrade`
    - if a package is broken or cannot be updated then try holding it
    - if ssh connection is lost and not using `tmux`/`screen` then resume upgrade with: `dpkg --configure -a`

#### Hold a package (apt)
- Hold a package: `sudo apt-mark hold <package-name>`
- Remove the hold: `sudo apt-mark unhold <package-name>`
- Show all packages on hold: `sudo apt-mark showhold`