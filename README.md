# Qv2ray Debian Repository

This project is a Debian repository hosted on GitHub Pages.

## Supported Distributions

- Debian Buster
- Debian Bullseye/Sid
- Ubuntu 20.04 (Focal Fossa)
- Ubuntu 20.10 (Groovy Gorilla)

## Configuration

### Official Repository

```bash

# Install lsb-releases
$ sudo apt install lsb-release

# Install some prerequisites needed by adding GPG public keys
$ sudo apt install gnupg ca-certificates curl

# Import our GPG key. Notice the hyphen at the end of line.
$ curl -sSL https://qv2ray.net/debian/pubkey.gpg | sudo apt-key add -

# Add the our official APT repository:
$ echo "deb [arch=amd64] https://qv2ray.net/debian/ `lsb_release -cs` main" | sudo tee /etc/apt/sources.list.d/qv2ray.list

# To update the APT index:
$ sudo apt update

# You can install Qv2ray from APT now:
$ sudo apt install qv2ray
```

### FastGit Mirror (in case `qv2ray.github.io` is blocked)

[![fastgit.org](https://img.shields.io/badge/powered--by-fastgit.org-blue)](https://fastgit.org/)

```bash

# Install lsb-releases
$ sudo apt install lsb-release

# Install some prerequisites needed by adding GPG public keys
$ sudo apt install gnupg ca-certificates curl

# Import our GPG key. Notice the hyphen at the end of line.
$ curl -sSL https://raw.fastgit.org/Qv2ray/debian/master/pubkey.gpg | sudo apt-key add -

# Add the our official APT repository:
$ echo "deb [arch=amd64] https://raw.fastgit.org/Qv2ray/debian/master/ `lsb_release -cs` main" | sudo tee /etc/apt/sources.list.d/qv2ray-fastgit.list
$ sudo apt update

# You can install Qv2ray from APT now:
$ sudo apt install qv2ray
```
