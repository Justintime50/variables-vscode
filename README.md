# Variables VS Code Extension

The [Variables VS Code Extension](https://marketplace.visualstudio.com/items?itemName=JustinHammond.variables) adds syntax highlighting support to VS Code for `VARIABLES` files.

Variables files may look something like this:

```variables
VARIABLES_VERSION 1

ENVVAR int description goes here

# Comments are supported
MY_ENV str? this will help future engineers know what this env var is for
```

## Installation

### Marketplace Installation

1. Open VS Code
2. Go to the Extensions menu
3. Search for "Variables"
4. Install

Alternatively, [install directly from this link](https://marketplace.visualstudio.com/items?itemName=JustinHammond.variables).

### Manual Installation

1. Open VS Code
2. Go to the Extensions menu
3. Select 3 dots in the menu bar, select `Install from VSIX`
4. Select available VSIX file (extension packaged up) or build from source (see [Development](#development)) below

If you need a screenshot of this, checkout <https://stackoverflow.com/a/50232194/6064135>

## Development

```shell
# Install the `vsce` tool
npm install -g @vscode/vsce

# Package the extension
vsce package

# Release the extension (pre-releases must have different versions than GA releases)
vsce publish --pre-release
vsce publish
```

## Attribution

[Variable icons created by Flipicon - Flaticon](https://www.flaticon.com/free-icons/variable)
