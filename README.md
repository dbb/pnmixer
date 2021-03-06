PNMixer
=======

PNMixer is a simple mixer application designed to run in your system
tray.  It integrates nicely into desktop environments that don't have
a panel that supports applets, and therefore can't run a mixer applet.
In particular it's been used quite a lot with fbpanel and tint2, but
should run fine in any system tray.

PNMixer is a fork of [OBMixer](http://jpegserv.com/?page_id=282) with
a number of additions.  These include: 

- Volume adjustment with the scroll wheel
- Select which ALSA device and channel to use
- Detect disconnect from sound system and re-connect if requested
- Bind and use HotKeys for volume control
- Texual display of volume level in popup window
- Continous volume adjustment when dragging the slider (not just when you let go)
- Draw a volume level onto system tray icon
- Use system icon theme for icons and use mute/low/medium/high
  volume icons
- Configurable middle click action
- Preferences for:
	- volume text display
	- volume text position
	- icon theme
	- amount to adjust per scoll
	- middle click action
	- drawing of volume level on tray icon

Source and so on are at:
[https://github.com/nicklan/pnmixer](https://github.com/nicklan/pnmixer)

Download
--------
Latest version can always be found at:
[https://github.com/nicklan/pnmixer/downloads](https://github.com/nicklan/pnmixer/downloads)

Dependencies
------------

Development files from the following libraries are required to build PNMixer
from source:

* glib2.0
* gtk+2.0

To install them (on a Debian-based system, for example) run:

    aptitude install libglib2.0-dev libgtk2.0-dev

In total, these packages and their dependencies will require approximately 
**40MB** of disk space, but they can be uninstalled after compilation is 
complete.

Compilation and Install
-----------------------
To install this program cd to this directory and run:

./autogen.sh

make

sudo make install
