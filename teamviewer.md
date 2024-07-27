# TeamViewer on wayland

```sh
# install
paru -S teamviewer

# start and enable daemon
systemctl start teamviewerd.service 
systemctl enable teamviewerd.service

# run
QT_QPA_PLATFORM="" teamviewer 
```
