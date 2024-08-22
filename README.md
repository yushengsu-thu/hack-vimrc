# Hack your personal vim
- You could download sheng_vimrc and paste its context to `~/.vimrc`


# Requirent
- (basic packages) Download Vim-plug and follow the instructions at [link](https://github.com/junegunn/vim-plug.git)
```bash
curl -fLo ~/.vim/autoload/plug.vim --create-dirs \
    https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim
```
and then `vim ~/.vimrc`
```vim
:PlugInstall
:PlugUpdate
```
and then
```bash
source ~/.vimrc
```

- (coc.nvim package) If you could install `nodejs` follow this [link](https://github.com/neoclide/coc.nvim). If you cannot install `nodejs` please use nvm as follows:
```bash
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.1/install.sh | bash
```

- After the installation, you may need to close and reopen your terminal, or you can run the following to make `nvm` available in the current session:
```bash
export NVM_DIR="$([ -z "${XDG_CONFIG_HOME-}" ] && printf %s "${HOME}/.nvm" || printf %s "${XDG_CONFIG_HOME}/nvm")"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"  # This loads nvm
```
- Once installed, verify the installation with:
```
nvm --version
```

- (coc.nvim package) Then, restart your terminal or server. And then,
```bash
nvm install node
nvm install 14.17.0
```

# Install packages
- (coc.nvim package) Get into the `~/.vimrc` and add
```bash
Plug 'neoclide/coc.nvim', {'branch': 'release'}
```
- Finally, execute the following command in `~/.vimrc`:
```bash
:PlugInstall
:PlugUpdate
```

# Note that:
After installing the `coc.nvim`, you gotta change the config in `~/.vimrc`. You can find the example in this [link](https://github.com/neoclide/coc.nvim). But I haven't added this part into my '~/.vimrc'. I gotta deal with some redundant parts (ex. remove ctags configs) and conflict isses to merge it. 


