# Tiny Logtail

Tiny Logtail is a command-line program, simply printing log file lines that have not been read yet.

### Installation:
```
$ cd tiny-logtail
$ make
$ chmod +x tiny-logtail
```
### Usage:
```
$ tiny-logtail <log_file> <offset_file>
```
### Example:
```
$ cat > abc.txt
a
b
c
^D
$ tiny-logtail abc.txt
a
b
c
$ echo d >> abc.txt
$ tiny-logtail abc.txt
d
```
