# Variables VS Code Extension

The Variables VS Code Extension adds syntax highlighting support to VS Code for `VARIABLES` files.

Variables files may look something like this:

```variables
VARIABLES_VERSION 1

ENVVAR int description goes here

# Comments are supported
MY_ENV str? this will help future engineers know what this env var is for
```

## Installation

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
```
