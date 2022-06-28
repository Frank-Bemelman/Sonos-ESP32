# SonosUPnP


Fork From original Sonos library : https://github.com/javos65/Sonos-ESP32

Issue - Sonos Play 5 was almost never found, or accidently as a side effect of Windows PC also regularly sending out SSDP requests. 
Improved the scan/search. The original code would often miss certain Sonos devices or add them multiple times to the same short list of max 4 devices.
Changes made to uint8_t SonosUPnP::CheckUPnP(IPAddress *List,int Listsize) and removal of SonosUPnP::readback_IP(IPAddress *IPa,char* buf,char pointer,char bufsize)
Now finds all Sonos products each and every time and adds them only once to the list. 



