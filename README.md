# gtk-variant.el
A package to set the theme variant (titlebar color) of emacs

This plugin uses the xprop command to set an X11 property that some window managers use to set the GTK decorations. This allows for a dark titlebar, which this plugin sets by default.
This plugin will stop working on wayland if Emacs ever moves to wayland.

Usage:
```elisp
(add-hook 'window-setup-hook #'gtk-variant-set-frame)
(add-hook 'after-make-frame-functions #'gtk-variant-set-frame)
```
