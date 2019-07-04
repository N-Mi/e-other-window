# e-other-window
e-other-window.el --- flash windows when you change to them

This is a small usefull Emacs package from Kevin A. Burton that flashes the current window when switching from a window to another using a keybinding.

Upstream URL has been broken for years (at least 2006), and I preciously kept this file to install it from computers to computers. I thought maybe somebody could be interested in this usefull piece of code. As of now, it's working fine on my current Emacs26.

Here is how I configure it in `.emacs` file (you may adapt the keybinding as your needs) :
```
;; load e-other-window
;;
(load-file "~/.emacs.d/e-other-window.el")

;; cycle through windows using C-$ and C-*
(global-set-key [?\C-\*] `e-other-window)
(global-set-key [?\C-\$]
                '(lambda () (interactive) (e-other-window -1)))

```
