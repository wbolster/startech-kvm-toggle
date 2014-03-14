=============================
KVM toggling for Startech KVM
=============================

This is a script that toggles a Startech KVM switch to another input source
without having to press the physical button.

Why?
====

* No more arm stretching to reach for the button somewhere on your desk

* No annoying clicking sound of the mechanical button anymore


How to use?
===========

Just run the script.

But this is quite some typing, so usually you would add a custom keybinding in
Gnome (or other desktop environment) to execute this script, and then you will
have a working hot key.


How does it work?
=================

According to the manual, pressing Scroll Lock twice in a row can be used for
this, but this does not work on Linux machines. It seems the KVM does not
actually respond to the Scroll Lock key, but responds to the Scroll Lock LED
light on the keyboard instead. By default this LED does not seem to be used in
Linux desktop environments, so this script explicitly toggles the LED using
``xset``.
