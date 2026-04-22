---
icon: material/console-line
title: Config
---

# Configuration

To create config links (manually):

```console
% ln -s dotfiles/vimrc ~/.vimrc
% ln -s dotfiles/gitconfig ~/.gitconfig
% ln -s dotfiles/pythonstartup ~/.pythonstartup
```

## Timezone

To set the timezone:

```console
% sudo timedatectl set-timezone Asia/Singapore
```

## Locale

To configure locale:

```console
% sudo locale-gen en_US.UTF-8
% sudo dpkg-reconfigure locales
% sudo update-locale LANG=en_US.UTF-8
```


