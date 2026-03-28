# Question 2

## Q2: Filter Error Logs

### Problem
Write a Bash script that reads an `access.log` file and prints only lines containing the word `ERROR`.

### Input (`access.log`) 
```
INFO Server started
ERROR Disk failure
WARNING Low memory
error Connection timeout
```

### Expected Output
```
ERROR Disk failure
error Connection timeout
```

### Expected Output for file (access.log)
The file `access.log` is available in the repo under files. You can copy paste from that file.

```
ERROR Disk failure detected on /dev/sda
error Connection timeout while reaching database
ERROR Failed to write to log file
error Failed to process uploaded file
````

### Test Cases
1. Mixed logs → Only lines containing "error"
2. No matching lines → No output
3. Case sensitivity should be preserved
