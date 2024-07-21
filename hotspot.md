# Create a Wi-Fi hotspot on Linux using `nmcli`

### Setup
```sh
nmcli con add type wifi ifname wlan0 con-name Hostspot autoconnect yes ssid 17ach6h
nmcli con modify Hostspot 802-11-wireless.mode ap 802-11-wireless.band bg ipv4.method shared
nmcli con modify Hostspot wifi-sec.key-mgmt wpa-psk
nmcli con modify Hostspot wifi-sec.psk "12345678"
```

### Change Password
```sh
nmcli con modify Hostspot wifi-sec.psk "12345678"
```

### Run
```sh
nmcli con up Hostspot
```

# Note
If after reboot `nmcli con up Hotspot` doesn't work

Use this command instead to start Hotspot

```sh
UUID=$(grep uuid /etc/NetworkManager/system-connections/Hotspot | cut -d= -f2)
nmcli con up uuid $UUID
```
