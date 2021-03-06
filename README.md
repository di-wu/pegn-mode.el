# PEGN-mode

This is an Emacs mode for editing PEGN grammars.

## Features
- [x] Simple Syntax Highlighting
- [ ] Indentation

## Installation

### Manual

Check out the repository, add it to your load path and configure Emacs to automatically load it when opening a .pegn file:

``` emacs-lisp
(add-to-list 'load-path "/path/to/pegn/mode/")
(autoload 'pegn-mode "pegn-mode" nil t)
(add-to-list 'auto-mode-alist '("\\.pegn\\'" . pegn-mode))
```

Restart Emacs or evaluate the statements with `C-x C-e`.

### Tokens and Classes

```elisp
; use regexp-opt to generate the regex below.
; 1. M-x eval-expression
; 2. (regexp-opt '("LIST" "OF" "WORDS"))
; 3. wrapped in < and > to indicate only surrounded by space or beginning/end-of-file.
```
