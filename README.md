# Qv2ray Debian Repository

This project is a Debian repository hosted on GitHub Pages.

** Supported Distributions **

- Debian Buster
- Debian Bullseye/Sid
- Ubuntu 20.04 (Focal Fossa)
- Ubuntu 20.10 (Groovy Gorilla)


FastGit Mirror [![fastgit.org](https://img.shields.io/badge/powered--by-fastgit.org-blue)](https://fastgit.org/)

## Debian Configuration

### Add Qv2ray public keys to your system: 

```bash
# Install some prerequisites needed by adding GPG public keys
$ sudo apt-get install gnupg ca-certificates curl

# Import our GPG key. Notice the hyphen at the end of line.
$ curl -sSL https://qv2ray.net/debian/pubkey.gpg | sudo apt-key add -

# you can also import GPG public keys by using FastGit:
# $ curl -sSL https://raw.fastgit.org/Qv2ray/debian/master/pubkey.gpg | sudo apt-key add -
```

### Add the our official APT repository:

```bash
$ echo "deb [arch=amd64] https://qv2ray.net/debian/ stable main" | sudo tee /etc/apt/sources.list.d/qv2ray.list
# If you are using unstable version Debian, you should use this command instead: 
# $ echo "deb [arch=amd64] https://qv2ray.net/debian/ unstable main" | sudo tee /etc/apt/sources.list.d/qv2ray.list

# To update the APT index:
$ sudo apt update

# You can install Qv2ray from APT now:
$ sudo apt install qv2ray
```

### FastGit UK Mirror (in case `qv2ray.github.io` is blocked)

```bash

# Add the our official APT repository:
$ echo "deb [arch=amd64] https://raw.fastgit.org/Qv2ray/debian/master/ stable main" | sudo tee /etc/apt/sources.list.d/qv2ray-fastgit.list
# If you are using unstable version Debian, you should use this command instead: 
# $ echo "deb [arch=amd64] https://raw.fastgit.org/Qv2ray/debian/master/ unstable main" | sudo tee /etc/apt/sources.list.d/qv2ray-fastgit.list

# To update the APT index:
$ sudo apt update

# You can install Qv2ray from APT now:
$ sudo apt install qv2ray
```

## Ubuntu Configuration

### Add Qv2ray public keys to your system: 

```bash
# Install some prerequisites needed by adding GPG public keys
$ sudo apt install curl gnupg2 ca-certificates lsb-release

# Import our GPG key. Notice the hyphen at the end of line.
$ curl -sSL https://qv2ray.net/debian/pubkey.gpg | sudo apt-key add -

# you can also import GPG public keys by using FastGit:
# $ curl -sSL https://raw.fastgit.org/Qv2ray/debian/master/pubkey.gpg | sudo apt-key add -
```

### Add the our official APT repository:

```bash
$ echo "deb [arch=amd64] https://qv2ray.net/debian/ `lsb_releases -cs` main" | sudo tee /etc/apt/sources.list.d/qv2ray.list

# To update the APT index:
$ sudo apt update

# You can install Qv2ray from APT now:
$ sudo apt install qv2ray
```

### FastGit Mirror (in case `qv2ray.github.io` is blocked)

```bash

# Add the our official APT repository:
$ echo "deb [arch=amd64] https://raw.fastgit.org/Qv2ray/debian/master/ `lsb_release` main" | sudo tee /etc/apt/sources.list.d/qv2ray-fastgit.list

# To update the APT index:
$ sudo apt update

# You can install Qv2ray from APT now:
$ sudo apt install qv2ray
```
