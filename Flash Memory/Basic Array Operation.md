---
tags:
  - ECE_564
  - Lecture_13
---
**How to update / erase a page** ([[NAND Array Structure]])
1) Copy valid page data
2) Block erase 
![[Basic Array Operation.png]]

*System level issues for page update*:
- Write only works on erased page
- [[In-place update]] of a page is not available 
- Erase operation cannot be don on a single page




**Read Operation**: Array biasing scheme
- Read 1 page at a time ([[NAND Array Structure]])
- Cell 