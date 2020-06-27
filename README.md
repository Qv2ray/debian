# Qv2ray Debian Repository
This project is a Debian repository hosted on Github pages.
## Usage
```bash
$ curl -sS https://qv2ray.github.io/debian/pubkey.gpg | sudo apt-key add -
$ echo "deb https://qv2ray.github.io/debian/ stable main" | sudo tee /etc/apt/sources.list.d/qv2ray.list
# echo "deb https://qv2ray.github.io/debian/ unstable main" | sudo tee /etc/apt/sources.list.d/qv2ray.list (for debian testing/unstable and Ubuntu 20.10+)
```
