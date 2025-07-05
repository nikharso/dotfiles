# 🛠️ My Dotfiles

A minimal yet powerful dotfiles setup built for speed, clarity, and productivity for **VSCode**, **Neovim**, **tmux**, **Ghostty** and **Alacritty**.

This repo brings together:

- ⚡ VSCode with Vim keybindings
- 🧠 Fully tuned Neovim config (Lua-based)
- ⌨️ Tmux workflow
- 🖼️ Custom wallpapers
- 🖋️ Nerd Fonts
- 🧳 Terminal configs: Ghostty & Alacritty

> [!NOTE]
>
> As of now, My daily Drivers for coding is Ghostty (terminal) and VSCode (code editor).

---

## 📦 What's Inside

| Component      | Description |
|----------------|-------------|
| `nvim/`        | Full Neovim config with Treesitter, LSPs, fuzzy finding, and more |
| `vscode/`      | `settings.json` and `keybindings.json` with Vim mode and ergonomic keymaps |
| `tmux/`        | Minimal `.tmux.conf` with sane defaults |
| `ghostty/`     | My Ghostty configuration for Mac/Linux |
| `fonts/`       | Nerd Font files used across the setup |

---

## 🧠 My VSCode + Vim Setup

A minimalist yet powerful configuration that brings the best of **Vim** keybindings to **VSCode**, and a fully-loaded **Neovim** environment for power users.

This setup is optimized for developers who want fast navigation, distraction-free UI, and ergonomic keybindings — with sensible defaults.

If you're using VSCode with Vim mode, here’s what you need for a clean and productive workflow.

### 🔌 Required Extensions

Ensure the following extensions are installed:

1. [Vim](https://marketplace.visualstudio.com/items?itemName=vscodevim.vim)
2. [Tabler Product Icons](https://marketplace.visualstudio.com/items?itemName=zguolee.tabler-icons)
3. [Catppuccin for VSCode](https://marketplace.visualstudio.com/items?itemName=Catppuccin.catppuccin-vsc)
4. [Symbols](https://marketplace.visualstudio.com/items?itemName=miguelsolorio.symbols)
5. [Prettier - Code formatter](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)

> [!NOTE]
> Once installed, copy `settings.json` and `keybindings.json` from this repo into your VSCode `User` folder.

---

### 🧭 Keybindings Cheatsheet

> `[N]` – Normal Mode  
> `[V]` – Visual Mode  
> `[I]` – Insert Mode

#### 🚀 Navigation

| Shortcut | Mode | Action |
|---------|------|--------|
| `Ctrl + h/l/j/k` | [N] | Move between splits or editor windows |
| `Ctrl + e` | [N] | Toggle File Explorer |
| `Tab / Shift + Tab` | [N] | Switch tabs forward/backward |
| `Shift + j/k` | [V] | Move selected lines up/down |
| `Shift + k` | [N] | Show hover |
| `Space + c + a` | [N] | Code action |
| `Space + c + r` | [N] | Rename symbol |
| `Space + c + s` | [N] | Go to symbol |
| `Space + b + d/o` | [N] | Close active / other buffers |
| `Space + Space` | [N] | Quick Open |
| `Space + g + d/r/g` | [N] | Go to definition / references / Git |
| `Ctrl + m` | [N] | Toggle fold |
| `Ctrl + n` | [N] | Add selection to next find match |
| `j + j` | [I] | Escape to Normal mode |

---

### 🗂️ File Explorer

When the explorer panel is focused:

| Key | Action |
|-----|--------|
| `r` | Rename file |
| `c` | Copy file |
| `p` | Paste file |
| `d` | Delete file |
| `x` | Cut file |
| `a / Shift + a` | New file / folder |
| `s / Shift + s` | Open in vertical / horizontal split |

> [!NOTE]
> Some `Ctrl` keys like `Ctrl+C`, `Ctrl+A`, `Ctrl+P` are intentionally disabled in Vim mode to use VSCode-native bindings.

---

## 🧪 Neovim Configuration

Want full Vim power? You can use my **Neovim** setup as a complete development environment.

### 🛠 Requirements

- **Neovim** `>= 0.9.0` (compiled with LuaJIT)
- **Git** `>= 2.19.0` (for partial clone support)
- A [Nerd Font](https://www.nerdfonts.com/)
- A working **C compiler** (required by `nvim-treesitter`)

---

### 🔧 Setup Steps

```bash
# Clone this repository
git clone https://github.com/nikharx/dotfiles.git

# Navigate into the directory
cd dotfiles

# Backup your current Neovim config (if any)
mv ~/.config/nvim ~/.config/nvim.bak

# Copy my config
cp -r ./nvim ~/.config/nvim

# Launch Neovim
nvim
