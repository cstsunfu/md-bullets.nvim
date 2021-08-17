# md-bullets.nvim

This plugin is a clone of [org-bullets](https://github.com/akinsho/org-bullets.nvim). PS: Almost all code is copied directly from the origin repo.
This plugin is used for markdown.

## Pre-requisites

- neovim 0.5+

## Installation

The last symbols is displayed for list.

```lua
use {"cstsunfu/md-bullets.nvim", config = function()
  require("org-bullets").setup {
    symbols = { "◉", "○", "✸", "✿" }
    -- or a function that receives the defaults and returns a list
    symbols = function(default_list)
      table.insert(default_list, "♥")
      return default_list
    end
  }
end}

```
