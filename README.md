# ESP32 WiFi and Bluetooth Blocker

This is a Python script designed to demonstrate how an ESP32 module can be used as a WiFi and Bluetooth blocker. Please note that this is just a demonstration - I take no responsibility for any misuse of this code!

## Requirements

- Kali Linux or Debian-based operating system
- Computer with wireless network interface card (NIC) supporting monitor mode and packet injection
- ESP32 module
- USB cable or similar connection method
- Python 2.7

## Installation

1. Install required packages:
apt-get update && apt-get dist-upgrade -y apt-get install git aircrack-ng bluez-utils python-bluez python2.7


2. Clone this repository and change into the directory:
git clone https://github.com/J-CK-L/Wi-FiInterceptor cd wifi-bluetooth-blocker


3. Install required Python libraries:
pip install bluepy


4. Connect your ESP32 module to your computer via USB cable or similar connection method

## Usage

1. Run the following command in your terminal:

Replace "yourusername" with your actual GitHub username.
python2.7 wifi_bluetooth_blocker.py


This will start sending deauthentication packets to all devices connected to every available WiFi network within range of your wireless adapter.

## Parameters

You can customize the script's behavior using these optional parameters:

- `-i <interface>`: Specify which wireless interface to use (e.g., `wlan0mon`)
- `-d <delay>`: Set delay between scans in seconds (default is 60)
- `-v`: Enable verbose output
- `--help`: Display this help message

## Issues and Troubleshooting

1. If you encounter any errors or issues, please check that all required packages are installed correctly.

2. Make sure your wireless adapter supports monitor mode and packet injection.

3. Ensure you have root privileges when running the script.

4. If you experience connectivity problems after running the script, try resetting your router or turning off your WiFi adapter and re-enabling it.

## Future Updates

I plan to add more features and improvements to this project in the future, such as:

- Support for different types of attacks (e.g., WPS attack, dictionary attack)
- Better error handling and logging
- More detailed statistics about blocked devices
- Cross-platform support

Stay tuned for updates!

For more information about working with ESP32 modules and their capabilities, check out [this guide](https