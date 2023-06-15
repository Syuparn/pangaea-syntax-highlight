# pangaea-syntax-highlight README

[![MIT License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat)](LICENSE)
[![Extention Version](https://img.shields.io/badge/version-0.2.0-green.svg)](https://marketplace.visualstudio.com/items?itemName=Syuparn.pangaea-syntax-highlight)

VSCode Syntax Highlighting for Pangaea Language

(If you would like to know about Pangaea, see [https://github.com/Syuparn/Pangaea](https://github.com/Syuparn/Pangaea))

## Features

### Syntax Highlighting

![highlighting](images/highlighting.png)

### Snippets

- `func`: new Func object (`{|| }`)
- `iter`: new Iter object (`<{|| }>`)
- `m`: new method-form Func object (`m{|| }`)
- `m`: new method-form Iter object (`m<{|| }>`)

> **Tips:** These snippets recommend **tabsize 2**.
> 
> To change tabsize, open `settings.json` by `Preferences Open Settings(JSON)`
> in the command palette and add
> 
> ```
> "[pangaea]": {
>     "editor.tabSize": 2
> }, 
> ```

# Development
## Deploy to marketplace

```bash
# 1. install vsce
$ npm install --global @vscode/vsce

# 2. create a new token via `https://dev.azure.com/${your_account}/_usersSettings/tokens`
# - Organization: All accessible organizations
# - Scopes: Marketplace (Acquire, Manage)

# 3. publish new version
$ vsce publish minor
```
