---
icon: material/package-variant-closed
title: hugo
---

# Tools: Hugo

`Hugo` is a static site generator.
It is always used at GitHub Pages.

See more at <https://gohugo.io>

## Installation

Install specific version (v0.139.4) of Hugo:

```console
% wget https://github.com/gohugoio/hugo/releases/download/v0.139.4/hugo_extended_0.139.4_linux-amd64.deb
% sudo dpkg -i hugo_extended_0.139.4_linux-amd64.deb
% hugo version
hugo v0.139.4-3afe91d4b1b069abbedd6a96ed755b1e12581dfe+extended linux/amd64 BuildDate
```

## Quick Start

To create a new post:

```console
% hugo new content posts/first.md
```

(Optional) To prevent any upgrade or `Hugo` version:

| Action | Apt (.deb) Command | Snap Command |
| :----- | :----------------- | :----------- |
| Lock Version | `sudo apt-mark hold hugo` | `snap refresh --hold hugo` |
| Check Status | `apt-mark showhold` | `snap list hugo` (look for "held") |
| Unlock | `sudo apt-mark unhold hugo` | `snap refresh --unhold hugo` |


## Upgrade

```
% apt-mark showhold 
hugo
% sudo apt-mark unhold hugo
% wget https://github.com/gohugoio/hugo/releases/download/v0.165.0/hugo_extended_0.165.0_linux-amd64.deb
% sudo dpkg -i hugo_extended_0.165.0_linux-amd64.deb
% hugo version
hugo v0.165.0-76a5e1880ab46688155b02e99bab9be2a6134492+extended linux/amd64 BuildDate=2026-08-12T14:26:28Z VendorInfo=gohugoio
```



