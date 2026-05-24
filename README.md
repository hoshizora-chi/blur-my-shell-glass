# GNOME Shell Extension - Blur my Shell Glass
Please refer to the original blur my shell extension repository for more information.
### Development

To install the extension from source:

```sh
git clone https://github.com/hoshizora-chi/blur-my-shell-glass
cd blur-my-shell
make install
```

You will then need to reload GNOME shell, for example by login out and in again, or under Xorg, `alt+f2` and type `r`.

To debug the extension, you can use Looking Glass (`alt+f2`, type `lg`); I stored the extension object in `global.blur_my_shell`.

To see the extension logs, you can use:

```sh
# for debug logs (when Debug is activated in preferences)
sudo journalctl /usr/bin/gnome-shell | grep Blur my Shell

# for crash logs in GNOME shell
sudo journalctl /usr/bin/gnome-shell | grep blur-my-shell

# for crash logs in the extension's preferences
sudo journalctl /usr/bin/gjs | grep blur-my-shell
```

Just don't hesitate to open issues and pull requests, and sorry if I take some time to answer!

## License

This program is distributed under the terms of the GNU General Public License, version 3 or later.
