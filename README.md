# avy-flycheck
`avy-flycheck` is a GNU Emacs package for syntax errors navigation. It depends on `flycheck` to provide syntax error checking and `avy` for easy navigation.

Jump to and fix syntax errors using `flycheck` with `avy` interface

## Configuration overview

### add path of this package to your `load-path`
```elisp
(add-to-list 'load-path
	     "path/to/the/directory/of/avy-flycheck")
```
then simply `require` the package
```elisp
(require 'avy-flycheck)
```

### bind to a key for your convenience.
>you can choose your own binding.
```elisp
(global-set-key (kbd "C-c ;") #'avy-flycheck-goto-error)
```

### A few customizations are provided.
>Set Method for displaying avy overlays.
```elisp
(setq avy-flycheck-style 'pre)
```

## Contributing

### Copyright Assignment

`avy-flycheck` is subject to the same [copyright assignment](http://www.gnu.org/prep/maintain/html_node/Copyright-Papers.html) policy as Emacs itself, org-mode, CEDET and other packages in [GNU ELPA](http://elpa.gnu.org/packages/). Any [legally significant](http://www.gnu.org/prep/maintain/html_node/Legally-Significant.html#Legally-Significant) contributions can only be accepted after the author has completed their paperwork. Please see [the request form](http://git.savannah.gnu.org/cgit/gnulib.git/tree/doc/Copyright/request-assign.future) if you want to proceed.

The copyright assignment isn't a big deal, it just says that the copyright for your submitted changes to Emacs belongs to the FSF. This assignment works for all projects related to Emacs. To obtain it, you need to send one email, then send one letter (if you live in the US, it's digital), and wait for some time (in my case, I had to wait for one month).

### Style

Use your own judgment for the commit messages, I recommend a verbose style using `magit-commit-add-log`.
