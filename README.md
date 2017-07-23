## My Vim Configs

### Usage

#### clone this repo
```sh
git clone https://github.com/padma0/vim.git ~/.vim
```
Open vim and then run `:PlugInstall`. After that, quit vim and create some dirs:
#### make a symbolic link to vimrc
```sh
ln -s .vim/vimrc .vimrc
```
#### Adding new stuff
1. Add plugins to ~/.vim/.vimrc-plug
2. Set colorscheme at ~/.vim/vimrc-colors
3. Add keymaps to ~/.vim/vimrc-maps

#### Code Completion
YouCompleteMe provides code completion for several languages, including go and C-family. In order to code completion to work, you should follow some steps. Detailed explanation is on their github repository page: [https://github.com/Valloric/YouCompleteMe]

There are also some code snippets available, provided by **ultisnips** and **vim-snippets** plugins.

### Some key-bindings

#### Leader Key
The leader key is mapped to **space**. To change it, just go to **vimrc-set** file.

#### Directory Tree (NERDTree)
To open, just hit **space+e**, then hit **o** to open a file or directory. For more commands, type '?' while nerdtree is open.

#### Switch between buffers
Since I usually create lots of buffers, I prefer to use ctrlp to search them, just hit **space+b** to show all opened buffers and search them. If you prefer tabline, take [vim-buftabline](https://github.com/ap/vim-buftabline) a try

#### Fuzzy file search
Use **CTRL+p** and type the name of the file you want.

#### Searching
Search file content is provided by CtrlSF plugin. To do a quick file search, just type **<leader>f**

#### Expand code snippets
To expand suggested code snippets, just select the snippet with tab and press **<c-j>**
