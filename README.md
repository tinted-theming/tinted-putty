tinted-putty
============

[Base16] and [Base24] colors for [PuTTY]


Introduction
------------

This project provides `.reg` files for configuring PuTTY colors
according to the `base16 system` and `base24 system`.

This repo was originally named `base16-putty`, but since we've now got
the added [Base24] template and theme support, and maybe different ones
in future, we renamed to `tinted-putty` so we don't lock ourselves into
a single scheme system.


Usage
-----

1. Make sure to have the most recent stable version of PuTTY;
2. Make sure that your version is [configured] to [provide] 256 colors
   support;
3. Choose your theme from the [base16-gallery];
4. Locate the corresponding file in `putty` directory and download it;
5. Edit the file, and change session name in
   `[HKEY_CURRENT_USER\Software\SimonTatham\PuTTY\Sessions\` **`{{SESSION_NAME}}`** `]`
   to the session you would like to apply the theme;
6. Run the file and accept it to make changes in Windows Registry.


Issues or Contributions
-----------------------

This repo rebuilds the colorschemes every week, so make sure to pull to
keep up to date with the latest changes.

If you're you're looking to build the colorschemes manually to test out
a change:

1. Install [builder-rust] or a compatible tool.
2. Execute `tinted-builder-rust build path/to/tinted-putty`
3. Check if updates took place (new/modified files are placed inside the `/putty` directory).

Have a look at [these guides] for more information.

Thanks
------

- @staticaland for the [original material](https://github.com/staticaland/base16-putty);
- @iamthad and @ticky for [mapping](https://github.com/iamthad/base16-mintty) `base16` vars into color names used by PuTTY;
- @chriskempson for the original conception of the [tinted-theming](https://github.com/tinted-theming/home).

[Base16]: https://github.com/tinted-theming/home
[Base24]: https://github.com/tinted-theming/base24
[PuTTY]: https://en.wikipedia.org/wiki/PuTTY
[base16-gallery]: https://tinted-theming.github.io/base16-gallery/
[configured]: https://web.archive.org/web/20140803065929/http://www.grok2.com/blog/2013/12/01/putty-linux-terminal-xterm-emacs-256-colors/
[provide]: https://sanctum.geek.nz/arabesque/putty-configuration/
[these guides]: https://opensource.guide/how-to-contribute/
[builder-rust]: https://github.com/tinted-theming/tinted-builder-rust
[releases' page]: https://github.com/tinted-theming/tinted-builder-rust/releases
