# .vim

## Importing my entire Vim setup is as easy as:

```
cd ~			# cd into your home directory
rm -rf .vim
git clone git@github.com:btexpress/.vim.git 
			(or git clone https://github.com/btexpress/.vim.git)
sed -i 's/^M//' .vim/symbolic-link-script           (for MS Windows users using cygwin)
sed -i 's/^M//' .vim/install-vundle-and-vim-plugins (for MS Windows users using cygwin)
sh .vim/symbolic-link-script
sh .vim/install-vundle-and-vim-plugins
```

Two important points:  
1.  Use 'https://github.com/btexpress/.vim.git' instead of 'git@github.com:btexpress/.vim.git' for "git clone" argument if you do NOT have ssh keys set up in github.com

1.  You CANNOT cut and paste the '^M' characters in the 'sed' lines.  You have to type them in manually.  To enter '^M', type CTRL-V, then CTRL-M. That is, hold down the CTRL key then press V and M in succession.

Here are links to all the plugins installed in this .vimrc:

1.	[Vundle, the plug-in manager for Vim](https://github.com/VundleVim/Vundle.vim).  
1.	[The NERDTree - A tree explorer plugin for vim](https://github.com/scrooloose/nerdtree).  
1.	[Vim python-mode. PyLint, Rope, Pydoc, breakpoints from box](https://github.com/python-mode/python-mode).  
1.	[syntastic - Syntax checking hacks for vim](https://github.com/vim-syntastic/syntastic).  
1.	[Tabular - Vim script for text filtering and alignment](https://github.com/godlygeek/tabular).  
1.	[vim-ansible-yaml - Add additional support for Ansible in VIM](https://github.com/chase/vim-ansible-yaml).  
1.	[yaml-vim - YAML syntax/indent plugin for Vim](https://github.com/mrk21/yaml-vim).  
1.	[NERDTree and tabs together in Vim, painlessly](https://github.com/jistr/vim-nerdtree-tabs).  
1.	[vim-puppet - Puppet niceties for your Vim setup](https://github.com/rodjek/vim-puppet).  
1.	[sensible.vim - a universal set of defaults](https://github.com/tpope/vim-sensible).  
1.	[Rocannon - Vim for Ansible playbooks](https://github.com/MicahElliott/Rocannon).  
1.	[vim-json - A better JSON for Vim](https://github.com/elzr/vim-json).  
1.	[indentLine - A vim plugin to display the indention levels with thin vertical lines](https://github.com/Yggdroot/indentLine).  


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
