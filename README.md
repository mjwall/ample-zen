## About

Ample Zen is a theme for Emacs 24.  It is my combination of
ample-theme by Jordon Biondo
(https://github.com/jordonbiondo/ample-theme) and Zenburn-Emacs by
Bozhidar Batsov (https://github.com/bbatsov/zenburn-emacs).  Credit
goes to them, as they did the hard work.

I wanted to combine the colors of AmpleTheme and the robustness of
Zenburn-Emacs.  It has been tested on Mac OSX 10.8 on both the GUI and
terminal. This is my first attempt at a theme.

## Screenshot

![Ample Zen Screenshot](https://raw.github.com/mjwall/ample-zen/master/ample-zen.png
 "Ample Zen Screenshot")

## Installation

Download `ample-zen-theme.el` to a directory like
`~/.emacs.d/themes/`. Then add it your custom load path with something
like the following in your `~/.emacs.d/init.el`:

```lisp
(add-to-list 'custom-theme-load-path "~/.emacs.d/themes/")
```
You can then load the theme interactively like so:

`M-x load-theme RET ample-zen`

or call this in your `~/.emacs.d/init.el`

```lisp
(load-theme 'ample-zen t)
```

### Package.el

If you have the [Marmalade](http://marmalade-repo.org) configured, you
can install this package with the following.

```lisp
M-x package-install ample-zen-theme
```

At the time of this commit, a pull request has been merged to
[MELPA](http://melpa.milkbox.net).  At some point, `package-install
ample-zen-theme` should work from there as well.

## Ugly colors in the terminal Emacs version

If your Emacs looks considerably uglier in a terminal (compared to the
GUI version) try adding this to your `.bashrc` or `.zshrc`:

```bash
export TERM=xterm-256color
```
