# README

## Installation

Swap should be as big as RAM

## Setup

Solaar for Logi Options replacement

Enable Large Text under Accessibility settings if your monitor DPI is funny

zsh and oh-my-zsh 

FiraCode font with litigatures

```bash
sudo apt install fonts-firacode
```

~~Meslo font from NerdFonts~~

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