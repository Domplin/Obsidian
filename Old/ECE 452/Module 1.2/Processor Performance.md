- How can we quantify performance of a processing chip?
	- there must be some associated workload to assess performance 
		- *workload:* set of tasks someone (you) cares about


- **Benchmark:** standard workloads
	- Used to compare performance across machines
	- Either are or highly representative of actual programs people run
	- *Example:* H.264/MPEG decoding, gcc compiler, etc.

- **Micro-benchmarks:** non-standard non-workloads
	- Tiny programs used to isolate certain aspects of performance
	- Not representative of complex behaviors of real applications
	- *Examples:* binary tree search, towers-of-hanoi, 8-queens, etc.