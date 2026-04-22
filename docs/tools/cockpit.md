---
icon: material/package-variant-closed
title: cockpit
---

# Tools: Cockpit

Cockpit is a web-based graphical interface for servers to perform system administration on the Linux OS.
It also provide terminal shell access via browser.

See more at <https://cockpit-project.org/>

## Installation

Install and start `cockpit`.

```console
% sudo apt install -u cockpit
% sudo systemctl enable --now cockpit.socket
% sudo systemctl status cockpit.socket
```

By default, `cockpit` will run and listen on TCP port 9090.

## Quick Start

After installing and enabling Cockpit, visit port 9090 on your server. 
For example, open browser at <http://localhost:9090> for same machine.
And you will be able to login with user/password.


