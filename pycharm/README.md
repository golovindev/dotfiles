# PyCharm Configuration

This directory contains configuration files for PyCharm, including custom
color schemes and UI theme settings.


## Credits & Acknowledgements
The **Pustota** editor color scheme (`Pustota-color-theme`)
included here is originally developed and
designed by [**Nikita Sobolev**](https://github.com/sobolevn).
All rights to the theme belong to him.

You can find the original project here:
[https://github.com/pustota-theme/pustota](https://github.com/pustota-theme/pustota).
Please note that the version included in these dotfiles is merely a rather
mediocre manual port to PyCharm, created solely for personal convenience.


## Important Note on UI Themes
While the editor color scheme (`Pustota-color-theme`) is included here and
will be applied automatically, the **Dracula Pitch Black Theme** cannot be
fully automated just by copying these dotfiles.

The Dracula theme is a third-party plugin from the JetBrains Marketplace.
The configuration file (`options/laf.xml`) tells PyCharm to use this theme,
but it **does not install the plugin itself**.


### How to get it working:
1. Open PyCharm after running the dotfiles installation.
2. The IDE will likely default to the standard Dark theme
(Darcula or New UI Dark) because the Dracula Pitch Black plugin is missing.
3. Go to **Settings/Preferences -> Plugins -> Marketplace**.
4. Search for and install the **Dracula Pitch Black** plugin.
5. Restart PyCharm.

Once restarted, PyCharm will read the `laf.xml` file provided by these
dotfiles and automatically switch to the Dracula theme.


*Note: Automatically installing PyCharm plugins via CLI scripts is often
fragile and depends heavily on how PyCharm was installed
(JetBrains Toolbox, Homebrew, standalone, etc.), which is why manual
installation of the plugin is recommended.*
