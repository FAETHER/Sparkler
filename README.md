Sparkler - Nifty little gizmo for amusing your mouse


Produces "sparks" around your mouse pointer in X, similar to those in
"Discworld". Just run it when your X server starts (for example from your
~/.xinitrc) and have fun!


There are two versions of Sparkler:
 * sparkler-root:
 	Draws on the root window, which means the sparkles are behind all
	windows and changes to the root window made by other programs (for
	example a background image rotator or xplanet) are not possible.

 * sparkler-topwin: (which I recommend)
 	Draws on a shaped top-level window, which means that the sparks are
	visible all the time, but it is possible that mouse clicks get blocked
	when you click on a spark, though that occurs very seldom.
	Warning: Due to the bug with xcompmgr the blend will not happen corectly and trasparency will be about %50
	to avoid this use different compositor, for instance picom works correctly.
To build:

make <version>
make install

All you need should be the compiler and xlibs.

Please change INSTALLDIR in the Makefile, if you want "make install" to copy the
binary to a different location than /usr/local/bin.

If you want to experiment a bit, there are some constants at the top of the
source files you can modify (number of sparks, lifetime, ...).

If you have problems with the compilation or any other questions, please send
e-mail:

Christian Reitwiessner <christian@reitwiessner.de>


Or if it concerns the circle distribution of the sparkles, mail to:

Erik OShaughnessy <eriko@schwa.central.sun.com>

<p align="center">
<img src="https://github.com/FAETHER/Sparkler/blob/master/simplescreenrecorder-2019-12-24.gif" href="" height="256">
