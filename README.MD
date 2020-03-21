# Sparen's Script Skeleton

After what seems to have been ages of copying over prior work and then spending hours and hours tearing through it in order to swap graphics and the like, my BHA entry proved that if I really want to iterate fast, I need two things.

One, a standard library and setup that has some form of organization but which is not tied to any strict implementation.

Two, no package, since adding a package effectively means adding hours onto logistics and replacing placeholder graphics while coupling me to whatever system I have in use.

This Script Skeleton aims to bring sanity back to my scripting by allowing me all the flexibility I had way back when I was starting out with ph3 while also providing me with all of the libraries I need (as well as a common repository for templating and iterating on those templates).

### Notes

- No scores are kept. In fact, no persistent CommonData is used at all besides storing the user's replay name and their spell history.
- Since there is no package, there are no continues. Some minor hooks (e.g. End Scene) still have provisions for continue checking. 
- Only CommonData remaining are those used for tracking spell/life fragments, those used for tracking which boss is currently present, and minor dialoge event trackers. All graphical effects are enabled (it has been years; computers should be good enough to handle the 'moderately advanced' effects I began using half a decade ago).
- Finally using a lib folder for all random function libraries with high potential for actual refactoring. Everything is at some point planned for switchover to .dnh
- Some things *need* to be custom implemented, such as boss animations. These need to be filled out manually.  