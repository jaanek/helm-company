helm-company.el
============

[Helm] interface for [company-mode]

## Requirements

- [Helm]
- [company-mode]

## Installation

## Installation

### Manual

Just drop `helm-company.el`. somewhere in your `load-path`.

```lisp
(add-to-list 'load-path "~/somewhere")
```

### MELPA

If you're an Emacs 24 user or you have a recent version of package.el
you can install `helm-company.el` from the [MELPA](http://melpa.milkbox.net/) repository.

## Configuration

Add the following to your Emacs init file.

### Manual

    (require 'helm-company)
    (eval-after-load 'company
      '(define-key company-active-map (kbd "C-:") 'helm-company))

### MELPA

    (eval-after-load 'company
      '(define-key company-active-map (kbd "C-:") 'helm-company))

## Usage

####  `helm-company`

Select `company-complete` candidates by [`helm`][helm].
It is useful to narrow campany candidates.

[Helm]:http://emacs-helm.github.io/helm/
[company-mode]:http://company-mode.github.io/
