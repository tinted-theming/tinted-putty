base16-putty
============

Base16 colors for PuTTY


Introduction
------------

This project provides `.reg` files for configuring PuTTY colors
according to the `base16 system`.


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
6. Run the file and accept it to make changes in Windows Registry.


Issues or Contributions
------------------------

This repo rebuilds the colorschemes every week, so make sure to pull to
keep up to date with the latest changes.

If you're you're looking to build the colorschemes manually to test out
a change:

1. Install [base16-builder-go](https://github.com/base16-project/base16-builder-go)
   or a compatible tool.
   (Note that in the case of `base16-builder-go`
   the [releases' page](https://github.com/base16-project/base16-builder-go/releases)
   contains pre-built binaries that can be simply downloaded and executed).
2. Execute the `builder` binary from the `base16-putty` directory.
   In the case of `base16-builder-go` no argument is required.
3. Check if updates took place (new/modified files are placed inside the `/putty` directory).

Have a look at [these guides](https://opensource.guide/how-to-contribute/) for more information.


Thanks
------

- @staticaland for the [original .reg material](https://github.com/staticaland/base16-putty)
