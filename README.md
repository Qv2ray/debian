# Qv2ray Debian Repository

This project is a Debian repository hosted on GitHub Pages.

## Supported Distributions

- Debian Buster
- Debian Bullseye/Sid
- Ubuntu 20.04 (Focal Fossa)
- Ubuntu 20.10 (Groovy Gorilla)

## Configuration

### Official Repository

NOTE: Replace `$YOUR_DISTRIBUTION` with your distribution code (`stable`/`unstable`/`focal`/`groovy`...) below.

```bash
# Install some prerequisites needed by adding GPG public keys
$ sudo apt-get install gnupg ca-certificates curl

# Import our GPG key. Notice the hyphen at the end of line.
$ curl -sSL https://qv2ray.net/debian/pubkey.gpg | sudo apt-key add -

# Add the our official APT repository:
$ echo "deb [arch=amd64] https://qv2ray.net/debian/ $YOUR_DISTRIBUTION main" | sudo tee /etc/apt/sources.list.d/qv2ray.list

# To update the APT index:
$ sudo apt-get update

# You can install Qv2ray from APT now:
$ sudo apt-get install qv2ray
```

### FastGit UK Mirror (in case `qv2ray.github.io` is blocked)

[![fastgit.org](https://img.shields.io/badge/powered--by-fastgit.org-blue)](https://fastgit.org/)

NOTE: Replace `$YOUR_DISTRIBUTION` with your distribution code (`stable`/`unstable`/`focal`/`groovy`...) below.

```bash
# Install some prerequisites needed by adding GPG public keys
$ sudo apt-get install gnupg ca-certificates curl

# Import our GPG key. Notice the hyphen at the end of line.
$ curl -sSL https://raw.fastgit.org/Qv2ray/debian/master/pubkey.gpg | sudo apt-key add -

# Add the our official APT repository:
$ echo "deb [arch=amd64] https://raw.fastgit.org/Qv2ray/debian/master/ $YOUR_DISTRIBUTION main" | sudo tee /etc/apt/sources.list.d/qv2ray-fastgit.list
$ sudo apt-get update

# You can install Qv2ray from APT now:
$ sudo apt-get install qv2ray
```
