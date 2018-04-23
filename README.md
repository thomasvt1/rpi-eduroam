# rpi-eduroam


## To create hash
echo -n 'password' | iconv -t utf16le | openssl md4 > hash.txt

## Locations
/etc/wpa_supplicant/wpa_supplicant.conf

/etc/network/interfaces
