---
marp: true
title: Technical Documentation Presentation
author: 24f2002696@ds.study.iitm.ac.in
theme: gaia
paginate: true
---

<style>
section {
  background-color: #f5f5f5;
  color: #333;
}
h1 {
  color: #2c3e50;
  border-bottom: 3px solid #3498db;
}
h2 {
  color: #34495e;
}
code {
  background-color: #ecf0f1;
  padding: 2px 5px;
  border-radius: 3px;
}
</style>

# Technical Documentation
## Product API Guide

**Author:** 24f2002696@ds.study.iitm.ac.in
**Date:** November 2025

---

<!-- _backgroundColor: #2c3e50 -->
<!-- _color: white -->

## Overview

This documentation covers:
- API Architecture
- Performance Metrics
- Algorithm Complexity
- Best Practices

---

![bg](https://images.unsplash.com/photo-1451187580459-43490279c0fa?w=1200&q=80)

# System Architecture

Building scalable solutions

---

## Algorithm Complexity

The time complexity of our search algorithm:

$$
O(n \log n)
$$

Space complexity for the hash table:

$$
O(n)
$$

For binary search operations:

$$
T(n) = T(n/2) + O(1) = O(\log n)
$$

---

<!-- _footer: Technical Documentation © 2025 -->

## Performance Metrics

**Average Response Time:** $\mu = 45ms$

**Standard Deviation:** $\sigma = 12ms$

**99th Percentile:** $P_{99} = 120ms$

The efficiency gain follows:

$$
\text{Efficiency} = \frac{T_{\text{old}} - T_{\text{new}}}{T_{\text{old}}} \times 100\%
$$

---

## API Endpoints
```python
# GET request example
import requests

response = requests.get('https://api.example.com/data')
print(response.json())
```

**Complexity:** $O(1)$ lookup time

---

![bg left:40%](https://images.unsplash.com/photo-1517694712202-14dd9538aa97?w=800&q=80)

## Key Features

- Fast retrieval: $O(\log n)$
- Efficient storage: $O(n)$
- Scalable architecture
- Real-time processing

---

<!-- _backgroundColor: #ecf0f1 -->

## Big-O Notation Summary

| Operation | Time Complexity | Space Complexity |
|-----------|----------------|------------------|
| Search    | $O(\log n)$    | $O(1)$          |
| Insert    | $O(\log n)$    | $O(1)$          |
| Delete    | $O(\log n)$    | $O(1)$          |
| Sort      | $O(n \log n)$  | $O(n)$          |

---

## Asymptotic Analysis

For large datasets where $n \to \infty$:

$$
\lim_{n \to \infty} \frac{n \log n}{n^2} = 0
$$

This proves our algorithm scales better than $O(n^2)$ solutions.

---

![bg fit](https://images.unsplash.com/photo-1504868584819-f8e8b4b6d7e3?w=1200&q=80)

---

<!-- _footer: Contact: 24f2002696@ds.study.iitm.ac.in -->

# Thank You

Questions?

**Repository:** github.com/24f2002696/marp-documentation
```

## Key Changes Made:

1. **Slide 3** - Changed from `backgroundImage:` directive to `![bg]()` syntax
2. **Slide 7** - Added `![bg left:40%]()` for a split background
3. **Slide 10** - Added `![bg fit]()` for a full background slide

The `![bg]()` syntax is the proper Marp way to add background images. The variations include:
- `![bg]()` - Full background
- `![bg fit]()` - Fit to slide
- `![bg left:40%]()` - Background on left side (40% width)

Now update your `slides.md` file on GitHub with this corrected content, and the raw URL should work correctly!

The raw URL format remains:
```
https://raw.githubusercontent.com/24f2002696/marp-documentation/main/slides.md
