# uGet Integrator

Integrate uGet Download Manager with Google Chrome, Chromium, Opera, Vivaldi and Mozilla Firefox.

## Installation

> **NOTE:** uget-integrator is still under development. Please stick with [uget-chrome-wrapper](https://slgobinath.github.io/uget-chrome-wrapper/#installation) until new release.

### Arch

```
yaourt -S uget-chrome-wrapper
```

### Ubuntu & Linux Mint

```
sudo add-apt-repository ppa:slgobinath/uget-chrome-wrapper
sudo apt update
sudo apt install uget-chrome-wrapper
```

### Other Linux

```
sudo pip3 install urllib3
wget https://raw.githubusercontent.com/ugetdm/uget-integrator/master/install/linux/install_uget_integrator.sh
sudo sh install_uget_integrator.sh
```

### Windows

1. Install [Python 3.4 or latest](https://www.python.org/downloads/)
2. Install the latest uGet Download Manager using [Windows installer](https://github.com/ugetdm/uget-windows-installer/releases)
3. Download and install the latest [uget-integrator_x.x.x.x.exe](https://github.com/ugetdm/uget-integrator/releases)

## Known Issues

**Firefox not interrupting downloads**
If the uGet extension does not interrupt downloads in Mozilla Firefox, first ensure that the architecture(`32` bit or `64`bit) of Firefox match with your operating system.
If that does not help, delete `handlers.json` from the following path:

Firefox Stable:
```
~/.mozilla/firefox/mwad0hks.default/handlers.json
```

Firefox Nightly:
```
~/.mozilla/firefox-trunk/mwad0hks.default/handlers.json
```

Where `mwad0hks` is a random string so you may have a different folder name.

If the above solution works but does not persist, solution provided in [#3](https://github.com/ugetdm/uget-integrator/issues/3) may give you a permanent solution.

For more details, please check issues [#43](https://github.com/slgobinath/uget-chrome-wrapper/issues/43) and [#3](https://github.com/ugetdm/uget-integrator/issues/3).

## License

GNU General Public License v3