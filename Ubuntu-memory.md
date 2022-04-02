# Ubuntu memory

## Size of a Directory

```
sudo -sh /var
```

- s - Display only the total size of the specified directory, do not display file size totals for subdirectories

- h - Print sizes in a human-readable format (h).

**Output**

> 85G /var

### Size of first level dirs, sorted

```
sudo du -h -d1 /home/user/Documents/Apps/ | sort -rh
```

## RAM Usage

```
free -m
```
