TODO
====

List of things to get done.

General
-------

Backup lib archives which are not on github

libarchive
----------

freeShop wasn't working with those directives, is it now ?

SQLite
------

* Implement `sqlite3_os_init` and `sqlite3_os_end`, or replace
  `-DSQLITE_OS_OTHER=1` with `-DSQLITE_OS_UNIX=1`?
* Remove `--disable-threadsafe` and implement locking mechanism.
