# Wi-Fi-Linux-Script

This is a very basic python script designed to simplify the Wi-Fi management in Linux through command-line operations. 
Internally it uses the nmcli tool, allowing basic operations like the following.

## Features

- On / Off the Wi-Fi
- Connecting / Disconnecting from a Network
- Check the general Wi-Fi status
- List available networks

## Requirements

`nmcli`: NetworkManager command-line tool. You can install it via package manager: `sudo apt-get install nmcli`

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
Or clone this repo:
```
git clone https://github.com/YonatanAlexander/Wi-Fi-Linux-Script.git
```

## Usage

If you already downloaded the script, so you can use it directly via command-line, something like this: `/Path/to/script/wifi <options>` <br/>
For example:
```
/Path/to/script/wifi on                                    # Enable Wi-Fi
/Path/to/script/wifi list                                  # List available networks
/Path/to/script/wifi connect <SSID>  <Password>            # Connect to a network using it SSID and the password
```

## Configure (Optional)

You can also make additional configures to simplify the use of the script by using one of the following options.

### Creating an alias

You can create an alias to the Wi-Fi script in your shell's configuration file (e.g., `.bashrc`, `.zshrc`, etc.) and simplify the execution through command-line.
For example, if you're using `zsh`, you can add the following to your `.zshrc`: 
```
alias wifi="/Path/to/script/wifi"  # Create the 'wifi` alias for the script
```
Apply the changes:
```
source ~/.zshrc
```
Now you can execute the script by simply typing `wifi <options>`

### Installing the Script to a System-Wide Location

For convenience, you can move or copy the script to `~/.local/bin` so that it can be executed from any location in your terminal. <br/>
For that.
```
cp /path/to/script/wifi ~/.local/bin/wifi
```
or
```
cp /path/to/script/wifi ~/.local/bin/wifi
```

Ensure `~/.local/bin` is in your `PATH`. For that, add the following line to your shell's configuration file: 
```
export PATH="$HOME/.local/bin:$PATH"
```
And apply the changes:

```
source ~/.yourShellConfigFile
```

Now you can execute the script by simply typing `wifi <options>`

## Help

Anyways you can execute `wifi -h` or `wifi --help` to see the help
