# Gruvbox Theme for Midnight Commander

A warm, retro-inspired color scheme for Midnight Commander based on the popular Gruvbox theme.


## Features

- **Warm color palette**: Dark brown backgrounds with cream text and orange accents
- **Excellent readability**: High contrast colors designed for comfortable file browsing  
- **Color-coded file types**: Directories, executables, symlinks, and archives are distinctly colored
- **Complete coverage**: Themed panels, editor, viewer, menus, and dialogs
- **256-color support**: Takes advantage of modern terminal color capabilities

## Color Scheme

- **Background**: Dark brown (`color235`)
- **Text**: Light cream (`color223`) 
- **Highlights**: Warm orange (`color214`)
- **Directories**: Green (`color109`)
- **Executables**: Yellow-green (`color142`)
- **Archives**: Orange (`color172`)
- **Links**: Purple (`color175`)

## Installation

### Quick Install

```bash
# Create the skins directory
mkdir -p ~/.local/share/mc/skins/

# Download the skin file
curl -o ~/.local/share/mc/skins/gruvbox.ini https://raw.githubusercontent.com/USERNAME/mc-gruvbox-skin/main/gruvbox.ini

# Configure MC to use the theme
echo "skin=gruvbox" >> ~/.config/mc/ini
```

### Manual Install

1. **Download the skin file**: Save `gruvbox.ini` to your MC skins directory:
   ```bash
   mkdir -p ~/.local/share/mc/skins/
   ```

2. **Copy the skin file**: Place `gruvbox.ini` in the skins directory

3. **Configure Midnight Commander**: Edit your MC configuration file:
   ```bash
   nano ~/.config/mc/ini
   ```
   
   Find the line starting with `skin=` and change it to:
   ```
   skin=gruvbox
   ```
   
   If the line doesn't exist, add it to the `[Midnight-Commander]` section.

4. **Restart MC**: Close and reopen Midnight Commander to see the new theme.

## Alternative Installation Locations

If the above doesn't work, try placing the skin file in one of these locations:

- `~/.config/mc/skins/gruvbox.ini`
- `/usr/share/mc/skins/gruvbox.ini` (system-wide, requires sudo)

## Requirements

- Midnight Commander 4.8.0 or later
- Terminal with 256-color support
- Modern terminal emulator (iTerm2, Alacritty, Kitty, etc.)

## Troubleshooting

### Theme not loading
1. Verify the skin file is in the correct location
2. Check that your MC config has `skin=gruvbox`
3. Ensure your terminal supports 256 colors:
   ```bash
   echo $TERM
   ```
   Should show something like `xterm-256color`

### Colors look wrong
- Make sure your terminal emulator supports 256 colors
- Try different terminal color profiles if colors appear washed out

## Contributing

Found a bug or want to improve the theme? 

1. Fork this repository
2. Make your changes
3. Test with different file types
4. Submit a pull request

## License

MIT License - feel free to modify and share!

## Credits

- Inspired by the [Gruvbox](https://github.com/morhetz/gruvbox) color scheme by Pavel Pertsev
- Created for the Midnight Commander file manager
- Color palette adapted for terminal file browsing

## Screenshots

*Add screenshots showing the theme in action with different file types and MC features*
