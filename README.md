# Table of Contents
   * [Home Assistant configuration](#home-assistant-configuration)
      * [Z-Wave](#z-wave)
      * [The key software](#the-key-software)

# Home Assistant configuration
This is my primary [Home Assistant](https://home-assistant.io/) Core configuration, This instance is running core-2021.6.6 (Python Version 3.8.9) on a Raspberry Pi 4 (8GB).

## Z-Wave
My Z-Wave stack runs on a Raspberry Pi 4

## The key software

* [Home Assistant](https://home-assistant.io/)
* [nginx](https://nginx.org/en/) to provide remote access, in conjunction with [Let's Encrypt VIA DuckDNS](https://github.com/home-assistant/hassio-addons/tree/master/duckdns)
* MariaDB for the database
