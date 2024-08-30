# Developer Environment Workflow & Configurations

This is a summary of my current developer environment setup.

- **Alacritty** - Main Terminal
- **Vim** - Lightweight Text Editor
- **Tmux** - Terminal Multiplexer for managing multiple terminal sessions
- **Neovim** - Main Text Editor for code development
- **Visual Studio Code** - Backup IDE
- **Yabai** - Tiling Window Manager for efficient workspace management
- **SketchyBar** - Status Bar with customizable widgets and information display
- **Zsh** - Default Shell for managing terminal sessions with advanced features and customization

## Alacritty

This file sets up Alacritty, a GPU-accelerated terminal emulator, with various settings to enhance appearance and usability.

### General Settings
- **Import Theme**: Loads the `coolnight.toml` theme from the specified path, applying a pre-defined color scheme and visual settings.
- **Environment Variables**: Sets the terminal type to `"xterm-256color"`, enabling 256-color support for applications running in the terminal.

### Window and Appearance Settings
- **Window Padding**: 
  - `padding.x`: Adds 10 pixels of padding on the horizontal axis.
  - `padding.y`: Adds 11 pixels of padding on the vertical axis.
- **Window Decorations**: 
  - `decorations`: Removes window decorations like minimize, maximize, and close buttons for a cleaner, buttonless look.
- **Window Opacity**: 
  - `opacity`: Sets the terminal window's opacity to 80%, making it slightly transparent.
- **Option Key Behavior**: 
  - `option_as_alt`: Configures both left and right Option (Alt) keys to function as the Alt key.

### Font Settings
- **Font Family**: 
  - `normal.family`: Specifies `"0xProto Nerd Font"` as the font used in the terminal, which is a variant of Nerd Font.
- **Font Size**: 
  - `size`: Sets the font size to `15` for improved readability.

## Vim

## NeoVim

## Tmux

## Visual Studio Code

## Yabai
This file configures Yabai, a tiling window manager for macOS, with custom keyboard shortcuts to improve window management and productivity.

### Window Focus Management
- **Change Window Focus within the Same Space**:
  - `alt + j`: Focuses the window to the south.
  - `alt + k`: Focuses the window to the north.
  - `alt + h`: Focuses the window to the west.
  - `alt + l`: Focuses the window to the east.

### Display Focus Management
- **Change Focus between External Displays**:
  - `alt + s`: Focuses the display to the west.
  - `alt + g`: Focuses the display to the east.

### Space Layout Adjustments
- **Rotate Layout Clockwise**:
  - `shift + alt + r`: Rotates the current space layout 270 degrees.
- **Flip Layout Along Y-Axis**:
  - `shift + alt + y`: Mirrors the layout along the y-axis.
- **Flip Layout Along X-Axis**:
  - `shift + alt + x`: Mirrors the layout along the x-axis.

### Window Management
- **Toggle Window Float**:
  - `shift + alt + t`: Toggles the floating state of the window, positioning it on a 4x4 grid.
- **Maximize Window**:
  - `shift + alt + m`: Toggles the window to fullscreen mode.
- **Balance Window Tree**:
  - `shift + alt + e`: Balances the tree of windows, resizing them to occupy equal areas.

### Window Swapping
- **Swap Windows**:
  - `shift + alt + j`: Swaps the window with the one to the south.
  - `shift + alt + k`: Swaps the window with the one to the north.
  - `shift + alt + h`: Swaps the window with the one to the west.
  - `shift + alt + l`: Swaps the window with the one to the east.

### Window Movement and Splitting
- **Move Window and Split**:
  - `ctrl + alt + j`: Moves the window to the south and splits it.
  - `ctrl + alt + k`: Moves the window to the north and splits it.
  - `ctrl + alt + h`: Moves the window to the west and splits it.
  - `ctrl + alt + l`: Moves the window to the east and splits it.

### Display Management
- **Move Window to Another Display**:
  - `shift + alt + s`: Moves the window to the display on the left and focuses on it.
  - `shift + alt + g`: Moves the window to the display on the right and focuses on it.

### Yabai Service Management
- **Stop, Start, and Restart Yabai**:
  - `ctrl + alt + q`: Stops the Yabai service.
  - `ctrl + alt + s`: Starts the Yabai service.
  - `ctrl + alt + r`: Restarts the Yabai service.

## Zsh
Customizes the Zsh shell with enhanced usability and productivity settings.

### Powerlevel10k Prompt
- **Instant Prompt**: Speeds up startup by preloading the prompt.
- **Theme**: Loads the Powerlevel10k theme.

### General Settings
- **Aliases**: 
  - `reload-zsh`: Reload Zsh.
  - `edit-zsh`: Edit Zsh config in Neovim.
- **History**: Saves 1,000 commands, shares across sessions, avoids duplicates.
- **Key Bindings**: Arrow keys search through command history.

### Plugins
- **Autosuggestions**: Recommends commands.
- **Syntax Highlighting**: Colors commands and syntax.

### Custom Aliases
- **`ls` Replacement**: Uses `eza` for icons in directory listings.

### Fuzzy Finder
- **fzf Integration**: Enables fuzzy search.

### Zoxide Setup
- **Enhanced Navigation**: `z` replaces `cd` for smarter directory jumps.

## Sketchybar
