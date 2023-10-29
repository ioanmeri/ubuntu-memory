# The du command

The du (disk usage) command measures the disk space occupied by files or directories.

## Size of a Directory

```
sudo du -sh /var
```

- s - Display only the total size of the specified directory, do not display file size totals for subdirectories

- h - Print sizes in a human-readable format (h).

**Output**

> 85G /var

## Display the disk usage of the first-level subdirectories

```
sudo du -shc /var/*
```

```
24K	/var/db
4.0K	/var/empty
4.0K	/var/games
77G	/var/lib
4.0K	/var/local
0	/var/lock
3.3G	/var/log
0	/var/mail
4.0K	/var/opt
0	/var/run
196K	/var/spool
28K	/var/tmp
85G	total
```

### Size of first level dirs, sorted

```
sudo du -h -d1 /home/user/Documents/Apps/ | sort -rh
```
