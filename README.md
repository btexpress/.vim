# .vim

## Importing my entire Vim setup is as easy as:

```
cd ~			# cd into your home directory
rm -rf .vim
git clone git@github.com:btexpress/.vim.git 
			(or git clone https://github.com/btexpress/.vim.git)
sh .vim/symbolic-link-script
sh .vim/install-vundle-and-vim-plugins
```

Use 'https://github.com/btexpress/.vim.git' instead of 'git@github.com:btexpress/.vim.git' for "git clone" argument if you do NOT have ssh keys set up in github.com

Here are links to all the plugins installed in this .vimrc:

[Vundle, the plug-in manager for Vim](https://github.com/VundleVim/Vundle.vim).
[The NERDTree - A tree explorer plugin for vim](https://github.com/scrooloose/nerdtree).
[Vim python-mode. PyLint, Rope, Pydoc, breakpoints from box](https://github.com/python-mode/python-mode).
[syntastic - Syntax checking hacks for vim](https://github.com/vim-syntastic/syntastic).
[Tabular - Vim script for text filtering and alignment](https://github.com/godlygeek/tabular).
[vim-ansible-yaml - Add additional support for Ansible in VIM](https://github.com/chase/vim-ansible-yaml).
[yaml-vim - YAML syntax/indent plugin for Vim](https://github.com/mrk21/yaml-vim).
[NERDTree and tabs together in Vim, painlessly](https://github.com/jistr/vim-nerdtree-tabs).
[vim-puppet - Puppet niceties for your Vim setup](https://github.com/rodjek/vim-puppet).
[sensible.vim - a universal set of defaults](https://github.com/tpope/vim-sensible).
[Rocannon - Vim for Ansible playbooks](https://github.com/MicahElliott/Rocannon).
[vim-json - A better JSON for Vim](https://github.com/elzr/vim-json).
[indentLine - A vim plugin to display the indention levels with thin vertical lines](https://github.com/Yggdroot/indentLine).


#### Disregard all text below.  'YouCompleteMe' plugin has been temporarily disabled.

Extra steps needed for using the 'YouCompleteMe' plugin:

```
sudo apt install build-essential cmake python3-dev
cd ~/.vim/bundle/YouCompleteMe
python3 install.py --all
```
If 'YouCompleteMe' or any other plugin is not desired, you can edit your '~/.vimrc' and comment the plugin out by putting a double quote at the beginning of the line the plugin is invoked; e.g.,
```
" Plugin 'Valloric/YouCompleteMe'
```

For a more detailed explaination of the 'YouCompleteMe' plugin, or any problems with it, see https://github.com/Valloric/YouCompleteMe
