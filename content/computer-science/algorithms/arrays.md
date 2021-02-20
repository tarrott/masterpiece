---
title: "Arrays"
date: 2021-01-31T08:56:42-05:00
draft: false
weight: 2
---


## Time/Space Complexity

- O(1) Access - Read/Write
- O(n) Insert
    - at start - O(n) due to shifting all other elements
    - at end - O(1)
    - at ith position - O(n)
- O(n) Deletion
- O(n) Add (when it doubles max size)

## Memory Requirements
- Reserved memory can cause excess unused memory
- Memory may not be available for a long continuous block


## Ease of Use
- straightforward