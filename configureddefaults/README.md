# Configured Defaults

This whole directory servers as a synchronized mirror of `.minecraft`. Every sub-directory and / or file placed within will be copied to the main `.minecraft` directory during game launch if the directory / file is not already present.
There is no way of overriding an existing file, a copy will only be made when the target destination is empty.

Please note that due to the way Minecraft handles `options.txt` specifically it is sufficient to include only the options you want to set a preset for. All missing options will be filled in using their internal defaults when the file is read by the game.

Examples:
- `.minecraft/configureddefaults/options.txt` will be copied to `.minecraft/options.txt` if not already present
- `.minecraft/configureddefaults/config/jei/jei.toml` will be copied to `.minecraft/config/jei/jei.toml` if not already present

Note that this `README.md` file is excluded from being copied to `.minecraft`.

Änderungen:

options.txt:
- wenn nur die änderungen in die datei geschrieben werden und es auch key bind änderungen gibt, werden die änderungen nicht übernommen 
- fullscreen on
- gamma auf 1.0
- guiScale auf 3
- shader keybinds aus (reload, toggle und open menu - das ist sonst auf "R", "K" und "O")
