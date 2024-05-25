# Linux-Kernal-Modules
Linux Kernel Module Design and Development Project with Basic Kernel Data Structures

```

+-----------------------------------------+
|       The Set of Kernel Modules         |
+-----------------------------------------+
                  |
                  v
+-----------------------------------------+
| Module 1 - /proc/jiffies                |
|-----------------------------------------|
| - Create /proc/jiffies file             |
| - Report current value of jiffies       |
| - Remove /proc/jiffies on module removal|
+-----------------------------------------+
                  |
                  v
+-----------------------------------------+
| Module 2 - /proc/seconds                |
|-----------------------------------------|
| - Create /proc/seconds file             |
| - Report elapsed seconds since load     |
|   using jiffies and HZ rate             |
| - Remove /proc/seconds on module removal|
+-----------------------------------------+
                  |
                  v
+-----------------------------------------+
| Module 3 - List Tasks using             |
|           for_each_process              |
|-----------------------------------------|
| - Iterate through all tasks             |
| - Output task command, state, pid       |
| - Compare kernel log buffer with ps -el |
| - Output to kernel log buffer (dmesg)   |
+-----------------------------------------+
                  |
                  v
+-----------------------------------------+
| Module 4 - DFS Tree of Tasks            |
|-----------------------------------------|
| - Begin from init_task                  |
| - Perform DFS iteration of all tasks    |
| - Output task name, state, pid          |
| - Output to kernel log buffer (dmesg)   |
| - Verify with ps -eLf                   |
+-----------------------------------------+
                  |
                  v
+-----------------------------------------+
| Module 5 - Linked List of Struct color  |
|-----------------------------------------|
| - Create linked list with 4 elements    |
| - Output contents to kernel log buffer  |
| - Delete elements and free memory on    |
|   module exit                           |
| - Verify with dmesg                     |
+-----------------------------------------+
                  |
                  v
+-----------------------------------------+
| Module 6 - Collatz Sequence             |
|-----------------------------------------|
| - Create module named collatz           |
| - Generate and store sequence in        |
|   kernel linked list                    |
| - Output sequence to kernel log buffer  |
| - Delete list and free memory on exit   |
| - Verify with dmesg                     |
+-----------------------------------------+

```
