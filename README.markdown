OSX Window Sizing
=================

OSX Window Sizing is a set of apps that makes it dead-simple to change the size of 
you windows. At present, it comes with two apps: center and maximize

maximize
--------

Maximize will maximize your windows to full-screen. It will take drawers into consideration
as well, so applications like TextMate will truly fill the screen. This works even in 
applications with Zoom buttons that don't truly maximize (like Safari).

center
------

Center will ask you for a pixel size (e.g. "1024x768") and resize your application window
to that size. It will then center the application on the screen. It defaults to 800x600.

Installation
------------

Install the scripts by typing `rake install` in this directory. This will compile the
applescripts into .scpt files and copy them into your ~/Library/Scripts folder.

Usage
-----

It is recommended that you bind the scripts to shortcut keys in the system. I personally
use `ctrl-shift-M` for maximize and `ctrl-shift-C` for center.

Running `rake install_fastscripts` will download a free app called FastScripts Lite,
mount it, and open the mounted folder so you can complete the installation. This will
provide a menu-bar replacement for the `Scripts` menubar that will allow you to attach
keys to any script.

OSX Window Sizing will only work if the window in question is the front-most window
(future versions might provide support for choosing the window or windows you wish 
to resize).