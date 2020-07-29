# Qv2ray Debian Repository
This project is a Debian repository hosted on GitHub Pages.

## Configuration

### Official Repository

```bash
# Install some prerequisites needed by adding GPG public keys
$ sudo apt-get install gnupg ca-certificates curl

# Import our GPG key. Notice the hyphen at the end of line.
$ curl -sSL https://qv2ray.github.io/debian/pubkey.gpg | sudo apt-key add -

# Add the our official APT repository:
$ echo "deb https://qv2ray.github.io/debian/ stable main" | sudo tee /etc/apt/sources.list.d/qv2ray.list
# echo "deb https://qv2ray.github.io/debian/ unstable main" | sudo tee /etc/apt/sources.list.d/qv2ray.list (for debian testing/unstable and Ubuntu 20.10+)

# To update the APT index:
$ sudo apt-get update

# You can install Qv2ray from APT now:
$ sudo apt-get install qv2ray
```

### FastGit Mirror (in case `qv2ray.github.io` is blocked)
[![fastgit.org](https://img.shields.io/badge/powered--by-fastgit.org-blue)](https://fastgit.org/)


```bash
# Install some prerequisites needed by adding GPG public keys
$ sudo apt-get install gnupg ca-certificates curl

# Import our GPG key. Notice the hyphen at the end of line.
$ curl -sSL https://raw.fastgit.org/Qv2ray/debian/master/pubkey.gpg | sudo apt-key add -

# Add the our official APT repository:
$ echo "deb https://raw.fastgit.org/Qv2ray/debian/master/ stable main" | sudo tee /etc/apt/sources.list.d/qv2ray.list
# echo "deb https://raw.fastgit.org/Qv2ray/debian/master/ unstable main" | sudo tee /etc/apt/sources.list.d/qv2ray.list (for debian testing/unstable and Ubuntu 20.10+)

# To update the APT index:
$ sudo apt-get update

# You can install Qv2ray from APT now:
$ sudo apt-get install qv2ray
```
