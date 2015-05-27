# vim-css-shorthand

Type faster by shorthand that will auto-expand as you type. Supports less, sass, scss, stylus, and plain CSS.

![](https://raw.githubusercontent.com/rstacruz/vim-css-shorthand/gh-pages/screencast.gif)

[![Status](https://travis-ci.org/rstacruz/vim-css-shorthand.svg?branch=master)](https://travis-ci.org/rstacruz/vim-css-shorthand)  

## Expansions

* Properties will be auto-completed: `m ` → `margin: `
* Values will be auto-completed: `float:l` → `float: left`
* Default units will be added: `border-radius: 4⏎` → `border-radius: 4px;`
* Shortcuts for common statements are available: `fl⏎` → `float: left;`
* Semicolons are inserted automatically so you can write CSS in one go: `dib` `⏎` `m0a` `⏎`
* ...and more

| Shortcut     | Expansion              |
| ---          | ---                    |
| `dib`        | display: inline-block; |
| `m0`         | margin: 0;             |
| `m0a`        | margin: 0 auto;        |
| `m-15`       | margin: -15px;         |
| `m:auto`     | margin: auto;          |
| `fle 1 auto` | flex: 1 auto;          |
| `float left` | float: left;           |

## Reference

[See the source](plugin/definitions.py) while I haven't put together something here yet.

## Installation

Using [vim-plug]:

```vim
Plug 'rstacruz/vim-css-shorthand'
```

This requires vim with Python support.

 * Neovim: `:help nvim-python`
 * Howebrew: `brew install macvim --with-cscope --with-lua --override-system-vim --with-luajit --with-python3 --with-python` ([info](http://ricostacruz.com/til/use-macvim-with-lua.html))

Caveats:

* Not fully functional when [auto-pairs] is installed along with it (conflict in the `<Space>` binding). PR's welcome!

## Thanks

**vim-css-shorthand** © 2015+, Rico Sta. Cruz. Released under the [MIT] License.<br>
Authored and maintained by Rico Sta. Cruz with help from contributors ([list][contributors]).

> [ricostacruz.com](http://ricostacruz.com) &nbsp;&middot;&nbsp;
> GitHub [@rstacruz](https://github.com/rstacruz) &nbsp;&middot;&nbsp;
> Twitter [@rstacruz](https://twitter.com/rstacruz)

[MIT]: http://mit-license.org/
[contributors]: http://github.com/rstacruz/vim-css-shorthard/contributors
[auto-pairs]: https://github.com/jiangmiao/auto-pairs
[vim-plug]: https://github.com/junegunn/vim-plug
