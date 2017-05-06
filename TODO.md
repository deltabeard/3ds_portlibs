TODO
====

List of things to get done.

General
-------

Backup lib archives which are not on github

libarchive
----------

freeShop wasn't working with those directives, is it now ?

libxml2
-------

libxml2 wont compile, with reference undefined to gzdOpen (zlib is installed though)


SQLite
------

* Implement `sqlite3_os_init` and `sqlite3_os_end`, or replace
  `-DSQLITE_OS_OTHER=1` with `-DSQLITE_OS_UNIX=1`?
* Remove `--disable-threadsafe` and implement locking mechanism.
