# CBenoit VIM config

I assume that you are under a Unix based system.

Put .vim folder in your home directory.
`$ mv .vim ~`

To use the .vimrc :
`$ ln -s ~/.vim/.vimrc ~/.vimrc`

Don't hesitate to change anything to fit your needs.

## Installation

Plugins managed using Vundle! You can easily install or remove plugins, and they are installed into ~/.vim/bundle/.
See https://github.com/gmarik/vundle for more information.
Everything will automatically be installed at vim first start with this config.
If you want to remove some plugins, do it before launching vim.
You should restart vim after plugins installation.
If gvim isn't appearing, try to run text based vim from terminal.

### Dependencies

You'll need vim 7.4+ compiled with python and ruby support (if you use all plugins in my .vimrc file).
You can check with `vim --version | grep '+python'` and `vim -- version | grep '+ruby'` or you can use vim command mode : `:echo has('python')` and `:echo has('ruby')`.

## Plugins

+ [Ack](https://github.com/mileszs/ack.vim) — Search for pattern in files.
+ [Airline](https://github.com/bling/vim-airline) — A beautiful status bar.
+ [ctrlp](https://github.com/kien/ctrlp.vim) — Search for files.
+ [Cpp Enhanced Highlight](https://github.com/octol/vim-cpp-enhanced-highlight) — Better C++ highlight.
+ [EditorConfig](https://github.com/editorconfig/editorconfig-vim) — Help to define and maintain consistent coding styles.
+ [Fugitive](https://github.com/tpope/vim-fugitive) — An awesome Git wrapper.
+ [LustyExplorer & LustyJuggler](https://github.com/sjbach/lusty) — A fuzzy file and buffer explorer.
+ [Tabular](https://github.com/godlygeek/tabular) — To align regions of text.
+ [UltiSnips](https://github.com/sirver/ultisnips) — Excellent solution to handle snippets in VIM.
+ [VIM Markdown](https://github.com/plasticboy/vim-markdown) — Support for markdown.
+ [YouCompleteMe](https://github.com/Valloric/YouCompleteMe) — Handle autocompletion.

Colorscheme used :
[Monokai](https://github.com/crusoexia/vim-monokai)

## About auto-completion

To use YouCompleteMe plugin, you'll need to build a third party program. You should read the doc about it with `:help youcompleteme`.
You may need to install extra dependencies.

Some YouCompleteMe alternatives :
+ [neocomplete](https://github.com/Shougo/neocomplete.vim)
+ [supertab](https://github.com/ervandew/supertab)
+ [clang_complete](https://github.com/Rip-Rip/clang_complete)
+ [python-mode](https://github.com/klen/python-mode)
+ [jedi-vim](https://github.com/davidhalter/jedi-vim)
+ [AutoComplPop](https://github.com/vim-scripts/AutoComplPop)

They may fit your needs or not. Just make your choice and modify the .vimrc file.

## About snippets

This config uses SirVer's UltiSnips to handle snippets.
You can learn more about it with `:help UltiSnips` and by looking at its github page [UltiSnips' readme](https://github.com/sirver/ultisnips).
SirVer made some screencasts very useful to start using it.
Since YouCompleteMe already use "Tab" key, I choose "c-j" (Ctrl + J) as UltiSnips' trigger key.
By the way, YouCompleteMe provides a nice completion menu for UltiSnips.

My .vimrc file comes with tons of snippets from [honza repository](https://github.com/honza/vim-snippets).

## Good resources to learn more about VIM editor

+ http://bepo.fr/wiki/Vim : VIM and bépo disposition! [FRENCH]
+ http://vim-fr.org/ : french wiki about VIM. [FRENCH]
+ https://vimebook.com/ : book to start learning how to use VIM. [FRENCH]
+ http://www.vim.org/index.php : official website of course! [ENGLISH]
+ http://vim.wikia.com/ : wiki about VIM. [ENGLISH]
+ http://vim.wikia.com/wiki/Vim_Tips_Wiki : some tips. [ENGLISH]
+ http://vimcasts.org/ : various nice screencasts about VIM. [ENGLISH]

### Inspirations

+ [Fisa VIM config](https://github.com/fisadev/fisa-vim-config)
+ [Axiaoxin VIM config](https://github.com/axiaoxin/vim-settings)
+ [Auto installing Vundle](http://www.erikzaadi.com/2012/03/19/auto-installing-vundle-from-your-vimrc/)
+ [This blog post](http://nvie.com/posts/how-i-boosted-my-vim/)

