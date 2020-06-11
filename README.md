<!-- [![Melpa Status](http://melpa.org/packages/flycheck-guile-badge.svg)](http://melpa.org/#/flycheck-guile) -->

flycheck-guile
===============

This library provides a [flycheck][] checker for the [GNU Guile][guile]
programming language.  It requires a working [Geiser][geiser] configuration, and
runs `guild compile` on your code to collect warnings and errors.

Installation
------------

This package is not yet available on [MELPA][melpa].

To install it manually, download this code, add the directory to your Emacs
`load-path`, and `(require 'flycheck-guile)` somewhere in your Emacs
configuration.

Usage
-----

The checker will automatically activate in `scheme-mode` buffers with
`geiser-mode`, where `guile` is the current scheme implementation.

If it seems like the checker is not working, try running `M-x
flycheck-verify-checker guile` for some diagnostics.

License
-------

This program is free software: you can redistribute it and/or modify it under
the terms of the GNU General Public License as published by the Free Software
Foundation, either version 3 of the License, or (at your option) any later
version.

This program is distributed in the hope that it will be useful, but WITHOUT ANY
WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
PARTICULAR PURPOSE.  See the GNU General Public License for more details.

You should have received a copy of the GNU General Public License along with
this program.  If not, see <http://www.gnu.org/licenses/>.

See [COPYING](COPYING) for details.

Credits
-------

`flycheck-guile` was originally written by Ricardo Wurmus as part of [Guile
Studio][guile-studio].

[flycheck]: https://github.com/flycheck/flycheck
[geiser]: https://www.nongnu.org/geiser/
[guile]: https://www.gnu.org/software/guile/guile.html
[guile-studio]: https://git.elephly.net/software/guile-studio.git
[melpa]: http://melpa.org