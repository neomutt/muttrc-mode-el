# muttrc-mode
major mode for editing muttrc

Documentation:

To build the info file:
  makeinfo muttrc-mode.texi

Installation:

Add these lines to your Emacs config:
  (autoload 'muttrc-mode "muttrc-mode.el"
        "Major mode to edit muttrc files" t)
  (setq auto-mode-alist
            (append '(("muttrc\\'" . muttrc-mode))
                    auto-mode-alist))

Install muttrc-mode.el to a directory somewhere in the load-path.
