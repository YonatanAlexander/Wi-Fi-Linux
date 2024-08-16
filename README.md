# Wi-Fi-Linux-Script

This is a very basic python script designed to simplify the Wi-Fi management in Linux through command-line operations. 
Internally it uses the nmcli tool, allowing basic operations like the following.

## Features
- On / Off the Wi-Fi
- Connecting / Disconnecting from a Network
- Check the general Wi-Fi status
- List available networks

## Requirements
- `nmcli`: NetworkManager command-line tool. You can install it via package manager: `sudo apt-get install nmcli`

## Installation
Download the wifi script. You can do it using one of the folowing commands:
- Using `curl`
```bash
curl -O https://raw.githubusercontent.com/YonatanAlexander/Wi-Fi-script-for-Linux/main/wifi
```

- Using `wget`
```bash
wget https://raw.githubusercontent.com/YonatanAlexander/Wi-Fi-script-for-Linux/main/wifi
```

## Usage

Use this script is very easy, you can do it in several ways
1. Execute the script directly:
If you already downloaded the script, so you can use it directly vía command-line, something like this: `~/Path/to/script/wifi <args>`
For example:
```
~/Path/to/script/wifi on                                    # Enable Wi-Fi
~/Path/to/script/wifi list                                  # List available networks
~/Path/to/script/wifi connect <SSID>  <Password>            # Connect to a network using it SSID and the password 
```




