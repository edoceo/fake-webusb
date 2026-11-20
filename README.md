# Fake WebUSB

This project runs only on Linux.
It uses some scripts to create a fake USB device that is has WebUSB Support, a WebUSB Gadget.

## Create Device

You can use the shell script `webusb-device-create.sh`.
Read it to see what's happening, I have minimal error checking.


## Run a Device Bridge.

This is for devices that are **NOT** natively supports WebUSB.
You can run the python script `webusb-device-bridge.py` to bridge them.

That will map a standard USB device into the WebUSB Space.

```shell
./webusb-device-bridge.py /dev/ttyUSB4
```
