 Moin and welcome to Gosu!

 Gosu's main website is http://www.libgosu.org/, which always has the latest
links to all relevant information.

 The actual source code, wiki, issue tracker etc. are all hosted on GitHub:

    http://github.com/jlnr/gosu/

 The best entry point into Gosu's documentation is the wiki home page:

    http://github.com/jlnr/gosu/wiki

 Try doing the tutorial there if you don't know how to start out. Or look at
one of the games in the Gosu Users board.

 Remember that Gosu is licensed under the MIT license and feel invited to fork,
port and transmogrify all parts of it. The only license that may affect you by
indirection is libogg's (BSD-style). If you release a Gosu game in any common
binary form, you will need to mention use of libogg and libvorbis somewhere.
 
 Complaints, questions, feedback?
* Visit the boards,                         http://www.libgosu.org/
* try your luck in the chat,              irc://irc.freenode.org/gosu
* or e-mail me. Have fun, write games!         julian@raschke.de

===========
About this Raspberry Pi Prototype branch

This Raspberry Pi Prototype branch, forked from the original SDL2 branch, is an unofficial prototype experiment. The built gem package was tested under the below environment.

Raspberry Pi Type B Rev.2 + Raspbian + Ruby 2.0.0p451
Linux raspberrypi 3.10.25+ #622 PREEMPT Fri Jan 3 18:41:00 GMT 2014

prerequisites:
sudo apt-get install libopenal-dev libfreeimage-dev libvorbis-dev libsndfile1-dev
SDL2
SDL2_ttf
glesv1_cm in /opt/vc/lib shipped with raspbian

DISTCC environment *optional

Build and install:
rake linux:package GOSU_RELEASE_VERSION=0.7.99
cd pkg
gem install gosu-0.7.99.gem

Usage:
cd gosu/example
ruby Tutorial.rb
ESC to terminate

Running from LXDE Terminal:
cd gosu/example
SDL_VIDEODRIVER=RPI ruby Tutorial.rb
ESC to terminate and return to LXDE

Masami Yamakawa
Monoxit inc.
