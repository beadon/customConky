# customConky
A custom conky configuration for Ubuntu systems

For ultra-compact viewing consider using the always wonderful artwiz fonts.  Maintained here : https://github.com/whitelynx/artwiz-fonts-wl

Of course, further configuration notes are available here:
https://wiki.archlinux.org/title/Conky


To start on Ubuntu Desktop start, move conky.desktop to an autostart location

```
mv conky.desktop ~/.config/autostart/conky.desktop
```

Deploy to a user locally managed location

```
mv .conky ~
```

Symlink the chosen config file to use
```
cd ~
ln -s ~/.conky/beadonConky/minimalist-bw .conkyrc
```

If you'd like to start this without logging out / logging in again, start it from command line, since this is now registered in gtk, the path to the desktop file is not required, it will by found by the launcher if the .desktop file in in the autostart location for the current user
```
gtk-launch conky.desktop
```

## Note

There is a network lookup to http://ipecho.net/plain
Feel free to remove this if you don't want your machine reaching out to the site to get the public IP.
The current config reaches out every 3600 seconds, so it's relatively infrequent (once an hour)


## Testing
Last tested with conky 1.19.6 compiled 2024-04-01 for Linux x86_64


## Ideas

Check out some of the setups over at [ConkyPorn](https://www.reddit.com/r/Conkyporn/)
