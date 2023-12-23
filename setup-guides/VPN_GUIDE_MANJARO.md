# VPN Guide for Manjaro(arch-based)

> - As of writing these instructions, I had kernel version "6.1.68-1-MANJARO".
> - Whenever you are asked for IIIT username and passwords during this procedure, you are to enter your LDAP credentials (the one you use to login at https://courses.iiit.ac.in/)

## Pre-requisites

Install openvpn on your system if you don't have it already. If I have some time to spare, I prefer to use

```bash
sudo yay -Syu openvpn
```

this will install openvpn along with any other updates pending. Otherwise, simply use

```bash
sudo yay -S openvpn
```

You can use other package managers too like pacman or pamac or flatpak.

## Step-by-Step instructions to download and setup the VPN

1. Open your web browser and visit [https://vpn.iiit.ac.in/](https://vpn.iiit.ac.in/).
2. Navigate to the **Instructions for Linux** section.
3. Locate and download the configuration file named **ubuntu.ovpn** by clicking the provided link at the top. Please note that even though it mentions Ubuntu, this is the correct file for all users. You will then be prompted to enter your username and password in order to download the file.
4. Once the file is downloaded, access your system's settings and go to **Settings --> Network --> VPN**. Create a new connection, and when prompted for the VPN type, choose the last option labeled **Import from file**.
5. When prompted to select a file, choose the recently downloaded **ubuntu.ovpn** file.
6. After selecting the file, the configuration details will be automatically populated. Simply enter your username (your email address) and password when prompted.
7. Voila! You're good to go. Just toggle the switch as needed.
