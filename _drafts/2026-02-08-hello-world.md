---
title: "Hello World: My First Blog Post"
date: 2026-02-08 12:00:00 +0900
categories: [Blog, Introduction]
tags: [hello-world, getting-started]
---

## Welcome

This is my first blog post! I built this blog using **Jekyll** with the **Chirpy** theme. Let me demonstrate some of the features this blog supports.

## Code Snippets

### Python

```python
def fibonacci(n: int) -> list[int]:
    """Generate the first n Fibonacci numbers."""
    if n <= 0:
        return []
    fib = [0, 1]
    for _ in range(2, n):
        fib.append(fib[-1] + fib[-2])
    return fib[:n]

print(fibonacci(10))
# Output: [0, 1, 1, 2, 3, 5, 8, 13, 21, 34]
```

### JavaScript

```javascript
const debounce = (fn, delay) => {
  let timer;
  return (...args) => {
    clearTimeout(timer);
    timer = setTimeout(() => fn(...args), delay);
  };
};

// Usage
const handleSearch = debounce((query) => {
  console.log(`Searching for: ${query}`);
}, 300);
```

### Bash

```bash
#!/bin/bash
# Deploy script
echo "Building site..."
bundle exec jekyll build
echo "Deploy complete!"
```

### Inline Code

You can also use inline code like `console.log("hello")` or reference file paths like `/etc/nginx/nginx.conf`{: .filepath }.

## Images

Here's how you can include images in posts:

```markdown
![Description](/assets/img/sample.png){: width="700" height="400" }
_Image caption here_
```

## YouTube Embed

You can embed YouTube videos using the built-in include:

{% include embed/youtube.html id='dQw4w9WgXcQ' %}

## Prompt Callouts

Chirpy supports styled prompt blocks:

> This is a **tip** — useful advice for the reader.
{: .prompt-tip }

> This is an **info** block — additional context or background.
{: .prompt-info }

> This is a **warning** — something to be careful about.
{: .prompt-warning }

> This is a **danger** block — critical information about potential issues.
{: .prompt-danger }

## What's Next

I'll be sharing posts about software engineering, programming tips, and things I learn along the way. Stay tuned!
