dwm - dynamic window manager
============================
dwm is an extremely fast, small, and dynamic window manager for X.


Requirements
------------
In order to build dwm you need the Xlib header files.


Installation
------------
Edit config.mk to match your local setup (dwm is installed into
the /usr/local namespace by default).

Afterwards enter the following command to build and install dwm (if
necessary as root):

    make clean install


Running dwm
-----------
Add the following line to your .xinitrc to start dwm using startx:

    exec dwm

In order to connect dwm to a specific display, make sure that
the DISPLAY environment variable is set correctly, e.g.:

    DISPLAY=foo.bar:1 exec dwm

(This will start dwm on display :1 of the host foo.bar.)

In order to display status info in the bar, you can do something
like this in your .xinitrc:

    while xsetroot -name "`date` `uptime | sed 's/.*,//'`"
    do
    	sleep 1
    done &
    exec dwm


Configuration
-------------
The configuration of dwm is done by creating a custom config.h
and (re)compiling the source code.

Some ScreenShots For You
------------------------

![desktopw](https://github.com/sandroamiridze/dwm1/assets/110345189/4accc23e-24b7-4603-b3b4-342a353d305d)

![desktop](https://github.com/sandroamiridze/dwm1/assets/110345189/88e8aa7b-846b-4125-9548-cf4cba11f73c)

![desktopw2](https://github.com/sandroamiridze/dwm1/assets/110345189/b156c88f-b2b9-4896-afb0-830c786df1f1)
