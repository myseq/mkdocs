---
icon: material/package-variant-closed
title: glances
---

# Tools: Glances

`Glances` is an open-source system cross-platform monitoring tool. 
It allows real-time monitoring of our system such as 

 - CPU, memory, disk, network usage
 - monitoring of running processes 
 - monitoring of logged in users
 - temperatures
 - voltages
 - fan speeds
 - container management systems such as Docker, LXC.

See more at <https://github.com/nicolargo/glances>

## Installation

Install `glances` with : `% sudo apt install glances`

And patch it for web UI:

```conf
#!/usr/bin/env bash
apt install -y glances
systemctl enable glances.service
systemctl stop glances.service
export GLANCES_VERSION=$(glances -V | head -n 1 | awk '{print $2}' | sed 's/^v//')
wget "https://github.com/nicolargo/glances/archive/refs/tags/v${GLANCES_VERSION}.tar.gz"
tar -xzf v${GLANCES_VERSION}.tar.gz
cp -r glances-${GLANCES_VERSION}/glances/outputs/static/public/ /usr/lib/python3/dist-packages/glances/outputs/static/
sed -i '/ExecStart=\/usr\/bin\/glances -s -B 127.0.0.1/c\ExecStart=\/usr\/bin\/glances -w -B 0.0.0.0 -t 10 -p 61208' /usr/lib/systemd/system/glances.service
systemctl daemon-reload
systemctl start glances.service
```

> See <https://github.com/nicolargo/glances/issues/2021>

## Quick Start

`Glances` offers multiple modes:

 1. Standalone
 1. Client/Server (-c /-s)
 1. Web server(-w)
 1. Fetch(--fetch)





