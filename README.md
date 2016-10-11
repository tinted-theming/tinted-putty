base16-putty
============

Base16 colors for PuTTY


Introduction
------------

This project provides `.reg` files for configuring PuTTY colors according to
[base16](https://github.com/chriskempson/base16).

The [original work](https://github.com/staticaland/base16-putty) from
@staticaland has gotten a little bit outdated and does not cover all the
available themes.


Usage
-----

1. Make sure to have the most recent stable version of PuTTY;
2. Make sure that your version is
   [configured](http://www.grok2.com/blog/2013/12/01/putty-linux-terminal-xterm-emacs-256-colors/)
   to [provide](https://sanctum.geek.nz/arabesque/putty-configuration/)
   256 colors support;
3. Choose your theme from http://chriskempson.github.io/base16/;
4. Locate the corresponding file in `putty` directory and download it;
5. Edit the file, and change session name in
   `[HKEY_CURRENT_USER\Software\SimonTatham\PuTTY\Sessions\` **`{{SESSION_NAME}}`** `]`
   to the session you would like to apply the theme;
6. Run the file and accept it make changes in Windows Registry...


Issues or Contributions
-----------------------

Please follow the [GitHub guide](https://guides.github.com/activities/contributing-to-open-source/).


Thanks
------

- @staticaland for the [original material](https://github.com/staticaland/base16-putty)
  (I would never find out about the `.reg` files...);
- @iamthad and @ticky for [mapping](https://github.com/iamthad/base16-mintty)
  `base16` vars into color names used by PuTTY;
- @chriskempson for the [base16 project](https://github.com/chriskempson/base16)
  and [builder](https://github.com/chriskempson/base16-builder-php)
