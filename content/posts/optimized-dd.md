---
author: "Reperak"
date: "2021-07-04"
tags: ["miscellaneous", "unix"]
title: "Optimized dd Command For Drives"
---

### The Actual Command
```bash
dd if=INPUT of=OUTPUT bs=128k oflag=direct status=progress
```

### Explanation
The flags used in the custom command are optimized for speed and correctness. It bypasses the kernel cache and uses a large block size to get performance that usually outperforms dd's defaults.

`oflag=direct` makes dd use direct I/O, avoiding the cache entirely, ensuring that bytes are written immediately. This flag almost always hurts performance tremendously, however setting a large block size fixes this issue, and in many cases makes it even faster than with the cache.

From my research, a block size of 128kb (indicated by the `bs=128k` flag) is optimal for drives, but you can experiment on your own to find the setting that works best for you.

### Conclusion
Hopefully this blog post is useful to you. Happy imaging!
