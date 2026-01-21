# Cluster

Information for the cluster server.

## Hardware

- **OrangePi Zero 3 / 4GB**
- **OS** - Debian 13 (modified Debian 12 from OrangePi image)
- **K3S**
- **Keepalived**
- **HAProxy**

## Deployed apps

- Longhorn
- NGinxProxyManager

## Installation guide

### Initial installation

Burned the Debian Server image with Balena Etcher in all SD cards.

> Change the default repositories with Debian repositories.
> Edited `etc/apt/sources.list`.

Update repositories.
Configured static IP and hostname.
Update from Bookworm to Trixie with `sudo apt full-upgrade`.
Clean unused dependencies with `sudo apt autoremove`.
Use GParted Live to partition SD (skip if not deploying Longhorn).
