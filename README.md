# showSSID

Generates continuous probe requests to identify hidden SSIDs

## Demo
```
python showSSID.py -i wlan1mon -f ssids -d .1 -c 5
[*] 802.11 Probe Request: SSID=[ssid1], count=5
[*] 802.11 Probe Request: SSID=[ssid2], count=5
[*] 802.11 Probe Request: SSID=[ssid3], count=5
[*] 802.11 Probe Request: SSID=[ssid4], count=5
[*] 802.11 Probe Request: SSID=[ssid5], count=5
[*] 802.11 Probe Request: SSID=[ssid6], count=5
[*] 802.11 Probe Request: SSID=[ssid7], count=5
```

## Usage
```
python showSSID.py -h
usage: showSSID.py [-h] -i interface [-d delay] [-c count] [-m mac]
                   (-s ssid | -f file)

optional arguments:
  -h, --help            show this help message and exit
  -i interface, --interface interface
                        wireless interface to use
  -d delay, --delay delay
                        seconds to delay (default=.3)
  -c count, --count count
                        number of packets to send per SSID per iteration
                        (default=10)
  -m mac, --mac mac     last 3 octets of source mac address (default=00:11:22)
  -s ssid, --ssid ssid  ssid name
  -f file, --file file  ssid file
```

## Credits
* [Joey Belans](https://github.com/joeybelans)