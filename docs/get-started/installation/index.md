# Installation

To use this plugin, you must install both the **Gemini CLI tool** and the **Sublime Text package**.

## Install Gemini CLI

The plugin relies on the Google Gemini CLI. Ensure you have Node.js installed, then run:

```bash
npm install -g @google/gemini-cli
```

**Requirement:** gemini-cli version `0.34.0` or higher is required.

The plugin automatically detects CLI installation across multiple environments, including **Homebrew**, **npm-global**, **Yarn**, and common local binary directories.

## Install GeminiCLI Plugin

### Via Package Control (Recommended)
The easiest way to install the plugin is through **Package Control**:
1. Open the command palette (`Cmd+Shift+P` on macOS, `Ctrl+Shift+P` on Windows/Linux).
2. Type `Package Control: Install Package` and press `Enter`.
3. Search for `GeminiCLI` and press `Enter`.

### Manual Installation
If you prefer to install from source:
1. Open Sublime Text and navigate to `Preferences` -> `Browse Packages...`.
2. Clone the repository into that directory:
   ```bash
   git clone https://github.com/flashmodel/gemini-st GeminiCLI
   ```
3. Restart Sublime Text.

## Configuration

If the command line tool is installed in a non-standard path, or you wish to use a specific `gemini` version, you can manually set the path in `Preferences -> Package Settings -> GeminiCLI -> Settings`.

Example `gemini_command` paths:
- Windows: `"C:/Users/myname/AppData/Roaming/npm/gemini.cmd"`
- macOS/Linux: `"/usr/local/bin/gemini"`
