# ducount - disk usage count
Calculates disk usage for files in a given directory.

It mimics the functionality of the unix du command by recursively scanning files in
the target directory. It will additionally display file count and age information.

Usage: ducount [PATH]
Columns are printed in the following order:
- size
- count
- age of youngest file in dir (recursive)
- dir or file
- path

```
root@pc:/mozilla-release$ ducount modules/
152.35 KB   14        5 days old     d modules/libbz2
299.55 KB   72        5 days old     d modules/libmar
404.06 KB   45        5 days old     d modules/libpref
434.2 KB    132       5 days old     d modules/libjar
580.39 KB   36        5 days old     d modules/zlib
817.41 KB   21        5 days old     d modules/brotli
12.11 MB    811       2 days old     d modules/freetype2
14.74 MB    1138      .
```
