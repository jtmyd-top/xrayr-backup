# XrayR Backup

This directory backs up the XrayR installer and runtime helper files used on the server.

Included:
- `alist/newxrayr-install.sh`: public AList installer script.
- `runtime/XrayR-manager.sh`: installed XrayR management script, if present.
- `runtime/XrayR.service`: installed systemd service file, if present.
- `defaults/`: default files shipped with the installed XrayR package.

Not included:
- `/etc/XrayR/config.yml` from the running server, because it may contain panel URLs, node IDs, keys, or other secrets.
- XrayR binary and large `.dat` rule files.

Current public install command:

```bash
bash <(curl -Ls https://raw.githubusercontent.com/jtmyd-top/xrayr-backup/main/alist/newxrayr-install.sh)
```
