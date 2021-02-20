---
title: "Linked Lists"
date: 2021-01-31T08:57:06-05:00
draft: false
weight: 5
---

## Time/Space Complexity

- O(n) Access - Read/Write
- O(n) Insert (However, no need for shifting following items like in an array)
    - at start - O(1)
    - at end - O(n) due to traversing the entire list to get to the last node
    - at ith position - O(n)
- O(n) Deletion (However, no need for shifting following items like in an array)
- O(n) Add

## Memory Requirements
- No use of reserved memory
- Extra memory is required for pointer variables
- Memory is more available for mulitple small continuous blocks (than a large ones from an arry) 


## Ease of Use
- more prone to errors (segmentation fault or memory leak)