# AmneziaWG installer

**This project is a bash script that aims to setup a [AmneziaWG](https://docs.amnezia.org/ru/documentation/amnezia-wg/) VPN on a Linux server, as easily as possible!**

## Requirements

Supported distributions:

- AlmaLinux >= 9
- Debian >= 11
- Rocky Linux >= 9
- Ubuntu >= 22.04

others can work but not tested

2Gb of free space is required for temporary files.

## Usage

Before installation it is strictly recommended to upgrade your system to the latest available version and perform the reboot afterwards.

Use curl or wget to download the script:
```bash
curl -O https://raw.githubusercontent.com/Varckin/amneziawg-install/main/amneziawg-install.sh
```
```bash
wget https://raw.githubusercontent.com/Varckin/amneziawg-install/main/amneziawg-install.sh
```

Set permissions:
```bash
chmod +x amneziawg-install.sh
```

And execute:
```bash
./amneziawg-install.sh
```

Answer the questions asked by the script and it will take care of the rest.

It will install AmneziaWG (kernel module and tools) on the server, configure it, create a systemd service and a client configuration file.

Run the script again to add or remove clients!
