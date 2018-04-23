# rpi-eduroam


## To create hash
```
echo -n 'password' | iconv -t utf16le | openssl md4
```

## Locations
```
/etc/wpa_supplicant/wpa_supplicant.conf
```
```
/etc/network/interfaces
```

## Test network
Try this command to see if the network works. If it stops there might be a problem, exciting should be with CTRL+C. The problem will be mentioned before closing.
```
wpa_supplicant -i wlan0 -D wext -c /etc/wpa_supplicant/wpa_supplicant.conf -d
```
