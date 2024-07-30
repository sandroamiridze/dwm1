dwm - dynamic window manager
============================
This is my dwm .config which is an extremely fast, small, and dynamic window manager for X.


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
![awesame2](https://github.com/user-attachments/assets/e99b44b0-af52-4817-8cd1-d08244a03c82)

![awesame5](https://github.com/user-attachments/assets/218a70cf-4101-4ce0-b1f2-a2871162fe4f)

![awesame4](https://github.com/user-attachments/assets/ffb02fdd-17b4-4ba8-8fd5-b02e54d4abeb)

![awesame3](https://github.com/user-attachments/assets/46c00ad7-c1d8-433c-b5d5-b01b1b77687f)

![awesome](https://github.com/user-attachments/assets/98696eb6-2b0c-43a7-977f-7f3206d624ca)

----------------------
