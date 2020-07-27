# Qv2ray Debian Repository
This project is a Debian repository hosted on GitHub Pages.
## Usage
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
