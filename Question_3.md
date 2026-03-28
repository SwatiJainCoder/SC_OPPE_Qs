# Question 3

## Q3: Organize Files by Extension

### Problem
Write a Bash script that organizes files into subdirectories based on their file extensions.

### Input
```
file1.txt
file2.txt
image.png
script.sh
README
```

### Expected Output
```
txt/
file1.txt
file2.txt

png/
image.png

sh/
script.sh

./
README
```

<img width="418" height="591" alt="image" src="https://github.com/user-attachments/assets/b20a1a32-3b55-49fb-9fa8-dee8784dbfa4" />

# Test Cases
1. Files with extensions → Proper grouping
2. Files without extensions → Remain unchanged
3. Existing directories → Should not cause errors
4. The script should not be creating the directories by looking at the directory names (folder name) instead it should be able to identify it 
