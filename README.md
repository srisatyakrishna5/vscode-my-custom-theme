# Deep Focus Themes

Soft, low-fatigue Visual Studio Code themes for developers who spend long hours in the editor.

This extension now ships with four color themes:
- Deep Focus Dark
- Deep Focus Light
- Dev Theme Dark
- Dev Theme Light

## Features

### Optimized for Long Coding Sessions
- Soft backgrounds instead of harsh black or pure white
- Muted accents that reduce eye strain while preserving syntax clarity
- Balanced contrast for code, sidebars, tabs, and terminal output

### Dev Theme Palette Direction
- Keywords and flow: muted lavender
- Functions and methods: calm blue
- Strings: soft sage green
- Numbers and constants: warm amber
- Types and classes: muted gold
- Comments: fog gray with restrained emphasis

### Language Support
Syntax highlighting is tuned for:
- JavaScript & TypeScript
- Python
- HTML & CSS
- Markdown
- JSON & YAML
- Shell scripts
- General-purpose syntax scopes used by many other languages

### Accessibility First
- WCAG-compliant contrast ratios
- Clear visual hierarchy
- Distinct but non-harsh error and warning indicators

### UI Styling
- Softer tab, sidebar, and status bar surfaces
- More restrained highlights for selections and search matches

## 🚀 Installation

### Option 1: From VS Code Marketplace

Once published, you can install directly from VS Code:

1. Open VS Code
2. Go to Extensions (Ctrl+Shift+X)
3. Search for "Deep Focus"
4. Click Install
5. Select "Deep Focus Dark" from the Color Theme picker

### Option 2: Manual Installation (For Development)

1. **Clone or download** this repository
2. **Copy the theme files** to your VS Code extensions directory:
   ```bash
   # Windows
   cp -r . %USERPROFILE%\.vscode\extensions\deep-focus-1.0.0
   
   # macOS/Linux
   cp -r . ~/.vscode/extensions/deep-focus-1.0.0
   ```

3. **Reload VS Code** by pressing `Ctrl+Shift+P` (or `Cmd+Shift+P` on macOS) and running "Developer: Reload Window"

4. **Apply the theme**:
   - Press `Ctrl+Shift+P` (or `Cmd+Shift+P` on macOS)
   - Type "Preferences: Color Theme"
  - Select "Dev Theme Dark" or "Dev Theme Light"

### Option 3: Package and Install (For Distribution)

1. **Install vsce** (VS Code Extension Manager):
   ```bash
   npm install -g @vscode/vsce
   ```

2. **Package the extension**:
   ```bash
   vsce package
   ```

3. **Install the packaged extension**:
   ```bash
   code --install-extension deep-focus-1.0.0.vsix
   ```

## Theme Highlights

### Theme Families

#### Deep Focus
- Existing themes with the original Deep Focus visual direction

#### Dev Theme
- New softer dark and light variants
- No pink accents or hot neon hues
- Designed specifically to reduce visual fatigue in mixed-language projects

**JavaScript/TypeScript:**
```javascript
// Comments are italicized and muted
function calculateTotal(items) {
    const total = items.reduce((sum, item) => {
        return sum + item.price * item.quantity;
    }, 0);
    return `Total: $${total.toFixed(2)}`;
}
```

**Python:**
```python
# Clean, readable syntax highlighting
class DataProcessor:
    def __init__(self, data_source: str):
        self.data_source = data_source
        self.processed_count = 0
    
    def process_batch(self, batch_size: int = 100) -> bool:
        """Process data in batches for better performance"""
        try:
            # Processing logic here
            return True
        except Exception as e:
            logger.error(f"Processing failed: {e}")
            return False
```

### UI Features

- Active tabs use a low-intensity accent rather than a high-contrast strip
- Sidebars and panels stay legible without flattening the whole interface
- Git states, diagnostics, and diff colors remain distinct without oversaturation

## Customization

You can further customize the themes by modifying the files under `themes/`.

### Change the Accent Color
```json
{
  "colors": {
    "tab.activeBorder": "#your-color-here",
    "statusBar.background": "#your-color-here",
    "activityBar.activeBorder": "#your-color-here"
  }
}
```

### Adjust Font Styles
```json
{
  "tokenColors": [
    {
      "scope": ["comment"],
      "settings": {
        "fontStyle": "italic bold",
        "foreground": "#your-color-here"
      }
    }
  ]
}
```

## Recommended Settings

For the best experience with Dev Theme:

### Font
- **Recommended**: Fira Code, JetBrains Mono, or Cascadia Code
- Enable font ligatures for better code readability:
  ```json
  "editor.fontFamily": "'Fira Code', Consolas, 'Courier New', monospace",
  "editor.fontLigatures": true
  ```

## Contributing

Found a bug or have a suggestion? Feel free to:

1. Open an issue describing the problem or enhancement
2. Fork the repository and make your changes
3. Submit a pull request with a clear description

## License

This theme is released under the MIT License. See the `LICENSE` file for details.

## Repository

- **GitHub**: [srisatyakrishna5/vscode-my-custom-theme](https://github.com/srisatyakrishna5/vscode-my-custom-theme)
- **Issues**: Report bugs or request features on GitHub
- **Version**: 1.1.0

---

Built for developers who want a calmer editor without sacrificing syntax clarity.