# juke-x1
Linux-based cmus jukebox built into a kiosk with arduino keypad controls

Juke-X1 is a linux machine running cmus with custom
key bindings. The keypad is controlled by an Arduino
microprocessor. The system can be built into a kiosk.

The jukebox main functions are:
- listen to your library in shuffle/non-shuffle mode
(best if your library files are properly tagged).

- add music to a queue and listen to it like a regular jukebox.

Notes:
y-      win-add-p
e-      win-add-q
a-      win-add-l
i-      win-sel-cur

--------------------
re-order keypad- volume +-;
SHIFT- add win-add-p, win-sel-cur
spacebar for tree view

-------------------
FRAME
mobile; milkcrate on wheels?
case with lock to enclose laptop
screen is visible with lid closed
no timeouts, no hibernate, always on, no lock screen
remove monitor stand
mount 45 deg; add LEDs
--------------------
Alpha machine specs:
Dell D600 laptop 
32 bit single core
Intel(R) Pentium(R) M processor 1.80GHz
512 RAM
80 GB HD

OS- xubuntu 14.04
Once all is configured, edit grub to start in text mode.
(http://ubuntuhandbook.org/index.php/2014/01/boot-into-text-console-ubuntu-linux-14-04/);
To make Ubuntu do nothing when laptop lid is closed -->
sudo -H nano /etc/systemd/logind.conf | add line, HandleLidSwitch=ignore | restart with sudo restart systemd-logind;
Issue-
Screen still goes blank over time in terminal, but music still audible; trying to keep the screen active; 
Ran this:
setterm -blank 0 -powersave off -powerdown 0
//addtl ref at http://ubuntuforums.org/showthread.php?t=2172974

External monitor resolution was not recognized. Ran this to fix:
http://superuser.com/questions/155004/switch-monitors-from-the-command-line
xrandr --output VGA-0 --auto
xrandr --output LVDS --off
-----
Notes from user test
-build metal pipe frame
custom DIY button matrix
https://iamzxlee.wordpress.com/2013/07/24/4x4-matrix-keypad/
secure base
wheels
remote control frame
cmus gui; remote
migrate to raspberry pi 2
install xscreensaver
add 'click button' to xscreensaver
or create script so window doesnt blank after power on




