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