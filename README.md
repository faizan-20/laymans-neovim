# laymans-neovim
nvim configurations for a layman
 - easy to use and understandable configurations to build upon or use as it is

![example pic](https://raw.githubusercontent.com/faizan-20/laymans-neovim/main/lm-nvim.png)

# Features
 - Easy to use
 - native lsp with completion and diagnostics
 - powerfull syntax
 - sane defaults
 - looks good

## Requirements
1. Latest stable [neovim](https://github.com/neovim/neovim)

# How to install
1. git clone the repositiory
    
    ```git clone https://github.com/faizan-20/laymans-neovim```

2. copy nvim to ~/.config/
    
    ```cp laymans-neovim/nvim ~/.config```

3. create a folder for plugins
    
    ```mkdir ~/.vim/plugged```

4. open vim
    
    ```:PlugInstall```

## Additional Features / Hacking Guide
init.vim has everything except some plugin specific configurations
which you can find in the directory called Plugin to make it more
readable.

To add more language to LSP service install the proper language protocol ([reference](https://github.com/neovim/nvim-lspconfig/blob/master/CONFIG.md))
and add it to Plugin/lsp.lua
    ```local servers = { 'pyright', 'clangd', 'html' }```

To change/see general keymappings reffer to ```init.vim```
To change/see lsp specific mappings see ```Plugin/lsp.lua```
To change/see completion specific mappings see ```Plugin/nvim-cmp.lua```

To configure/change colorscheme see ```Plugin/color-config.vim```

remove annoying author name or change it to yours by going to 
```Plugin/alpha-nvim.lua``` ;)
