# Dotfiles

Configurazione personale per Ubuntu/WSL con Zsh, Tmux, WezTerm e Hyprland.

## ⚡ Requisiti

- Ubuntu 22.04/24.04 (o WSL2)
- Git
- Curl

## 🚀 Installazione

```bash
git clone https://github.com/tuousername/dotfiles.git ~/dotfiles
cd ~/dotfiles
./install.sh
```

## 📁 Struttura

| Componente | Descrizione |
|------------|-------------|
| `zsh/` | Configurazione Zsh con autosuggestions e syntax highlighting |
| `tmux/` | Configurazione Tmux con tema Catppuccin e plugins |
| `wezterm/` | Configurazione terminale WezTerm |
| `starship/` | Prompt Starship con tema Catppuccin |
| `hypr/` | Configurazione Hyprland (solo Linux nativo) |
| `waybar/` | Barra di stato per Wayland |
| `rofi/` | Launcher di applicazioni |
| `btop/` | Monitor di sistema |

## 🐧 Note su WSL

Su WSL alcune funzionalità GUI (Hyprland, Waybar) non sono disponibili. Lo script installerà automaticamente solo i tool CLI compatibili.

## 🔧 Tool Installati

### CLI
- Zsh + Oh My Zsh plugins
- Tmux + TPM
- Neovim
- Lazygit
- Zoxide
- FZF
- Eza (ls moderno)
- Bat (cat moderno)
- Btop

### GUI (solo Linux nativo)
- Hyprland
- Waybar
- Rofi
- WezTerm
- Swww (wallpaper)

## 📝 Comandi Utili

| Alias | Comando |
|-------|---------|
| `ls` | `eza --all --color=always --long --git --icons=always` |
| `lst` | `eza --tree --level=2 ...` |
| `cat` | `bat` |
| `cd` | `zoxide` |

## ⌨️ Tmux Keybindings

| Tasto | Azione |
|-------|--------|
| `Ctrl+a` | Prefix |
| `Ctrl+a + s` | Split orizzontale |
| `Ctrl+a + v` | Split verticale |
| `Ctrl+a + h/j/k/l` | Navigazione panes |
| `Ctrl+a + o` | Sessionx (switch session) |
| `Ctrl+a + p` | Floax (floating pane) |

## ⚠️ Troubleshooting

### Problema: Starship non si avvia
**Soluzione:** Assicurati che Cargo sia installato: `cargo install starship --locked`

### Problema: Plugin Tmux non caricati
**Soluzione:** Premi `Ctrl+a + I` per installare i plugin TPM

### Problema: Font Nerd non visualizzati
**Soluzione:** Riavvia il terminale o esegui `fc-cache -fv`

## 📄 Licenza

MIT - Fai ciò che vuoi con questa configurazione!
