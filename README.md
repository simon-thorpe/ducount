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

### Example Usage
The below example runs ducount on a directory called reports. The results are a list of subdirectories showing how many KB each one sums to, the total file count of each one, and the age of the youngest file. The totals of the reports directory itself are shown as the last row.
```
$ ducount reports/
152.35 KB   14        500 days old   d reports/archived
299.55 KB   72        28 days old    d reports/last_month
404.06 KB   45        5 days old     d reports/last_week
434.2 KB    132       2 days old     d reports/this_week
580.39 KB   36        1 days old     d reports/yesterday
817.41 KB   21        0 days old     d reports/today
12.11 MB    811       0 days old     d reports/current
14.74 MB    1138      .
```

### Install
Paste the following line into a terminal to install:
```
sudo wget -O/usr/bin/ducount https://raw.githubusercontent.com/simon-thorpe/ducount/master/ducount && sudo chmod +x /usr/bin/ducount
```

### Run
Then run in your directory of choice:
```
$ ducount
```
