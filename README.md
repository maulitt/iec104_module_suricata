# iec104_module_suricata
Trying to write iec104 module for suricata
- app-layer-iec104.c \
In this file there is a function ProbingParse which returns ALPROTO_IEC104 if it detected our protocol packet and ALPROTO_UNKNOWN otherwise. \
Now (17.11.21) I'm checking:
  1. starting byte (if it equals to 0x68)
  2. if the type of the packet is S or U (which have fixed length) the length should be equal to 4.  

