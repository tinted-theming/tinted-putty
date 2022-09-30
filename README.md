base16-putty
============

Base16 colors for PuTTY


Introduction
------------

This project provides `.reg` files for configuring PuTTY colors according to
the `base16 system`, originally created by
[Chris Kempson](https://github.com/chriskempson/base16).

This repository is based on @staticland's [original work](https://github.com/staticaland/base16-putty),
by adding a template that can be used to rebuild the themes.


Usage
-----

1. Make sure to have the most recent stable version of PuTTY;
2. Make sure that your version is
   [configured](http://www.grok2.com/blog/2013/12/01/putty-linux-terminal-xterm-emacs-256-colors/)
   to [provide](https://sanctum.geek.nz/arabesque/putty-configuration/)
   256 colors support;
3. Choose your theme from the [base16-gallery](https://base16-project.github.io/base16-gallery/);
4. Locate the corresponding file in `putty` directory and download it;
5. Edit the file, and change session name in
   `[HKEY_CURRENT_USER\Software\SimonTatham\PuTTY\Sessions\` **`{{SESSION_NAME}}`** `]`
   to the session you would like to apply the theme;
6. Run the file and accept it make changes in Windows Registry...


Rebuild
-------

1. Install [base16-builder-go](https://github.com/base16-project/base16-builder-go)
   or a compatible tool.
   (Note that in the case of `base16-builder-go`
   the [releases' page](https://github.com/base16-project/base16-builder-go/releases)
   contains pre-built binaries that can be simply downloaded and executed).
2. Execute the `builder` binary from the `base16-putty` directory.
   In the case of `base16-builder-go` no argument is required.
3. Check if updates took place (new/modified files are placed inside the `putty` directory)...


Issues or Contributions
------------------------

Please have a look on [these guides](https://opensource.guide/how-to-contribute/) for more information.


Thanks
------

- @staticaland for the [original material](https://github.com/staticaland/base16-putty)
  (I would never find out about the `.reg` files...);
- @iamthad and @ticky for [mapping](https://github.com/iamthad/base16-mintty)
  `base16` vars into color names used by PuTTY;
- @chriskempson for the [base16 project](https://github.com/chriskempson/base16)
  and [builder](https://github.com/chriskempson/base16-builder-php)
- The community behind [`base16-builder-go`](https://github.com/base16-project/base16-builder-go)
  and other `base16`/`base16`-inspired tools and schemes.
