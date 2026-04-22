---
icon: material/console-line
title: Shell
---

# Shell Env Setup

Update and setup the shell env.

```console
$ sudo apt update
$ sudo apt upgrade -y
```

```console
$ sudo apt install zsh
$ chsh -s `which zsh`
$ git clone https://github.com/myseq/dotfiles.git
$ echo 'source $HOME/dotfiles/shellstartup' >> .zshrc
$ echo 'source $HOME/dotfiles/shellstartup' >> .bashrc
$ logout
```


