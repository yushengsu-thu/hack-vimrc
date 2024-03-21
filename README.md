# Hack your personal vim
- You could download sheng_vimrc and paste its context to ~/.vimrc


# Requirent
- (basic packages) Download Vim-plug and follow the instructions at [link](https://github.com/junegunn/vim-plug.git)
```bash
source ~/.vimrc
```
- (coc.nvim package) If you could install nodejs follow this [link](https://github.com/neoclide/coc.nvim). If you cannot install nodejs please use nvm as follows:
```bash
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.1/install.sh | bash
```
- (coc.nvim package) Then, restart your terminal or server. And then,
```bash
nvm install node
nvm install 14.17.0
```

# Install pacakges
- (coc.nvim package) Get into the `~/.vimrc` and add
```bash
plug 'neoclide/coc.nvim', {'branch': 'release'}
```
- Finally, execute the following command in `~/.vimrc`:
```bash
:PlugInstall
:PlugUpdate
```
