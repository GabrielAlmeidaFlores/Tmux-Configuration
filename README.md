# Tmux Configuration

A personal tmux configuration focused on a smooth terminal workflow with Vim-style keybindings, plugin management via TPM, and the Tokyo Night theme.

## Features

- **256-color & RGB support** — full color terminal experience
- **Mouse support** — click to select panes/windows
- **Vim-style copy mode** — navigate and copy text with familiar keybindings
- **Smart splits** — new panes/windows open in the current working directory
- **Session persistence** — automatic save/restore via tmux-resurrect & tmux-continuum
- **Vim/Neovim integration** — seamless pane navigation with vim-tmux-navigator

## Plugins

| Plugin | Purpose |
|---|---|
| [tpm](https://github.com/tmux-plugins/tpm) | Plugin manager |
| [vim-tmux-navigator](https://github.com/christoomey/vim-tmux-navigator) | Seamless Vim/tmux pane navigation |
| [tmux-tokyo-night](https://github.com/fabioluciano/tmux-tokyo-night) | Tokyo Night status bar theme |
| [tmux-resurrect](https://github.com/tmux-plugins/tmux-resurrect) | Save and restore sessions |
| [tmux-continuum](https://github.com/tmux-plugins/tmux-continuum) | Automatic session saving |

## Installation

### Prerequisites

- tmux ≥ 2.6
- [TPM](https://github.com/tmux-plugins/tpm)
- `xclip` (for clipboard integration)
- `zsh` (configured as the default shell)

### Install TPM

```bash
git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm
```

### Apply the config

```bash
git clone https://github.com/flores/Tmux-Configuration.git
cp Tmux-Configuration/.tmux.conf ~/.tmux.conf
tmux source ~/.tmux.conf
```

Then press `prefix + I` (capital i) inside tmux to install all plugins.

## Key Bindings

| Binding | Action |
|---|---|
| `prefix + "` | Split pane vertically (same directory) |
| `prefix + %` | Split pane horizontally (same directory) |
| `prefix + c` | New window (same directory) |
| `prefix + [` → `v` | Begin visual selection in copy mode |
| `prefix + [` → `y` | Copy selection to system clipboard |
| `Ctrl+h/j/k/l` | Navigate panes (via vim-tmux-navigator) |

> Default prefix is `Ctrl+b`.
