[![Melpa Status](http://melpa.org/packages/ibuffer-vc-badge.svg)](http://melpa.org/#/ibuffer-vc)
[![Melpa Stable Status](http://stable.melpa.org/packages/ibuffer-vc-badge.svg)](http://stable.melpa.org/#/ibuffer-vc)
<a href="https://www.patreon.com/sanityinc"><img alt="Support me" src="https://img.shields.io/badge/Support%20Me-%F0%9F%92%97-ff69b4.svg"></a>

# ibuffer-vc: Group buffers in ibuffer list by VC project #

Emacs' `ibuffer-mode` is a wonderful replacement for the built-in
`list-buffer` command, and allows buffers to be grouped
programatically, e.g. by major mode.

If, like me, you mostly work on version-controlled files, you might
like to see your buffers grouped by the associated version control
project.

That's where `ibuffer-vc` comes in: it lets you:

* Group your buffers by their parent vc root directory
* See the VC status of the associated files
* Sort buffers by their VC status
* Display buffer filenames that are relative to their VC root

## Screenshot ##

![ibuffer-vc screenshot](http://i.imgur.com/RUYRJ.png)

## How to install ##

See `ibuffer-vc.el`, or (preferred) install from [MELPA][MELPA].


[MELPA]: http://melpa.org "MELPA"


<hr>


[💝 Support this project and my other Open Source work](https://www.patreon.com/sanityinc)

[💼 LinkedIn profile](https://uk.linkedin.com/in/stevepurcell)

[✍ sanityinc.com](http://www.sanityinc.com/)

[🐦 @sanityinc](https://twitter.com/sanityinc)

## How to install alternative non-ELPA package ##
1. Install in /.emacs.d/site-lisp/
2. Manually generate the ibuffer-vc-autoloads.el file by running (update-directory-autoloads)
3. Manually byte-compile ibuffer-vc.el
4. Remove ELPA version (which will always load first) via (package-list-packages)
5. Update init-ibuffer.el to remove (require-package) statement, which automatically downloads the package from ELPA
