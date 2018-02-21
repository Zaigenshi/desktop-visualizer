# desktop-visualizer
Linux Desktop Music visualizer made with SFML

![](visualizer.gif)

Based on [Cava](https://github.com/karlstav/cava), [Conky](https://github.com/brndnmtthws/conky), and [TheBITLINK's](https://github.com/TheBITLINK/desktop-visualizer) desktop-visualizer.

# Dependencies

 - PulseAudio
 - fftw3
 - SFML

# Building and installing

```
$ mkdir build && cd build
$ cmake ..
$ make
$ sudo make install
```

# Configuration

The configuration file is located in ```~/.config/deskvis/config.ini```

# Automatic Startup

To automatically start the visualizer on login add a deskvis.desktop containing the following:

```
[Desktop Entry]
Name=deskvis
Exec=/usr/local/bin/deskvis
Terminal=false
Type=Application
X-GNOME-Autostart-enabled=true 
```

to: ```~/.config/autostart/```

