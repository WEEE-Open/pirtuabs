# pirtuabs
A simply script that play a buzzer sound when pc reach login screen after boot. Useful for who work with a machine without a monitor.

`beep` is required!

for Arch:

    $ sudo pacman -S beep
      
for Debian:

    $ sudo apt install beep

for Fedora:

    $ sudo dnf install beep
    
1. copy `pirtuab_sound` file on wherever you want directory (i suggest `~/.local/share/sounds/`)
2. copy `pirtuabs.service` into `/etc/systemd/system/`
3. open with your editor `pirtuabs.service` and add `pirtuabs_sound` path to `ExecStart=path/to/pirtuabs_sound`
4. eneble with `$ systemctl enable pirtuabs.service`
5. restart

Edit `pirtuab_sound` like your want!!!!!!!!
