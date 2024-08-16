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

Download the Wi-Fi script. You can do it using one of the folowing commands:
- Using `curl`:
```
curl -O https://raw.githubusercontent.com/YonatanAlexander/Wi-Fi-Linux-Script/main/wifi
```

- Using `wget`:
```
wget https://raw.githubusercontent.com/YonatanAlexander/Wi-Fi-Linux-Script/main/wifi
```

## Configure

To configure the script for the execution, you have the following options.

### Execute the script directly (Easiest)

If you already downloaded the script, so you can use it directly vía command-line, something like this: `~/Path/to/script/wifi <args>` <br/>
For example:
```
/Path/to/script/wifi on                                    # Enable Wi-Fi
/Path/to/script/wifi list                                  # List available networks
/Path/to/script/wifi connect <SSID>  <Password>            # Connect to a network using it SSID and the password 
```

### Creating an alias (Optional)

You can create an alias to the Wi-Fi script in your shell's configuration file (e.g., `.bashrc`, `.zshrc`, etc.) and simplify the execution through command-line.
For example, if you're using `zsh`, so you can add something like the following to your `.zshrc`: 
```
alias wifi="/Path/to/script/wifi"  # Create the 'wifi` alias for the script
```
Apply the changes:
```
source ~/.zshrc
```

### Installing the Script to a System-Wide Location (Optional)
For convenience, you can move or copy the script to `~/.local/bin` so that it can be executed from any location in your terminal.
```
cp /path/to/script/wifi ~/.local/bin/wifi
```
or
```
cp /path/to/script/wifi ~/.local/bin/wifi
```

Ensure `~/.local/bin` is in your `PATH`. <br/>
For it, add the following line to your shell's configuration file: `export PATH="$HOME/.local/bin:$PATH"` and apply the changes:

## Help

Anyways you can execute the script with the `-h` or `--help` option for see the main menu

