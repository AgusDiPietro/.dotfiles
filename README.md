# Clone the repository and create symbolic links.

```python
export CODE_PATH=$HOME/projects/personal/code

## MacBook and Linux
ln -sf $CODE_PATH/dot-files/zsh/.zshrc ~/.zshrc
ln -sf $CODE_PATH/dot-files/tmux/.tmux.conf ~/.tmux.conf
git clone --depth 1 https://github.com/wbthomason/packer.nvim ~/.local/share/nvim/site/pack/packer/start/packer.nvim
ln -sf $CODE_PATH/dot-files/nvim/* ~/.config/nvim/
ln -sf $CODE_PATH/dot-files/zsh/minimal-char.zsh-theme ~/.oh-my-zsh/themes/minimal-char.zsh-theme
git clone --depth 1 https://github.com/eendroroy/alacritty-theme.git ~/.alacritty-colorscheme
ln -sf $CODE_PATH/dot-files/alacritty/* ~/.config/alacritty/

## Only for linux
ln -sf $CODE_PATH/dot-files/i3wm/i3/config ~/.config/i3/config
ln -sf $CODE_PATH/dot-files/wireplumber ~/.config/wireplumber
ln -sf $CODE_PATH/dot-files/dunst/dunstrc/.config/dunst/dunstrc
ln -sf $CODE_PATH/dot-files/polybar/* ~/.config/polybar/
ln -sf $CODE_PATH/dot-files/autorandr ~/.config/
ln -sf $CODE_PATH/dot-files/rofi/nord.rasi $HOME/.local/share/rofi/themes/
ln -sf $CODE_PATH/dot-files/rofi/config.rasi $HOME/.config/rofi/

## Use gpg with yubi:
gpg --import charlie-gpg-public.asc
gpg --edit-key <ID>
> trust 

https://github.com/drduh/YubiKey-Guide
```
