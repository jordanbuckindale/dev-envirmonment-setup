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
This configuration file customizes Vim settings to enhance the editing experience.

### General Settings
- **Compatibility Mode**: Disable compatibility with Vi (`nocompatible`).
- **Backspace Behavior**: Allows backspacing over indentations, end-of-line, and insert start (`backspace=indent,eol,start`).
- **Ruler**: Enables the ruler, showing the cursor position.
- **History Limit**: Keeps a history of 500 commands (`history=500`).
- **Ignore Modeline**: Prevents Vim from reading mode lines in files (`nomodeline`).
- **Syntax Highlighting**: Enabled by default (`syn on`).

### Text and Indent Settings
- **Line Numbers**: Displays line numbers (`number`).
- **Disable Wrap**: Disables text wrapping (`nowrap`).
- **Cursor Line**: Disables cursor line highlighting (`nocursorline`).
- **Mouse Support**: Enables mouse support (`mouse=a`).
- **Match Parentheses**: Shows matching parentheses (`showmatch`).
- **Auto Indentation**: Enables automatic indentation (`autoindent`).
- **Indent Width**: Sets indent width to 4 characters (`shiftwidth=4`).
- **Tab Settings**: 
  - Sets tab width to 4 characters (`tabstop=4`).
  - Converts tab characters to spaces (`expandtab`).

### Custom Key Mappings
- **Normal Mode Mappings**:
  - `F2`: Save file (`:w`).
  - `F3`: Save and quit file (`:wq`).
  - `F4`: Clear file contents (`ggdG`).
  - `F5`: Copy entire file contents to clipboard (`:%y+`).
- **Insert Mode Mappings**:
  - `F2`: Save file (`<C-o>:w`).
- **Navigation Shortcuts**:
  - `Ctrl+f`: Move to the end of the word.
  - `Ctrl+b`: Move to the beginning of the word.
  - `Ctrl+a`: Move to the end of the line.
  - `Ctrl+s`: Move to the beginning of the line.

## NeoVim
A collection of essential plugins and settings to enhance your Neovim experience.

### Core Utilities
- **plenary.nvim**: Utility functions used by other plugins.

### Appearance
- **folke/tokyonight.nvim**: A tokyonight colorscheme (with some custom color modifications).
- **nvim-lualine/lualine.nvim**: Enhanced statusline for a better visual experience.
- **akinsho/bufferline.nvim**: Improved tab display.

### Navigation
- **christoomey/vim-tmux-navigator**: Seamless navigation between Neovim splits and Tmux panes using `CTRL+h,j,k,l`.
- **nvim-tree/nvim-tree.lua**: File explorer for navigating files and directories.

### Productivity Tools
- **folke/which-key.nvim**: Displays keymap suggestions as you type.

### Fuzzy Finder and UI Enhancements
- **nvim-telescope/telescope.nvim**: Fuzzy finder for searching files, buffers, and more.
- **nvim-telescope/telescope-fzf-native.nvim**: FZF-native extension for better performance.

### Autocompletion and Snippets
- **hrsh7th/nvim-cmp**: Main autocompletion plugin.
  - **hrsh7th/cmp-buffer**: Completion source for text in the current buffer.
  - **hrsh7th/cmp-path**: Completion source for filesystem paths.
- **L3MON4D3/LuaSnip**: Snippet engine.
  - **saadparwaiz1/cmp_luasnip**: Completion source for LuaSnip.

### LSP and Code Intelligence
- **williamboman/mason.nvim**: Manage and install language servers, linters, and formatters.
  - **williamboman/mason-lspconfig.nvim**: Bridge between `mason` and `lspconfig`.
  - **neovim/nvim-lspconfig**: Simplifies LSP server configuration.
  - **hrsh7th/cmp-nvim-lsp**: Smart autocompletion with LSP integration.
- **folke/trouble.nvim**: Provides a better interface for diagnostics and other code-related issues.

### Formatting and Linting
- **stevearc/conform.nvim**: Easy configuration for formatters.
- **mfussenegger/nvim-lint**: Simple configuration for linters.
- **WhoIsSethDaniel/mason-tool-installer.nvim**: Automatically installs linters and formatters on startup.

### Comments
- **folke/todo-comments.nvim**: Highlight and search for comments like TODO, HACK, BUG.

### Treesitter and Syntax Highlighting
- **nvim-treesitter/nvim-treesitter**: Enhanced syntax highlighting and code navigation.
- **nvim-treesitter/nvim-treesitter-textobjects**: Additional text objects based on Tree-sitter.
- **windwp/nvim-autopairs**: Automatically close brackets, parentheses, quotes, etc.
- **windwp/nvim-ts-autotag**: Automatically close HTML/XML tags.
  
### Indentation
- **lukas-reineke/indent-blankline.nvim**: Display indent guides with Tree-sitter integration.

### Git Integration
- **lewis6991/gitsigns.nvim**: Shows Git changes and allows interaction with Git hunks.
- **kdheepak/lazygit.nvim**: Use Lazygit within Neovim.

### Miscellaneous
- **goolord/alpha-nvim**: Customizable start screen for Neovim.
- **rmagatti/auto-session**: Automatically save and restore Neovim sessions.

## Tmux
Customizes Tmux settings for an enhanced terminal experience.

### General Settings
- **True Color Support**: Enables 256-color mode.
- **Custom Prefix**: Changes the prefix key to `Ctrl-A` for Tmux commands.
- **Mouse Support**: Enables mouse usage within Tmux.
- **Vim Key Bindings**: Uses Vim-style key bindings for navigation and text selection.

### Pane Management
- **Resize Panes**: 
  - `h/j/k/l`: Resize panes left, down, up, and right by 5 units.
- **Navigation**:
  - `h/j/k/l`: Navigate between panes (Vim-style).
- **Split Panes**:
  - `|`: Splits window horizontally.
  - `-`: Splits window vertically.
- **Maximize Pane**: 
  - `m`: Toggles pane zoom.

### Refresh Configuration
- **Reload Config**: 
  - `r`: Reloads Tmux configuration file.

### Copy Mode
- **Selection and Copy**:
  - `v`: Begin text selection.
  - `y`: Copy selected text.

### Indexing and Directories
- **Base Index**: Sets pane and window indexing to start at 1.
- **Open Panes in Current Directory**: (Commented out by default.)

### Plugin Manager
- **TMUX Plugin Manager (TPM)**: Loads TPM and a set of useful plugins.
  - **Plugins**:
    - `vim-tmux-navigator`: Vim-style pane navigation.
    - `tmux-themepack`: Custom themes.
    - `tmux-resurrect`: Saves and restores Tmux sessions.
    - `tmux-continuum`: Autosaves sessions every 15 minutes.
- **Theme**: Uses `powerline/default/cyan` theme.
- **Session Persistence**: Enables capturing pane contents and auto-restoring sessions.


## Visual Studio Code
This guide provides instructions on how to customize the background of Visual Studio Code using the "Background" extension by Katsute.

### **Prerequisites**
- **Visual Studio Code**: Ensure you have the latest version installed.
- **Background Extension**: Install the extension from the [Visual Studio Code Marketplace](https://marketplace.visualstudio.com/items?itemName=katsute.background).

### **Installation Steps**
1. **Install the Extension:**
   - Open Visual Studio Code.
   - Go to the Extensions view by pressing `Ctrl+Shift+X` (Windows/Linux) or `Cmd+Shift+X` (Mac).
   - Search for "Background by Katsute."
   - Click **Install** to add the extension to your Visual Studio Code.
2. **Configure the Background:**
   - Open the command palette with `Ctrl+Shift+P` (Windows/Linux) or `Cmd+Shift+P` (Mac).
   - Type `>Background: Configuration` and select it to open the settings.
   - Add your desired configuration options to your settings.

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
