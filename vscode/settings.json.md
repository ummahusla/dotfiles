# Visual Studio Code Settings

### Requirements

* [Monaspace Neon font](https://monaspace.githubnext.com/)
* [zsh](https://ohmyz.sh/)
* [iTerm2](https://iterm2.com/)
* [Dracula Theme](https://draculatheme.com/visual-studio-code)

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
  "editor.fontSize": 14,
  "editor.fontFamily": "Monaspace Neon",
  "editor.formatOnPaste": false,
  "editor.cursorBlinking": "solid",
  "[typescriptreact]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "terminal.integrated.fontSize": 16,
  "editor.cursorStyle": "line",
  "editor.insertSpaces": true,
  "editor.tabSize": 23,
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
  "workbench.startupEditor": "none",
  "git.autofetch": true,
  "files.autoSave": "off",
  "git.confirmSync": false,
  "javascript.validate.enable": false,
  "explorer.confirmDelete": false,
  "[javascript]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode",
    "editor.formatOnSave": true
  },
  "[javascriptreact]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode",
    "editor.formatOnSave": true
  },
  "[jsonc]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode",
    "editor.formatOnSave": true
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
  "workbench.colorCustomizations": {},
  "importCost.typescriptExtensions": ["\\.tsx?$"],
  "workbench.colorTheme": "Dracula",
  "github.copilot.enable": {
    "*": true,
    "plaintext": true,
    "markdown": true,
    "scminput": false,
    "yaml": false
  },
  "files.associations": {
    "*.mdx": "markdown",
    "*.tsx": "typescriptreact"
  },

  "terminal.explorerKind": "external",
  "terminal.integrated.automationProfile.osx": {},
  "terminal.external.osxExec": "iTerm.app",
  "terminal.integrated.defaultProfile.osx": "zsh",
  "prettier.useEditorConfig": false,
  "playwright.reuseBrowser": true,
  "window.zoomLevel": 1
}
```
