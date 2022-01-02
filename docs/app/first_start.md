# Unpacking Beaglebone

Beaglebone shortcut is BBB.

1. Connect BeagleBone to BoneIO and plug-in network cable.
2. Find out BBB in your network.
3. Connect via ssh with username debian. Default password is temppwd.
4. Change default password by running

```bash
passwd
```

5. Update your BBB (click Yes if needed to perform upgrade). First upgrade can take ~30mins.

```bash
sudo apt-get update && sudo apt-get dist-upgrade
```

```bash
reboot
```

6. Disable unnecessary services (if you need some you can just avoid disabling it).

```bash
sudo systemctl disable bonescript-autorun nginx wpa_supplicant bonescript.socket cloud9.socket cryptsetup.target
```

```bash
reboot
```

7. Install dependencies

```bash
sudo apt-get install libopenjp2-7-dev libatlas-base-dev python3-venv
```
