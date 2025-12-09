# Deep Focus Theme

**Clean. Professional. Eye-strain free.**

A dark Visual Studio Code theme designed specifically for professional software engineers and developers who spend long hours coding. This theme prioritizes readability, accessibility, and productivity while maintaining a modern, minimalistic aesthetic.

## ✨ Features

### 🎯 **Optimized for Long Coding Sessions**
- Carefully balanced contrast ratios to reduce eye strain
- Dark mode base with warm, comfortable colors
- Subtle highlighting that won't distract from your code

### 🎨 **Professional Color Scheme**
- **Keywords & Control Flow**: Purple (`#c678dd`)
- **Strings**: Green (`#98c379`)
- **Numbers**: Orange (`#d19a66`)
- **Variables**: Warm beige (`#e8d5b7`)
- **Functions**: Blue (`#61afef`)
- **Classes & Types**: Yellow (`#e5c07b`)
- **Comments**: Muted gray (`#5c6370`) with italic styling

### 🔧 **Language Support**
Syntax highlighting optimized for:
- JavaScript & TypeScript
- Python
- Java
- C# & .NET
- Go
- HTML & CSS
- Markdown
- JSON & YAML
- And many more...

### ♿ **Accessibility First**
- WCAG-compliant contrast ratios
- Color-blind friendly color palette
- Clear visual hierarchy
- Distinct error and warning indicators

### 🎛️ **UI Styling**
- Clean, minimalistic sidebar and tabs
- Professional blue accent color (`#007acc`)
- Smooth hover effects and transitions
- Consistent spacing and typography

## 🚀 Installation

### Option 1: From VS Code Marketplace (Coming Soon)

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
   - Select "Deep Focus Dark"

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

## 🎯 Theme Highlights

### Syntax Examples

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

- **Clean Tabs**: Active tabs are clearly distinguished with the blue accent
- **Readable Sidebar**: Consistent spacing and muted colors for better focus
- **Status Bar**: Professional blue background with clear text
- **Error Highlighting**: Subtle but noticeable error and warning indicators
- **Git Integration**: Color-coded git status indicators

## 🔧 Customization

You can further customize the theme by modifying the `themes/deep-focus-dark.json` file in your local installation. Here are some common customizations:

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

## 🎨 Recommended Settings

For the best experience with Deep Focus:

### Icon Theme
- **Recommended**: Material Icon Theme by Philipp Kief
- **Installation**: Search for "Material Icon Theme" in the Extensions marketplace

### Font
- **Recommended**: Fira Code, JetBrains Mono, or Cascadia Code
- Enable font ligatures for better code readability:
  ```json
  "editor.fontFamily": "'Fira Code', Consolas, 'Courier New', monospace",
  "editor.fontLigatures": true
  ```

## 🤝 Contributing

Found a bug or have a suggestion? Feel free to:

1. Open an issue describing the problem or enhancement
2. Fork the repository and make your changes
3. Submit a pull request with a clear description

## 📄 License

This theme is released under the MIT License. See the `LICENSE` file for details.

## 🙏 Acknowledgments

Inspired by the best practices in theme design and accessibility guidelines. Special thanks to the VS Code team for providing excellent theming capabilities.

## 📊 Repository

- **GitHub**: [srisatyakrishna5/vscode-my-custom-theme](https://github.com/srisatyakrishna5/vscode-my-custom-theme)
- **Issues**: Report bugs or request features on GitHub
- **Version**: 1.0.0

---

**Happy Coding! 🚀**

*Made with ❤️ by Sri Satya Krishna Challa for developers who care about their coding environment.*