# Question 4

## Q4: Extract Color Names from HTML

### Problem
Write a Bash script that extracts color names and hex values from `index.html` and prints them in the format:
color-name:#hexvalue

### Input Example
```html
<span class="color-name">"aliceblue"</span>: <span class="color-code">"#f0f8ff"</span>
<span class="color-name">"aqua"</span>: <span class="color-code">"#00ffff"</span>
```

### Expected Output
```
aliceblue:#f0f8ff
aqua:#00ffff
```

### Correct output for file index.html
The file is shared with your under /files in this Github repo!

```
aliceblue:#f0f8ff
antiquewhite:#faebd7
aqua:#00ffff
aquamarine:#7fffd4
azure:#f0ffff
beige:#f5f5dc
bisque:#ffe4c4
black:#000000
blue:#0000ff
blueviolet:#8a2be2
```

### Test Cases
1. Valid HTML → Extract correctly
2. Missing values → Skip invalid entries
3. Multiple entries per line → Handle correctly
