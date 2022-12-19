# Visual Studio Code Settings

### Requirements

* [Dank Mono font](https://philpl.gumroad.com/l/dank-mono)

___

### `settings.json`

```json
{
  "[typescript]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "files.trimTrailingWhitespace": true,
  "[json]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "editor.fontSize": 16,
  "editor.fontFamily": "Dank Mono",
  "atomKeymap.promptV3Features": true,
  "editor.formatOnPaste": false,
  "editor.cursorBlinking": "solid",
  "[typescriptreact]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "terminal.integrated.fontSize": 16,
  "editor.cursorStyle": "line",
  "editor.insertSpaces": true,
  "editor.tabSize": 2,
  "editor.formatOnSave": true,
  "editor.accessibilitySupport": "off",
  "editor.fontLigatures": true,
  "editor.fontWeight": "400",
  "typescript.updateImportsOnFileMove.enabled": "always",
  "editor.cursorWidth": 5,
  "prettier.tabWidth": 2,
  "prettier.useTabs": false,
  "prettier.singleQuote": true,
  "diffEditor.ignoreTrimWhitespace": false,
  "editor.lineHeight": 25,
  "explorer.confirmDragAndDrop": false,
  "workbench.startupEditor": "newUntitledFile",
  "git.autofetch": true,
  "files.autoSave": "off",
  "git.confirmSync": false,
  "javascript.validate.enable": false,
  "explorer.confirmDelete": false,
  "[javascript]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "security.workspace.trust.untrustedFiles": "open",
  "editor.renderWhitespace": "none",
  "javascript.updateImportsOnFileMove.enabled": "always",
  "git.enableSmartCommit": true,
  "terminal.integrated.env.osx": {
    "FIG_NEW_SESSION": "1"
  },
  "gitlens.defaultDateFormat": null,
  "editor.inlineSuggest.enabled": true,
  "material-icon-theme.activeIconPack": "react",
  "material-icon-theme.files.associations": {},
  "workbench.colorCustomizations": {},
  "importCost.typescriptExtensions": ["\\.tsx?$"],
  "workbench.colorTheme": "Dracula",
  "github.copilot.enable": {
    "*": true,
    "yaml": false,
    "plaintext": true,
    "markdown": true
  }
}
```
