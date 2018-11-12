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
