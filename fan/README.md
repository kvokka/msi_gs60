Add to `/etc/modprobe.d/bbswitch.conf`

```
options bbswitch load_state=0 unload_state=1
```

in file `/etc/systemd/logind.conf` change `HandleLidSwitchDocked=ignore` to `HandleLidSwitchDocked=suspend`

Add to `sudo crontab -e`

```
@reboot sleep 60 && /sbin/modprobe bbswitch
```

copy `service/silent_fan.service` to `/etc/systemd/system/silent_fan.service`

run `sudo systemctl enable silent_fan.service`

copy `fan` to `/usr/fan`

reboot

run `powertop` and check `Tunables` tab. Add configs to `powertop_fixes` if required (the specs may vary
becouse of laptop config or bios version or external devices connextion or etc.)
