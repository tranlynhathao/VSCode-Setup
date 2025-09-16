# VS Code Setup

[![VS Code](https://img.shields.io/badge/VS%20Code-007ACC?style=flat&logo=visual-studio-code&logoColor=white)](https://code.visualstudio.com/)
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/yourusername/vscode-setup/graphs/commit-activity)

A comprehensive, production-ready VS Code configuration optimized for modern development workflows. This setup includes carefully curated settings, custom keybindings, and enhanced UI styling for maximum productivity.

## Features

### Editor Configuration

- **Clean Interface**: Minimalist design with reduced visual noise
- **Typography**: Optimized font settings with Geist Mono and JetBrains Mono
- **Code Formatting**: Prettier integration with format-on-save for multiple languages
- **Smart Suggestions**: Enhanced IntelliSense and code completion
- **Vim Integration**: Full Vim keybindings with custom mappings

### Custom Keybindings

- **Space-based Leader Keys**: Intuitive command palette access
- **Navigation**: Vim-style movement with `Ctrl+hjkl`
- **File Operations**: Streamlined file explorer interactions
- **Debugging**: Comprehensive debug workflow shortcuts
- **Code Actions**: Quick access to refactoring and code actions

### Visual Enhancements

- **Custom CSS**: Professional styling with backdrop blur effects
- **Command Palette**: Enhanced with custom styling and animations
- **Sidebar**: Clean file explorer with improved visual hierarchy
- **Hover Effects**: Polished tooltips and information displays

### Language Support

- **PHP**: Optimized for Laravel development with Intelephense
- **JavaScript/TypeScript**: Full React and Vue.js support
- **CSS/Tailwind**: Enhanced styling workflow
- **JSON**: Improved formatting and validation

## Installation

### Prerequisites

- VS Code 1.80.0 or higher
- [Vim Extension](https://marketplace.visualstudio.com/items?itemName=vscodevim.vim)
- [Custom CSS and JS Loader](https://marketplace.visualstudio.com/items?itemName=be5invis.vscode-custom-css)

### Setup Instructions

1. **Clone the repository**

   ```bash
   git clone https://github.com/yourusername/vscode-setup.git
   cd vscode-setup
   ```

2. **Backup your current settings**

   ```bash
   # Windows
   cp %APPDATA%\Code\User\settings.json %APPDATA%\Code\User\settings.json.backup
   cp %APPDATA%\Code\User\keybindings.json %APPDATA%\Code\User\keybindings.json.backup

   # macOS
   cp ~/Library/Application\ Support/Code/User/settings.json ~/Library/Application\ Support/Code/User/settings.json.backup
   cp ~/Library/Application\ Support/Code/User/keybindings.json ~/Library/Application\ Support/Code/User/keybindings.json.backup

   # Linux
   cp ~/.config/Code/User/settings.json ~/.config/Code/User/settings.json.backup
   cp ~/.config/Code/User/keybindings.json ~/.config/Code/User/keybindings.json.backup
   ```

3. **Install the configuration**

   ```bash
   # Copy settings and keybindings
   cp my-setup/settings.json ~/.config/Code/User/settings.json
   cp my-setup/keybindings.json ~/.config/Code/User/keybindings.json

   # Copy custom styling files
   cp my-setup/custom-style.css ~/custom-vscode.css
   cp my-setup/custom-script.js ~/custom-vscode-script.js
   ```

4. **Enable custom CSS**
   - Install the "Custom CSS and JS Loader" extension
   - Reload VS Code window (`Ctrl+Shift+P` → "Developer: Reload Window")

## Configuration Details

### Settings Highlights

#### Editor Behavior

- Disabled visual noise (brackets, hover delays, decorations)
- Enhanced word selection with custom separators
- Optimized cursor behavior and selection handling
- Smart indentation detection disabled for consistency

#### Code Formatting

- Prettier as default formatter for web technologies
- Format on save enabled for supported languages
- Consistent tab width (2 spaces) across all languages
- EditorConfig integration disabled for manual control

#### Search & Navigation

- Excluded common build directories from search
- Optimized file associations for PHP development
- Enhanced symbol navigation and reference finding

#### Vim Integration

- Custom leader key mappings (`Space` as primary leader)
- File explorer integration with Vim-style navigation
- Debug workflow optimized for Vim users

### Keybinding Reference

#### Navigation

- `Ctrl+h/j/k/l` - Navigate left/down/up/right
- `Space ,` - Show all editors
- `Space e` - Toggle sidebar and focus file explorer

#### Code Actions

- `Space c a` - Code actions
- `Space c r` - Rename symbol
- `Space c s` - Go to symbol
- `Shift+K` - Show hover information

#### File Operations

- `r` - Rename file (in file explorer)
- `c` - Copy file
- `p` - Paste file
- `d` - Delete file
- `a` - New file
- `s` - Open to side

#### Debugging

- `Space d a` - Start debugging
- `Space d t` - Stop debugging
- `Space d o` - Step over
- `Space d b` - Toggle breakpoint
- `Space d c` - Continue

## Custom Styling

The setup includes custom CSS that enhances the visual experience:

- **Command Palette**: Centered with backdrop blur and custom styling
- **File Explorer**: Improved selection states and typography
- **Hover Effects**: Enhanced tooltips with gradient backgrounds
- **Scrollbars**: Minimalist design with custom colors
- **Sidebar**: Professional shadows and visual hierarchy

## Recommended Extensions

While this setup works with minimal extensions, these are recommended for the full experience:

- [Vim](https://marketplace.visualstudio.com/items?itemName=vscodevim.vim)
- [Custom CSS and JS Loader](https://marketplace.visualstudio.com/items?itemName=be5invis.vscode-custom-css)
- [Prettier - Code formatter](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)
- [Material Icon Theme](https://marketplace.visualstudio.com/items?itemName=PKief.material-icon-theme)
- [Intelephense](https://marketplace.visualstudio.com/items?itemName=bmewburn.vscode-intelephense-client)

## Customization

### Modifying Settings

Edit `my-setup/settings.json` to customize editor behavior, then reinstall the configuration.

### Adding Keybindings

Add new keybindings to `my-setup/keybindings.json` following the existing format.

### Styling Changes

Modify `my-setup/custom-style.css` to adjust visual elements. Remember to update the file paths in your settings if you change the CSS file location.

## Troubleshooting

### Custom CSS Not Loading

1. Ensure the "Custom CSS and JS Loader" extension is installed and enabled
2. Check that the file paths in settings.json point to the correct CSS and JS files
3. Reload the VS Code window after making changes

### Keybindings Not Working

1. Verify that the Vim extension is installed and enabled
2. Check for conflicts with other extensions
3. Ensure the keybinding syntax is correct in keybindings.json

### Performance Issues

1. Disable unused extensions
2. Check if custom CSS is causing rendering issues
3. Consider reducing the number of enabled features in settings

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request. For major changes, please open an issue first to discuss what you would like to change.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- VS Code team for the excellent editor
- Vim extension maintainers for seamless integration
- The open-source community for inspiration and feedback

---

**Note**: This configuration is optimized for web development with a focus on PHP/Laravel, JavaScript/TypeScript, and modern CSS frameworks. Adjust settings as needed for your specific development environment.
