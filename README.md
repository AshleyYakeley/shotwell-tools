# shotwell-tools
Tools to help manage Shotwell photo libraries.
They only work with Shotwell library database schema version 20 (don't worry, they'll check for you).
Shotwell 0.18.0, at least, uses version 20.

**These tools might corrupt your library database.**
Make a back-up of your `photo.db` before using them.

## sw-consolidate
Give it a directory `DIR`, and it will move all photos and videos into directories of the form `DIR/year/month/day/`.
Also attempts to fix up dates.

## sw-merge
Give it the data directory of another Shotwell library, and it will merge it into your own Shotwell library.
It won't move files (use sw-consolidate for that), just merge in the library database.
