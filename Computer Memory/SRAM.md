---
tags:
  - lecture_4
  - ECE_564
---

- **SRAM**: Static [[Random Access Memory]]
	- [[Static vs Dynamic Memory|Static]]: holds data as long as power is applied 
	- [[Volatility of Memory|Volatile]]: can not hold data if power is removed 
	- 3 operations states:
		- Hold
		- Write
		- Read

- Basic 6T (6 transistor) SRAM Cell: Bi-stable (Cross coupled) inverters for storage. 
	- Two access transistors
	- Word line (WL) controls access
		- WL = 0 (hold)
		- WL = 1 (read/write)