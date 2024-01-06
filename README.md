# sysctl

List all kernel parameters:
```bash
sudo sysctl -a
```

Update kernel parameters:
```bash
sudo vim /etc/sysctl.conf
```

Add this to the `sysctl.conf` file for Proxmox VM:
```
fs.inotify.max_user_instances=512
```

Apply changes to system:
```bash
sudo sysctl --system
```

Verify value:
```bash
sudo sysctl fs.inotify.max_user_instances
```

List all the parameters from `/etc/sysctl.conf` file:
```bash
sudo sysctl -p
```

Live parameters can be changed by updating these files:
```bash
ls /proc/sys
```
