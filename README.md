# Intruder Detection System for Farms 🛡️🚜

This project implements an **Intruder Detection System** for farms using a **PIR Sensor** for intrusion detection and **Pushbullet** for real-time push notifications. The system is built on a **Raspberry Pi**, making it cost-effective and scalable for agricultural environments.

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Hardware Requirements](#hardware-requirements)
- [Software Requirements](#software-requirements)
- [Setup and Installation](#setup-and-installation)
  - [1. Install Raspbian OS](#1-install-raspbian-os)
  - [2. Create a Python Virtual Environment](#2-create-a-python-virtual-environment)
  - [3. Setup Pushbullet](#3-setup-pushbullet)
  - [4. Connect the PIR Sensor](#4-connect-the-pir-sensor)
  - [5. Clone the Repository](#5-clone-the-repository)
  - [6. Configure the Script](#6-configure-the-script)
  - [7. Run the System](#7-run-the-system)
- [How It Works](#how-it-works)
- [Future Enhancements](#future-enhancements)
- [License](#license)
- [Contributions](#contributions)

---

## Overview
Farmers often face issues with trespassers or animals damaging crops. This system uses a **Passive Infrared (PIR) sensor** to detect movement and sends instant **push notifications** to the farmer’s smartphone using **Pushbullet**, enabling timely action against intrusions.

---

## Features
- **Motion Detection**: Detects movement using the PIR sensor.
- **Real-Time Alerts**: Sends push notifications via Pushbullet to notify the user of any detected intrusion.
- **User-Friendly**: Simple setup and easy-to-use notifications.
- **Low Power Consumption**: Operates efficiently on Raspberry Pi.

---

## Hardware Requirements
- **Raspberry Pi** (any model with GPIO support)
- **PIR Motion Sensor** (e.g., HC-SR501)
- **Wi-Fi or Ethernet** for Raspberry Pi connectivity
- **5V Power Supply** for Raspberry Pi
- Optional: Protective casing for outdoor installation

---

## Software Requirements
- **Raspbian OS** (or any Raspberry Pi-compatible Linux distribution)
- **Python 3.7+**
- Python packages:
  - `RPi.GPIO`
  - `pushbullet.py`

---

## Setup and Installation

### 1. Install Raspbian OS
1. Download and install **Raspberry Pi Imager** to flash Raspbian OS onto an SD card.
2. Boot your Raspberry Pi and connect it to the internet.

---

### 2. Create a Python Virtual Environment
1. Install the `virtualenv` package:
   ```bash
   sudo apt-get install python3-venv
