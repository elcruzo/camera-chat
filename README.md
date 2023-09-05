# Camera Chat Application

This repository contains the code for the a LiveStream Chat Project featuring Real-Time Video Communication.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [Contributions](#contributions)
- [License](#license)

## Introduction

This Camera Chat Application is a simple Python-based project that allows users to establish real-time video communication between two devices on a local network. It uses the VidStream library for video streaming and communication.

## Features

- Real-time video streaming from a camera to a remote device.
- Two-way communication between a camera device and a remote viewer.
- Easy setup for local network communication.

## Requirements

To use this script, you need the following:

- Python 3.6 or higher installed on both the camera and remote devices.
- The `vidstream` library (see steps to install it below)
- The `time` module (usually included in Python standard library)
- The `threading` module (usually included in Python standard library)

## Installation

1. Clone this repository to to both the camera and remote devices or download it as a ZIP file:

   ```bash
   git clone https://github.com/elcruzo/camera-chat.git
   ```
2. Navigate to the project directory:

   ```bash
   cd camera-chat
   ```
3. Ensure you have Python 3.x installed. You can check by running:

   ```bash
   python3 --version
   ```
4. Install the Vidstream Library.

   ```bash
   pip install vidstream
   ```

   If Python is not installed, you can download it from the official [Python website](https://www.python.org/downloads/).

5. Update the IP addresses and port numbers in the `index.py` file to match your network setup. Modify the following lines to match your network setup:

   ```bash
    receiving = StreamingServer('192.168.0.68', 9999)
    sending = CameraClient('192.168.0.172', 9999)
   ```
6. Replace the IP addresses and port numbers with the appropriate values for your devices.


## Usage

1. Start the server on the receiving device by running the following command:
   ```bash
   python index.py
   ```
2. Wait for a moment to allow the server to initialize.
3. Start the client on the sending device by running the following command:
   ```bash
   python index.py
   ```
4. The video stream should now start, and you can see live video from the sending device on the receiving device.
5. To end the chat, simply press Enter (or any key) in the terminal where the server is running. This will stop the video stream on both devices.

## Contributions

Contributions to this repository are welcome! If you have any improvements or feature suggestions, feel free to fork this repository, make your changes, and submit a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Have fun exploring my Camera Chat Application! If you have any questions or run into issues, don't hesitate to ask for help.

   
