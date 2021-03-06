# MAPTOOL

Maptool is a small tool to generate nethack-style ASCII dungeons.
It is a WIP at the moment so expect breaking changes and bugs.

**LICENSE:** MIT see [LICENSE](https://github.com/dragonchaser/maptool/blob/master/LICENSE) file in this repository.

## usage

```
Usage: ./maptool.rb [options]
    -r, --rows=ROWS                  Dungeon rows (default: 10)
    -c, --cols=COLS                  Dungeon cols (default: 10)
    -e, --empty=PROBABILTY           Probablility of creating an empty tile (default: 0.02)
    -p, --precision=PRECISION        Precision used for calculationg weighted probablities with -e (default: 2, will resort to defaults if <2 || > 14)
    -b, --border                     Print tile border (default: false)
    -v, --verbose                    Verbose mode
    -V, --superverbose               Super verbose mode
    -h, --help                       Prints this help
```

## examples

### with border

```
.......................................
.            .            .    |~~|    .
.            .            . +--+~~+--+ .
.            .            . |~~~~~~~~| .
.    +-------.------------.-+~~~~~~~~+-.
.    |~~~~~~~.~~~~~~~~~~~~.~~~~~~~~~~~~.
.    |~~~~~~~.~~~~~~~~~~~~.~~~~~~~~~~~~.
.    |~~+----.------------.-+~~~~~~~~+-.
.    |~~|    .            . |~~~~~~~~| .
.    |~~|    .            . +--+~~+--+ .
.    |~~|    .            .    |~~|    .
........................................
.    |~~|    .            .    |~~|    .
.    |~~|    .            .    |~~|    .
.    |~~|    .            .    |~~|    .
.----+~~+----.------------.----+~~+----.
.~~~~~~~~~~~~.~~~~~~~~~~~~.~~~~~~~~~~~~.
.~~~~~~~~~~~~.~~~~~~~~~~~~.~~~~~~~~~~~~.
.----+~~+----.----+~~+----.----+~~+----.
.    |~~|    .    |~~|    .    |~~|    .
.    |~~|    .    |~~|    .    |~~|    .
.    |~~|    .    |~~|    .    |~~|    .
........................................
.    |~~|    .    |~~|    .    |~~|    .
.    |~~|    .    |~~|    .    |~~|    .
.    |~~|    .    |~~|    .    |~~|    .
.    |~~|    .    |~~|    .    |~~|    .
.    |~~|    .    |~~|    .    |~~|    .
.    |~~|    .    |~~|    .    |~~|    .
.    |~~|    .    |~~|    .    |~~|    .
.    |~~|    .    |~~|    .    |~~|    .
.    |~~|    .    |~~|    .    |~~|    .
.    |~~|    .    |~~|    .    |~~|    .
........................................
```

### without border

```
------------            ------------
~~~~~~~~~~~~            ~~~~~~~~~~~~
~~~~~~~~~~~~            ~~~~~~~~~~~~
----+~~+----            ----+~~+----
    |~~|                    |~~|
    |~~|                    |~~|
    |~~|                    |~~|
    |~~|        |~~|        |~~|
    |~~|     +--+~~+--+  +--+~~+--+
    |~~|     |~~~~~~~~|  |~~~~~~~~|
----+~~+-----+~~~~~~~~+--+~~~~~~~~+-
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
----+~~+-----+~~~~~~~~+--+~~~~~~~~+-
    |~~|     |~~~~~~~~|  |~~~~~~~~|
    |~~|     +--+~~+--+  +--+~~+--+
    |~~|        |~~|        |~~|
    |~~|        |~~|        |~~|
 +--+~~+--+     |~~|        |~~|
 |~~~~~~~~|     |~~|        |~~|
-+~~~~~~~~+-----+~~+--------+~~+----
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-+~~~~~~~~+-----+~~+--------+~~+----
 |~~~~~~~~|     |~~|        |~~|
 +--+~~+--+     |~~|        |~~|
    |~~|        |~~|        |~~|
```
