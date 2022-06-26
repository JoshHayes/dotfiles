# README

## Installation

Swap should be as big as RAM

## Setup

Enable Large Text under Accessibility settings if your monitor DPI is funny.
Recover backspace-to-go-back in Firefox by setting `browser.backspace_action` to 0 under `about:config`.

```bash
# Solaar for Logi Options replacement
sudo apt install solaar

# FiraCode font with litigatures
sudo apt install fonts-firacode

# zsh and oh-my-zsh 
sudo apt install zsh
chsh -s $(which zsh)    # remember to logout

# Bitwarden
# TODO

# Chezmoi
curl -sfL https://git.io/chezmoi | sh
sudo mv ./bin/chezmoi /usr/local/bin/

# Run chezmoi
chezmoi init JoshHayes
chezmoi apply

cd $(chezmoi source-path)
git remote set-url origin git@github.com:JoshHayes/dotfiles.git




```

Dropbox 

- issue: can only run one instance unless we hack the home dir [link](https://askubuntu.com/questions/475419/how-to-link-and-use-two-or-more-dropbox-accounts-simultaneously)
- issue: no smart sync on linux

AWS credentials and config in .aws 

### MATLAB

Install MATLAB — to get around the permissions for /usr/local/, do 

```bash
xhost +SI:localhost:root
sudo ./install
```

- Issue: Matlab starts with OpenGL but there is shit missing on Ubuntu.

### Git

You should be using SSH not HTTPS. Anyways, to store your credentials first do 

```bash
git config --global credential.helper cache
```

and then enter your name and the personal access token.

### Docker

Install Docker via the CLI, you may need to update permissions

```bash
chmod 777 /var/run/docker.sock
```