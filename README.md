# 💻 Tmux Configuration

A modular and aesthetic `tmux` setup managed by **TPM (Tmux Plugin Manager)**. This configuration focuses on a clean UI using the **Catppuccin** theme and workflow persistence.

<img src="https://raw.githubusercontent.com/GabrielAlmeidaFlores/GabrielAlmeidaFlores/refs/heads/main/assets/Tmux-Configuration/Tmux%20Eyeshot.png">

---

## 📦 Core Plugins

Currently, this setup utilizes the following plugins to enhance navigation and session management:

| Plugin | Description |
| --- | --- |
| [tpm](https://github.com/tmux-plugins/tpm) | The essential plugin manager for Tmux. |
| [vim-tmux-navigator](https://github.com/christoomey/vim-tmux-navigator) | Seamless navigation between Vim/Neovim and Tmux panes. |
| [catppuccin/tmux](https://github.com/catppuccin/tmux) | Soothing pastel theme (v2.1.2) for the terminal. |
| [tmux-resurrect](https://github.com/tmux-plugins/tmux-resurrect) | Persists tmux environments across system restarts. |
| [tmux-continuum](https://github.com/tmux-plugins/tmux-continuum) | Continuous saving of tmux sessions. |

---

## 🎨 Visuals & UI

The interface is customized with the **Catppuccin Mocha** palette:

* **Window Style:** Modern `rounded` status indicators.
* **Status Bar:** Minimalist design. The right side displays the active **application** and **session name**, while the left remains empty for focus.
* **Persistence:** Automatic restoration is enabled (`@continuum-restore 'on'`), and pane contents are captured during saves.

---

## 🛠️ Setup & Installation

1. **Install TPM:**
```bash
git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm

```


2. **Configuration:**
Add your settings to `~/.tmux.conf`.
3. **Install Plugins:**
* Open a Tmux session.
* Press `Prefix` (default `Ctrl+b`) + `I` (capital I) to fetch and install the plugins.



---

## ⌨️ Shortcuts

* **Navigation:** `Ctrl + h/j/k/l` to move between panes.
* **Save Session:** `Prefix + Ctrl + s` (via Resurrect).
* **Restore Session:** `Prefix + Ctrl + r` (via Resurrect).

> **Note:** The TPM initialization line must always remain at the very end of your configuration file.
