# WSJTX Transceiver Interface
A Python server to interface Arduino transmitter with WSJTX

This Python program connects to WSJTX using the UDP interface and retrieves TX status as mode and frequency to configure the Arduino transmitter.

The current TX message is also extracted and then encoded and loaded into the Arduino.

### Notes:

* The TX messsage is not present in current version of WSJTx but will be.
To have this feature now, a patch can be found in this thread.
        https://wsjtx.groups.io/g/main/message/18702
* The script uses a modified version of the Python class to decode UDP packets from WSJTX:
        https://github.com/rstagers/WSJT-X
* Weakmon: Used to convert callsigns, grid locators and signal reports into the FT8 or FT4 channel symbols. 
        https://github.com/rtmrtmrtmrtm/weakmon

