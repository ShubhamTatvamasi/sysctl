# sysctl

List all kernel parameters:
```bash
sudo sysctl -a
```

Update kernel parameters:
```bash
sudo vim /etc/sysctl.conf
```
> `reboot` your system after changes.

List all the parameters from `/etc/sysctl.conf` file:
```bash
sudo sysctl -p
```
