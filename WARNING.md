# UniqueStudio-2018AutumnESD

# **WARNING**

**Please read this before you start to flash your esp8266**

# SPI Flash Modes

The ESP8266 & ESP32 support four different SPI flash access modes: DIO, DOUT, QIO & QOUT.

You could change it via _make menuconfig_ -> _Serial flasher config_ -> _Flash SPI mode_

Because of some chips has special issue. If you have some problem in flashing, you are supposed to change the Flash SPI mode (try for all).

