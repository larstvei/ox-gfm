[![MELPA](http://melpa.org/packages/ox-gfm-badge.svg)](http://melpa.org/#/ox-gfm)
# Github Flavored Markdown exporter for Org Mode

This is a small exporter based on the Markdown exporter already existing in
Org mode. It should support the features [listed here](https://help.github.com/articles/github-flavored-markdown/).

## Installation

You can install `ox-gfm` using elpa. It's available on [melpa](http://melpa.org/#/ox-gfm):

<kbd> M-x package-install ox-gfm </kbd>

## Usage

This package adds an Org mode export backend for GitHub Flavored Markdown.

You can read more about [Org mode exporting here.](http://orgmode.org/manual/Exporting.html)

Org mode only loads these backends by default: ascii, html, icalendar, latex and odt

To manually enable this package you can simply require the package:

```emacs-lisp
(require 'ox-gfm)
```

If you want to automatically enable exporting to Github Flavored Markdown, you
can add this snippet in your emacs config:

```emacs-lisp
(eval-after-load "org"
  '(require 'ox-gfm nil t))
```

Once the package is loaded you can use it in Org mode with [the export
dispatcher](http://orgmode.org/manual/The-export-dispatcher.html#The-export-dispatcher).

You can use the exporter with `C-c C-e` or `M-x org-export-dispatch`
