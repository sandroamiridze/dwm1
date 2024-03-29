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

![nowindows](https://github.com/sandroamiridze/dwm1/assets/110345189/c6d55826-483c-45b4-ae3c-da2bfa460335)

![windowf](https://github.com/sandroamiridze/dwm1/assets/110345189/d9d2da70-60a4-4d36-b7e0-81997e5e20d0)

![2024-03-17-174636_1366x768_scrot](https://github.com/sandroamiridze/dwm1/assets/110345189/706773a0-ecf6-404a-a1ec-159a539a6e78)
