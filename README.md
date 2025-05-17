# 🛠️ Ryan's Dotfiles

Welcome to my dotfiles! This is my personalized setup for macOS using:

- ⚡️ `yabai` – dynamic tiling window manager
- ⌨️ `skhd` – keybind manager for macOS
- 🌀 `LazyVim` – a modern Neovim config
- 🦄 `zsh` with `oh-my-zsh` + `powerlevel10k`
- 🧭 `zoxide`, `colorls`, and other CLI sugar

---

## 🔧 Configured Tools

### 🧱 `yabai`

Located in `.config/yabai/`  
I use a **bsp** layout with sensible defaults:

- 12px gaps and padding
- Window focus with `alt + hjkl`
- Window swapping, warping, and movement between displays/spaces
- Floating toggle with grid placement
- Display mirroring and rotation

### ⌨️ `skhd`

Located in `.config/skhd/`  
My keybindings include:

- Vim-style window focus (`alt + hjkl`)
- Moving windows (`ctrl/alt/shift + hjkl`)
- Managing spaces (`shift + alt + 1-7`, `p`, `n`)
- Toggling float, fullscreen, and layout mirroring
- Starting/stopping `yabai` services via hotkeys

### 🌀 `LazyVim`

Located in `.config/nvim/`  
My Neovim config is based on [LazyVim](https://www.lazyvim.org/):

- Built-in LSP
- Treesitter, Telescope, and file navigation
- Lua-based configuration with plugin management

> This config is ideal for modern development across Go, TypeScript, and Python.

### 💬 `.zshrc` + Terminal Setup

Located at `.zshrc`

Features:

- 🦄 `powerlevel10k` theme
- `oh-my-zsh` for plugin and theme management
- CLI enhancements:
  - `alias ls='colorls'` for pretty directory listings
  - `fastfetch` on shell load for system info
  - `zoxide` for smarter `cd` navigation
- Auto-sourcing of `.p10k.zsh` if present

---

## 🧠 How to Use

```bash
git clone https://github.com/yourusername/dotfiles.git ~/dotfiles

# Symlink configs
ln -s ~/dotfiles/.config/yabai ~/.config/yabai
ln -s ~/dotfiles/.config/skhd ~/.config/skhd
ln -s ~/dotfiles/.config/nvim ~/.config/nvim
ln -s ~/dotfiles/.zshrc ~/.zshrc
