## My Vim Configs

### Usage

#### 0. requirement
- neovim
- [ripgrep](https://github.com/BurntSushi/ripgrep)
```sh
brew install neovim
brew install ripgrep
brew install yarn
brew install python
pip3 install neovim
```
#### 1. install plugins
```sh
git clone https://github.com/padma0/vim.git ~/.vim
ln -s ~/.vim ~/.config/nvim
nvim +PlugInstall
:CocInstall coc-marketplace coc-eslint coc-snippets coc-emmet coc-prettier coc-json coc-css coc-tsserver coc-elixir coc-diagnostic
```

### More details

#### Leader Key
The leader key is mapped to **comma**. To change it, just go to **vimrc-set** file.

#### Code Completion
The most powerful [auto-complete plugin](https://github.com/Shougo/neocomplete.vim), compatible with [vim-snippets](https://github.com/honza/vim-snippets).
There are also completion of words in adjacent tmux panes, provided by [tmux-complete.vim](https://github.com/wellle/tmux-complete.vim).

#### Directory Tree (NERDTree)
To open, just hit **Ctrl+e**, then hit **o** to open a file or directory. For more commands, type '?' while nerdtree is open.

#### Switch between buffers
Since I usually create lots of buffers, I prefer to use ctrlp to search them, just hit **space+b** to show all opened buffers and search them. If you prefer tabline, take [vim-buftabline](https://github.com/ap/vim-buftabline) a try

#### Fuzzy file search
Use **CTRL+p** or **space+p** and type the name of the file you want. For recent opened files, just use **space+r**.

#### Searching
Search file content is provided by CtrlSF plugin. To do a quick file search, just type **Ctrl-a**
