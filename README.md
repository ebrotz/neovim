# Neovim

This is my personal neovim setup. The initial plugin list was heavily
inspired by [LazyVim](https://www.lazyvim.org/), however I found the sheer amount
of plugins and keybindings too difficult to pick up, so I built this from the
ground up.

This configuration is set up for Neovim >=v0.12 and uses [Pack][pack] for plugin
management.

[pack]: https://neovim.io/doc/user/pack/

## Keybindings

Leader: space

This is not an exhaustive list of keybindings, but should be enough to get
started:

| Binding | Function |
| - | - |
| `<leader>ff` | Find file |
| `<leader>fg` | Find live grep |
| `<leader>fh` | Find help |
| `<leader>tn` | New floating terminal |
| `<leader>ts` | Select terminal |
| `<leader>ttsn` | Name terminal |
| `<leader>ttta` | Toggle all terminals |

## Plugins

* Completions: [Blink](https://github.com/saghen/blink.cmp)
* Filesystem Navigation: [Oil](https://github.com/stevearc/oil.nvim)
* Fomatting: [Conform](https://github.com/stevearc/conform.nvim)
* Fuzzy Find: [Telescope](https://github.com/nvim-telescope/telescope.nvim)
* [LSP](#lsp)
* Source Control: [LazyGit](https://github.com/kdheepak/lazygit.nvim)
* Status line: [Lualine](https://github.com/nvim-lualine/lualine.nvim)
* Theme: [Catppuccin](https://github.com/catppuccin/nvim)
* Tree-sitter management: [nvim-treesitter](https://github.com/nvim-treesitter/nvim-treesitter)

### LSP

* [mason](https://github.com/mason-org/mason.nvim)

* [mason-lspconfig](https://github.com/mason-org/mason-lspconfig.nvim)

* [nvim-lspconfig](https://github.com/neovim/nvim-lspconfig)

### Mason

These are the tools I primarily use for MacOS/Linux development and
are installed via Mason. I do not include them in-code because I do not guarantee
verification across all architectures (ie I use Windows for work).

* Bicep: [bicep-lsp](https://github.com/neovim/nvim-lspconfig/blob/master/lsp/bicep.lua).
Requires manual installation of the LSP and `init.lua` changes, if actually using
this.

* Go: gopls

* Lua: lua_ls

* Markdown: marksman

* OpenAPI: vacuum

* YAML: yaml-language-server

