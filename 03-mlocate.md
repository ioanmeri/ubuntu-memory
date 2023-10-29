# mlocate

mlocate is a **m**erging **locate** and database package. "Merging" means updatedb reuses the existing database to avoid re-reading most of the file system. This makes the database update faster and does not tax the system caches. mlocate can index several file systems including network file systems for network shares. This package is essential when attempting to quickly find documents in a terminal.

Edit the file /etc/updatedb.conf

Set up PRUNEPATHS with the directories you DO NOT want to search

PRUNEPATHS="/tmp /var/spool /media"
PRUNEPATHS: A whitespace-separated list of path names of directories which should not be scanned by updatedb. Each path name must be exactly in the form in which the directory would be reported by locate. By default, no paths are skipped.

Note that all of the above configuration information can also be changed or updated through the command line options to the utility updatedb.

---
