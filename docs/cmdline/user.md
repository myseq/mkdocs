---
icon: material/console-line
title: User
---

# User Management

Adding an user `xx` and adding to `sudo` group.

```console
% sudo adduser xx
% sudo usermod -aG sudo xx
% groups xx
xx : xx sudo users
% sudo whoami
root
```

Adding user with low-level cmd (with home folder created): `% sudo useradd -m yy`


