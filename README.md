# NOTE

This is a personal unmaintained fork of public archive available at https://github.com/Nitestack/PSNvimSwitcher

The author re-implemented the same functionality in Rust re-using `Nvim-Switcher` project name, but it didn't work for me out-of-the-box under Windows 10/PowerShell 7.

You can check his new implementation https://github.com/Nitestack/Nvim-Switcher

# Neovim Configuration Switcher

Neovim Switcher is a utility PowerShell module for switching between different Neovim configuration environments.

You'll need `fzf` installed.

## 🛠️ Installation

### Windows (Powershell)

#### Clone the repository

Use next command to get the list of module folders on your system

```pwsh
$env:PSModulePath -split ';'
```

Run this in one of the folders from the list above

```pwsh
git clone --depth 1 https://github.com/bybor/PSNvimSwitcher 
```


#### Include it in your PowerShell profile

Run, to open your profile file

```pwsh
nvim $profile
```

Add this line and save your changes

```pwsh
Import-Module Nvim-Switcher
```

## 📖 Documentation

### Commands

The commands below don't take any input parameters but will provide you with `fzf` based selection

- `nvims` or `nvs`: Select configuration to start Neovim with
- `nvims-add` or `nvs-add`: Download a Neovim configuration
- `nvims-del` or `nvs-del`: Uninstalls a Neovim configuration
- `nvims-c` or `nvc`: Configure a Neovim configuration
