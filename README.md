[![MELPA](http://melpa.org/packages/ox-gfm-badge.svg)](http://melpa.org/#/ox-gfm)
# Github Flavored Markdown exporter for Org Mode

This is a small exporter based on the Markdown exporter already existing in
Org mode. It should support the features [listed here](https://help.github.com/articles/github-flavored-markdown/).

## Installation

You can install `ox-gfm` using elpa. It's available on [melpa](http://melpa.org/#/ox-gfm):

<kbd> M-x package-install ox-gfm </kbd>

## Usage

This package adds an Org mode export backend for GitHub Flavored Markdown. You
can read more about [Org mode exporting here.](http://orgmode.org/manual/Exporting.html)

Exporting to Github Flavored Markdown is available through Org
mode's [export dispatcher](http://orgmode.org/manual/The-export-dispatcher.html#The-export-dispatcher)
once `ox-gfm` is loaded. Alternatively, exporting can be triggered by calling the
(autoloaded) function `M-x org-gfm-export-to-markdown`.

If you want to automatically load `ox-gfm` along with Org mode, then you can
add this snippet to your Emacs configuration:

```emacs-lisp
(eval-after-load "org"
  '(require 'ox-gfm nil t))
```
