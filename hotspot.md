# Create a Wi-Fi hotspot by using `linux-wifi-hotspot`

### Installation
```sh
paru -S linux-wifi-hotspot
```

# Important
If you want to serve hotspot and connect to Wi-Fi using one adapter you have to use same channel (and frequency) for both. 
To see channel of the connected Wi-Fi network: 
```sh
iw dev wlan0 info
```
* `wlan0` - name of adapter.
