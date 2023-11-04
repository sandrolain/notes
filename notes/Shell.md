# Shell

## Commands

- [**commandlinefu.com** is the place to record those command-line gems](https://www.commandlinefu.com/)

## Emulate `ll` command on mac

```sh
# in .zshrc or .profile
alias ll='ls -alG'
```

## Zsh

- https://ohmyz.sh/
- https://github.com/ohmyzsh/ohmyzsh/wiki/Themes
- https://github.com/powerline/fonts
  *iTerm2 users need to set both the Regular font and the Non-ASCII Font in "iTerm > Preferences > Profiles > Text" to use a patched font*

```shell
ZSH_THEME="agnoster"

plugins=(git kubectl docker docker-compose iterm2 brew)
```

### Zsh Kubernetes

- [kube-ps1: Kubernetes prompt for bash and zsh](https://github.com/jonmosco/kube-ps1)
