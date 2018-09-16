### muttrc-mode
major mode for editing muttrc

#### Documentation:

To build the info file:
  `makeinfo muttrc-mode.texi -o muttrc-mode.info`

Install it to the system INFOPATH:
  `install -o root -g root -m644 muttrc-mode.info /usr/share/info/muttrc-mode.info`

#### Installation:

Add these lines to your Emacs config:
```elisp
  (autoload 'muttrc-mode "muttrc-mode.el"
        "Major mode to edit muttrc files" t)
  (setq auto-mode-alist
            (append '(("muttrc\\'" . muttrc-mode))
                    auto-mode-alist))
```
Install muttrc-mode.el to a directory somewhere in Emacs' load-path.

#### Limitations:

- Multiline commands are not properly handled and their use can lead
  to unexpected results.
