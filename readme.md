Installation
============

Prerequisites
-------------
- Python 2.5+
- Twisted 8.2.0+
- pywin32 (Windows only)

Java and Mercurial are recommended as well, but not required.


System Requirements
-------------------
The backend should run on anything that supports Python and Twisted.
It has been tested on Linux, FreeBSD and Windows (XP and above).

The frontend has been tested on IE6, IE7, IE8, Firefox 3, Opera 10, Safari and Chrome.

Setup
-----
- Copy `config.py.example` to `config.py` and customize to fit your setup.
- Run `compile.py` to generate the HTML, minify the JavaScript/CSS, and copy the output to the correct locations.
- Run run.py. If you see an error about the select reactor being registered already, just run it again.
  Note that run.py has lots of arguments; you can see them with `--help`.
- Browse to `http://yourmachine:9090/`.

Development
-----------
Make symlinks as follows in the root directory

	ln -s static/js/debug js
	ln -s static/css/debug css

This will allow you to see changes without running `compile.py` every time.

See `http://instance/quidebug.html` for debug output or something.
It's not yet clear what this page is supposed to do.


FAQ
===

For answers to questions not covered here, see the [qwebirc FAQ](http://qwebirc.org/faq).