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
