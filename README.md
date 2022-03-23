# Table of Contents
   * [Home Assistant configuration](#home-assistant-configuration)
      * [Z-Wave](#z-wave)
      * [The key software](#the-key-software)

# Home Assistant configuration
This is my primary [Home Assistant](https://home-assistant.io/) Core configuration, This instance is running core-2021.6.6 (Python Version 3.8.9) on a Raspberry Pi 4 (8GB).

## Z-Wave
My Z-Wave stack runs on a Raspberry Pi 3, using the old All in One installer (effectively a [manual install like this](https://blog.ceard.tech/2017/12/installing-home-assistant-in-virtual.html), on a 16 GB card, that I've [upgraded to Python 3.6](https://blog.ceard.tech/2017/12/upgrading-python-virtual-environment.html). I use a [Razberry](https://razberry.z-wave.me/) board for Z-Wave control. The configuration for that instance can be [found here](https://github.com/DubhAd/HomeAssistant-ZWave).

To limit the risk brought by SD card corruption (a known risk with Pi3) I store the Home Assistant database on a USB stick, and use a multi-port USB charger with sufficient power for all ports, but have left one unused. The power cables are short, and high quality, to minimise issues with voltage drop. Of course, I also take [many different backups](https://blog.ceard.tech/2017/10/backing-up-home-assistant.html) to reduce the risk of losing anything.


## The key software

* [Home Assistant](https://home-assistant.io/)
* [nginx](https://nginx.org/en/) to provide remote access, in conjunction with [Let's Encrypt VIA DuckDNS](https://github.com/home-assistant/hassio-addons/tree/master/duckdns)
* MariaDB for the database
