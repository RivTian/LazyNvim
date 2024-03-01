## 开发环境

- WSL2: Manjaro 
- Neovim 0.9.5

```shell
yay -S fd ripgrep lazygit
yay -S neovim

# Make a backup of your current Neovim files:
# required, new machine maybe don't
$ mv ~/.config/nvim{,.bak}
rm -rf ~/.config/nvim

# optional but recommended
$ mv ~/.local/share/nvim{,.bak}
$ mv ~/.local/state/nvim{,.bak}
$ mv ~/.cache/nvim{,.bak}

rm -rf  ~/.local/share/nvim
rm ~/.local/state/nvim
rm ~/.cache/nvim

git clone https://github.com/RivTian/LazyNvim ~/.config/nvim
rm -rf ~/.config/nvim
nvim
```