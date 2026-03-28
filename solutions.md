# Bash Mini Coding Assignment – Solutions

## Q1: Total Size of Files in Current Directory
### Solution
```bash
total=0

for file in *; do
    if [[ -f "$file" ]]; then
        size=$(stat -c%s "$file")
        total=$((total + size))
    fi
done

echo "total size = $total"
```

## Q2: Filter Error Logs

### Solution

```bash
grep "error" access.log
```

```bash
grep -i "error" access.log
```

## Q3: Organize Files by Extension

### Solution

```bash
#!/bin/bash

for file in *; do
    [[ -d "$file" ]] && continue

    ext="${file##*.}"
    [[ "$file" == "$ext" ]] && continue

    if [[ ! -d "$ext" ]]; then
        mkdir "$ext"
    fi

    mv "$file" "$ext"/
done
```

## Q4: Extract Color Names from HTML

### Solution

```bash
tr '"' '\n' < index.html | while read -r token; do
    if [[ "$token" == \#?????? ]]; then
        code="$token"
        read -r name
        echo "$name:$code"
    fi
done
```
