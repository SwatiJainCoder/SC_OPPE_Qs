# Question 1

## Q1: Total Size of Files in Current Directory

### Problem
Write a Bash script that calculates the total size (in bytes) of all files in the current working directory.

### Input Example

```
-rw-r--r-- 1 user user 3 Oct 13 17:00 text.tex
-rw-r--r-- 1 user user 7 Oct 13 17:00 text.txt
-rw-r--r-- 1 user user 90 Oct 24 15:39 time
```

### Expected Output
```
total size = 100
```

### Test Cases
1. Files: 3, 7, 90 → Output: `total size = 100`
2. Empty directory → Output: `total size = 0`
3. Directory + files → Only file sizes counted
