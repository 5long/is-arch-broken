---
layout: post
title: NetworkManager 1.22
categories: Fixed
---

After upgrading NetworkManager to 1.22, some users can no longer connect to the network. NICs managed by NetworkManager would constantly switch between the states of connected and disconnected, or simply refuse to connect.

As seen on Reddit: <https://redd.it/ecjiqb>.

## State

Should be fixed since 1.22.2.

## Workarounds

- Switch to [a different network manager][diff-nm] (e.g. systemd-networkd)
- Downgrade NetworkManager to 1.20
- Downgrade kernel to < 5.4

## Tracked elsewhere

- Arch Linux: [FS#64880]

[diff-nm]: https://wiki.archlinux.org/index.php/Network_configuration#Network_managers
[FS#64880]: https://bugs.archlinux.org/task/64880
