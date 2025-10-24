# cli:bat

A cat(1) clone with syntax highlighting and Git integration.

See more <https://github.com/sharkdp/bat>.

## Installation

Simply `sudo apt install bat`.

## Testing

```
% batcat /etc/lsb-release
───────┬──────────────────────────────────────────────────────────────────────────────────────────────────
       │ File: /etc/lsb-release
───────┼──────────────────────────────────────────────────────────────────────────────────────────────────
   1   │ DISTRIB_ID=Ubuntu
   2   │ DISTRIB_RELEASE=24.04
   3   │ DISTRIB_CODENAME=noble
   4   │ DISTRIB_DESCRIPTION="Ubuntu 24.04.3 LTS"
───────┴──────────────────────────────────────────────────────────────────────────────────────────────────
```

## Options

 * Use `batcat --config-file` to show the config file path.
 * Use `batcat --list-themes` to list all themes.
 * To use specific theme, just `batcat --theme=TwoDark python_script.py`.
 * To set environment variable, `export BAT_THEME="TwoDark"`.



