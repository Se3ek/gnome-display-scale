# Purpose
This is a pair of scripts to change the GNOME
fractional scaling value to 100 % and to another value.

Main use is to change the scaling to 100 % before launching a game and then back
to the desired value after the game has quit since having fractional scaling
applied can cause games to pick up a wrong resolution.

# Requirements
* Python 3 must be installed on the system
* Right now this only works with Steam since I haven't figured out how to hook into the
launch and termination on other launchers like Heroic.
If anyone is more knowledgeable about this or has an easy way to do this,
please contribute.

# Usage
The scale100.py changes the scaling back to 100 %
so that should be able to stay the same.

The scalealt.py changes to the alternate value (in my personal preference to 125 %).
There, the value can be changed to a different preferred value for the normal desktop.
In both cases the values can be changed by altering the respective constant in the script.

## Scripts to PATH
Symlink the scripts to a folder in the path.
Example:

    ln -s *repo-dir*/gnome-display-scale100 $HOME/bin/gnome-display-scale100
    ln -s *repo-dir*/gnome-display-scalealt $HOME/bin/gnome-display-scalealt

## Scripts to Games
Add the scripts to the Game commands for each game this should apply to like this:

    gnome-display-scale100; %command%; gnome-display-scalealt

# Disclosure
I took the base of this script off a post on the Internet and modified it to fit my purpose.
