This is a pair of scripts to change the GNOME
fractional scaling value to 100 % and to another value.

Main use is to change the scaling to 100 % before launching a game and then back
to the desired value after the game has quit.

# Usage
The scale100.py changes the scaling back to 100 %
so that should be able to sta the same.

The scale125.py changes to the alternate value (in my preference to 125 %).
There, the value can be changed to a different preferred value for the normal desktop.

## Scripts to PATH
Symlink the scripts to a folder in the path.
Example:

    ln -s *repo-dir*/gnome-display-scale100 $HOME/bin/gnome-display-scale100

## Scripts to Games
Add the scripts to the Game commands for each game this should apply to like this:

    gnome-display-scale100; %command%; gnome-display-scale125
