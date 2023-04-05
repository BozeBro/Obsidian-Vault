#shell-info
Virtual Addresses act like a physical addresses but are fake.
Advantages of VM
1. Isolation - Programs do not interfere with each other
2. Don't worry about underrlying architecture. e.g. location of addresses on the stack.
3. Resource efficient (we can share physical address space)
Address Space have different range of addrs available.
1. virtual $\left\{ 0,1,\dots N-1 \right\}, N = 2^{n}$
2. physical $\left\{ 0,1,\dots M - 1 \right\} M = 2^{m}$
map $V \to P \cup \emptyset$
$map(a) = a' \text{ or }\emptyset$ if addr is not in the map 
Not efficient method.
see [[Page Table.excalidraw]]
Page Hit - Addr in page table, valid bit is set
Page Fault - No valid entry in page table, OS is invoked
1. seg fault returned
2. page in data, restart instruction
Use [[Paging]] to store more things for RAM