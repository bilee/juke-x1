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
mount 45 deg
leds
--------------------
Alpha machine specs:
Dell D600 laptop 
32 bit single core
Intel(R) Pentium(R) M processor 1.80GHz
512 RAM
80 GB HD

OS- xubuntu 14.04
Once all is configured, edit grub to start in text mode.
(http://ubuntuhandbook.org/index.php/2014/01/boot-into-text-console-ubuntu-linux-14-04/)

