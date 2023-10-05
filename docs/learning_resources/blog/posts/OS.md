---
authors: [AkashSingh3031]
categories:
  - Core Subjects
comments: true
date:
  created: 2023-01-05
  # updated: 2023-10-05
tags:
  - Core Subject
  - OS
title: Operating System
---

??? question "1. What is the main purpose of an operating system? Discuss different types?"
    !!! abstract "What is the main purpose of an operating system?"
        An operating system (OS) is system software that manages computer hardware, software resources, and provides common services for computer programs. So it manages the computer’s memory, processes, devices, files, and security aspects of the system. It also allows us to communicate with the computer without knowing how to speak the computer’s language. Without an operating system, a computer is not useful.

    !!! tip "Types of operating system:"
        ???+ info "Batch OS"
            Batch OS
        ???+ info "Distributed OS"
            Distributed OS
        ???+ info "Multitasking OS"
            Multitasking OS
        ???+ info "Network OS"
            Network OS
        ???+ info "Real-Time OS"
            Real-Time OS
        ???+ info "Mobile OS"
            Mobile OS

<!-- more -->

??? question "2. What is a socket, kernel and monolithic kernel ?"
    !!! abstract "Socket"
        A socket is defined as an endpoint for communication, A pair of processes communicating over a network employ a pair of sockets ,one for each process. A socket is identified by an IP address concatenated with a port number. 
        The server waits for incoming client requests by listening to a specified port. Once a request is received, the server accepts a connection from the client socket to complete the connection.
    !!! abstract "Kernel"
            Kernel is the central core component of an operating system that manages operations of computer and hardware. Kernel Establishes communication between user level application and hardware. Manages memory and CPU time. Decides state of incoming processes. Controls Disk, Memory, Task Management
    !!! abstract "Monolithic Kernel"
        It is one of the types of kernel where all operating system services operate in kernel space. It has dependencies between system components. It has huge lines of code which is complex.
        !!! success "Example"
            Unix, Linux, Open VMS, XTS-400 etc.

??? question "3. Difference between process and program and thread? Different types of process."
    !!! abstract "Process"
        Process is an instance of an executing program. For example, we write our computer programs in a text file and when we execute this program, it becomes a process which performs all the tasks mentioned in the program.

    !!! abstract "Program"
        Program is a set of instructions to perform a certain task. Eg: chrome.exe, notepad.exe

    !!! abstract "Thread"
        Thread is a path of execution within a process. A thread is also known as a lightweight process. The idea is to achieve parallelism by dividing a process into multiple threads. For example,Word processor uses multiple threads: one thread to format the text, another thread to process inputs.

??? question "4. Define virtual memory, thrashing, threads."
    !!! abstract "Virtual Memory"
        A computer can address more memory than the amount physically installed on the system. This extra memory is actually called virtual memory and it is a section of a hard disk that’s set up to emulate the computer’s RAM.
        The main visible advantage of this scheme is that programs can be larger than physical memory. Virtual memory serves two purposes. First, it allows us to extend the use of physical memory by using a disk. Second, it allows us to have memory protection, because each virtual address is translated to a physical address.

    !!! abstract "Thrashing"
        Thrashing is a condition or a situation when the system is spending a major portion of its time in servicing the page faults, but the actual processing done is very negligible. High degree of multiprogramming(if number of processes keeps on increasing in the memory), lack of frames (if a process is allocated too few frames, then there will be too many and too frequent page faults) causes Thrashing.

    !!! abstract "Threads"
        A thread is a single sequential flow of execution of tasks of a process so it is also known as thread of execution or thread of control.

??? question "5. What is RAID ? Different types."
    !!! abstract "RAID"
        RAID, or “Redundant Arrays of Independent Disks” is a technique which makes use of a combination of multiple disks instead of using a single disk for increased performance, data redundancy or both.Data redundancy, although taking up extra space, adds to disk reliability. This means, in case of disk failure, if the same data is also backed up onto another disk, we can retrieve the data and go on with the operation.

??? question "6. What is a deadlock? Different conditions to achieve a deadlock."
    !!! abstract "What is a deadlock"
        A Deadlock is a situation where each of the computer processes waits for a resource which is being assigned to some other process. In this situation, none of the processes gets executed since the resource it needs is held by some other process which is also waiting for some other resource to be released.

    !!! abstract "How deadlock is achieved" 
        Deadlock happens when Mutual exclusion, hold and wait, No preemption and circular wait occurs simultaneously.

    !!! tip "Necessary Conditions for deadlock"
        ???+ info "Mutual Exclusion"
            Mutual Exclusion
        ???+ info "Hold and Wait"
            Hold and Wait
        ???+ info "No preemption"
            No preemption
        ???+ info "Circular Wait"
            Circular Wait
        
??? question "7. What is fragmentation? Types of fragmentation."
    !!! abstract "Fragmentation"
        An unwanted problem in the operating system in which the processes are loaded and unloaded from memory, and free memory space is fragmented. Processes can’t be assigned to memory blocks due to their small size, and the memory blocks stay unused. It is also necessary to understand that as programs are loaded and deleted from memory, they generate free space or a hole in the memory. These small blocks cannot be allotted to new arriving processes, resulting in inefficient memory use.

        The conditions of fragmentation depend on the memory allocation system. As the process is loaded and unloaded from memory, these areas are fragmented into small pieces of memory that cannot be allocated to incoming processes. It is called fragmentation.

    !!! tip "Types of fragmentation"
        ???+ info "Internal"
            Internal
        ???+ info "External"
            External

??? question "8. What is spooling ?"
    !!! abstract "Spooling"
        SPOOL is an acronym for simultaneous peripheral operations online. Spooling is a process in which data is temporarily held to be used and executed by a device, program, or system.

        In spooling, there is no interaction between the I/O devices and the CPU. That means there is no need for the CPU to wait for the I/O operations to take place. Such operations take a long time to finish executing, so the CPU will not wait for them to finish.
        
        The biggest example of Spooling is printing. The documents which are to be printed are stored in the SPOOL and then added to the queue for printing. During this time, many processes can perform their operations and use the CPU without waiting while the printer executes the printing process on the documents one-by-one.

??? question "9. What is semaphore and mutex (Differences might be asked)? Define Binary semaphore."
    !!! abstract "Semaphore"
        Semaphore is simply a variable that is non-negative and shared between threads. A semaphore is a signaling mechanism, and a thread that is waiting on a semaphore can be signaled by another thread. 

        ???+ note "It uses two atomic operations"
            !!! info ""
                1) wait, 
            !!! info ""
                2) signal 
            for the process synchronization.
        A semaphore either allows or disallows access to the resource, which depends on how it is set up.

    !!! abstract "Mutex"
        The full form of Mutex is Mutual Exclusion Object. It is a special type of binary semaphore which used for controlling access to the shared resource. It includes a priority inheritance mechanism to avoid extended priority inversion problems. It allows current higher priority tasks to be kept in the blocked state for the shortest time possible. However, priority inheritance does not correct priority- inversion but only minimizes its effect.

??? question "10. Belady’s Anomaly"
    !!! abstract "Belady’s Anomals"
        Belady’s anomaly is the name given to the phenomenon where increasing the number of page frames results in an increase in the number of page faults for a given memory access pattern.

    !!! note "Solution to fix Belady’s Anomaly"
        Implementing alternative page replacement algo helps eliminate Belady’s Anomaly.. Use of stack based algorithms, such as Optimal Page Replacement Algorithm and Least Recently Used (LRU) algorithm, can eliminate the issue of increased page faults as these algorithms assign priority to pages

??? question "11. Starving and Aging in OS"
    !!! abstract "Starving/Starvation(also called Lived lock)"
        Starvation is the problem that occurs when low priority processes get jammed for an unspecified time as the high priority processes keep executing. So starvation happens if a method is indefinitely delayed.

    !!! note "Solution to Starvation" 
        Ageing is a technique of gradually increasing the priority of processes that wait in the system for a long time.

??? question "12. Why does trashing occur?"
    !!! abstract ""
        High degree of multiprogramming(if number of processes keeps on increasing in the memory) , lack of frames(if a process is allocated too few frames, then there will be too many and too frequent page faults.) causes Thrashing.

??? question "13. What is paging and why do we need it?"
    !!! abstract "Paging"
        Paging is a memory management scheme that eliminates the need for contiguous allocation of physical memory. This scheme permits the physical address space of a process to be non – contiguous.
    
    !!! abstract "Why do we need it"
        Paging is used for faster access to data. When a program needs a page, it is available in the main memory(RAM) as the OS copies a certain number of pages from your storage device to main memory. Paging allows the physical address space of a process to be noncontiguous.

??? question "14. Demand Paging, Segmentation"
    !!! abstract "Demand Paging"
        Demand paging is a method of virtual memory management which is based on the principle that pages should only be brought into memory if the executing process demands them. This is often referred to as lazy evaluation as only those pages demanded by the process are swapped from secondary storage to main memory.
        
        So demand paging works opposite to the principle of loading all pages immediately.

    !!! abstract "Segmentation"
        Segmentation is a memory management technique in which the memory is divided into the variable size parts. Each part is known as a segment which can be allocated to a process.

        The details about each segment are stored in a table called a segment table. Segment table is stored in one (or many) of the segments.

    !!! tip "Segment table contains mainly two information about segment"
        ???+ note "Base"
            It is the base address of the segment
        ???+ note "Limit"
            It is the length of the segment.

??? question "15. Real Time Operating System, types of RTOS."
    !!! abstract "RTOS"
        A real-time operating system (RTOS) is a special-purpose operating system used in computers that has strict time constraints for any job to be performed and is intended to serve real time applications that possess data as it comes in , typically without buffer delays.

    !!! tip "Types of RTOS"
        ???+ note "Hard RTOS"
            Hard RTOS
        ???+ note "Firm RTOS"
            Firm RTOS
        ???+ note "Soft RTOS"
            Soft RTOS

??? question "16. Difference between main memory and secondary memory."
    !!! abstract "Primary / Main memory" 
        Primary memory is the computer memory that is directly accessible by CPU. It is comprised of DRAM and provides the actual working space to the processor. It holds the data and instructions that the processor is currently working on. 
    
    !!! abstract "Secondary Memory / Mass Storage"
        The contents of the secondary memory first get transferred to the primary memory and then are accessed by the processor, this is because the processor does not directly interact with the secondary memory

??? question "17. Static Binding, Dynamic Binding"
    Static binding happens when the code is compiled, while dynamic bind happens when the code is executed at run time.

    !!! abstract "Static Binding"
        When a compiler acknowledges all the information required to call a function or all the values of the variables during compile time, it is called “static binding”. As all the required information is known before runtime, it increases the program efficiency and it also enhances the speed of execution of a program. Static Binding makes a program very efficient, but it declines the program flexibility, as ‘values of variable’ and ‘function calling’ are predefined in the program. Static binding is implemented in a program at the time of coding. Overloading a function or an operator is the example of compile time polymorphism i.e. static binding.

    !!! abstract "Dynamic Binding"
        Dynamic Binding Calling a function or assigning a value to a variable, at run-time is called “Dynamic Binding”. Dynamic binding can be associated with run time ‘polymorphism’ and ‘inheritance’ in OOP. Dynamic binding makes the execution of a program flexible as it can decide what value should be assigned to the variable and which function should be called, at the time of program execution. But as this information is provided at run time it makes the execution slower as compared to static binding.

??? question "18. FCFS Scheduling"
    !!! abstract "First Come First Serve (FCFS) Scheduling"
        First Come First Serve (FCFS) is an operating system scheduling algorithm that automatically executes queued requests and processes in order of their arrival. It is the easiest and simplest CPU scheduling algorithm. In this type of algorithm, processes which requests the CPU first get the CPU allocation first. This is managed with a FIFO queue. The full form of FCFS is First Come First Serve.

        As the process enters the ready queue, its PCB (Process Control Block) is linked with the tail of the queue and, when the CPU becomes free, it should be assigned to the process at the beginning of the queue.

??? question "19. SJF Scheduling"
    !!! abstract "Shortest Job First (SJF) Scheduling"
        Shortest Job First (SJF) is an algorithm in which the process having the smallest execution time is chosen for the next execution. This scheduling method can be preemptive or non-preemptive. It significantly reduces the average waiting time for other processes awaiting execution. The full form of SJF is Shortest Job First.

    ???+ tip "There are basically two types of SJF methods"
        !!! note "Non-Preemptive SJF"
            Non-Preemptive SJF
        !!! note "Preemptive SJF"
            Preemptive SJF

??? question "20. SRTF Scheduling"
    !!! abstract "SRTF Scheduling" 
        SRTF Scheduling is a preemptive version of SJF scheduling. In SRTF, the execution of the process can be stopped after a certain amount of time. At the arrival of every process, the short term scheduler schedules the process with the least remaining burst time among the list of available processes and the running process.

??? question "21. LRTF Scheduling"
    !!! abstract "LRTF Scheduling"
        This is a preemptive version of Longest Job First (LJF) scheduling algorithm. In this scheduling algorithm, we find the process with the maximum remaining time and then process it. We check for the maximum remaining time after some interval of time(say 1 unit each) to check if another process having more Burst Time arrived up to that time.

??? question "22. Priority Scheduling"
    !!! abstract "Priority Scheduling"
        Priority Scheduling is a method of scheduling processes that is based on priority. In this algorithm, the scheduler selects the tasks to work as per the priority.
        
        The processes with higher priority should be carried out first, whereas jobs with equal priorities are carried out on a round-robin or FCFS basis. Priority depends upon memory requirements, time requirements, etc.

??? question "23. Round Robin Scheduling"
    !!! abstract "Round Robin Scheduling"
        In Round-robin scheduling, each ready task runs turn by turn only in a cyclic queue for a limited time slice. This algorithm also offers starvation free execution of processes. Widely used preemptive scheduling method in traditional OS. All the jobs get a fair allocation of CPU. Cons include : Finding a correct time quantum is a quite difficult task in this system, Round-robin scheduling doesn’t give special priority to more important tasks.

??? question "24. Producer Consumer Problem"
    !!! abstract "About Producer-Consumer problem"
        The Producer-Consumer problem is a classic problem that is used for multi-process synchronisation i.e. synchronisation between more than one processes.

        The job of the Producer is to generate the data, put it into the buffer, and again start generating data. While the job of the Consumer is to consume the data from the buffer.

    !!! note "What’s the problem here?"
        ???+ quote "The following are the problems that might occur in the Producer-Consumer"
            !!! success ""
                The producer should produce data only when the buffer is not full. If the buffer is full, then the producer shouldn’t be allowed to put any data into the buffer.

            !!! success ""
                The consumer should consume data only when the buffer is not empty. If the buffer is empty, then the consumer shouldn’t be allowed to take any data from the buffer.

            !!! success ""
                The producer and consumer should not access the buffer at the same time.

        We can solve this problem by using semaphores.

??? question "25. Banker’s Algorithm"
    !!! abstract "Banker’s Algorithm"
        It is a banker algorithm used to avoid deadlock and allocate resources safely to each process in the computer system. The ‘S-State’ examines all possible tests or activities before deciding whether the allocation should be allowed to each process. It also helps the operating system to successfully share the resources between all the processes. The banker’s algorithm is named because it checks whether a person should be sanctioned a loan amount or not to help the bank system safely simulate allocation resources.

??? question "26. Explain Cache"
    !!! abstract "Cache"
        Cache memory is an extremely fast memory type that acts as a buffer between RAM and the CPU. It holds frequently requested data and instructions so that they are immediately available to the CPU when needed.

??? question "27. Difference between direct mapping, associative mapping and set-associative mapping"
    !!! abstract "Direct Mapping"
        In direct mapping cache, instead of storing total address information with data in cache only part of address bits is stored along with data.
        The new data has to be stored only in a specified cache location as per the mapping rule for direct mapping. So it doesn't need replacement algorithm.

    !!! abstract "Associative Mapping"
        In associative mapping both the address and data of the memory word are stored.
        The associative mapping method used by cache memory is very flexible one as well as very fast.
        This mapping method is also known as fully associative cache.

    !!! abstract "Set-Associative Mapping"
        In Set-Associative cache memory two or more words can be stored under the same index address. 
        Here every data word is stored along with its tag. The number of tag-data words under an index is said to form a text.

??? question "28. Difference between multitasking and multiprocessing"
    !!! abstract "Multi-tasking"
        Multi-tasking is the logical extension of multiprogramming. In this system, the CPU executes multiple jobs by switching among them typically using a small time quantum, and these switches occur so frequently that the users can interact with each program while it is running. Multitasking is further classified into two categories: Single User & Multiuser. 

    !!! abstract "Multiprocessing"
        Multiprocessing is a system that has two or more than two processors. In this, CPUs are added for increasing computing speed of the system. Because of Multiprocessing, there are many processes that are executed simultaneously. Multiprocessing is further classified into two categories: Symmetric Multiprocessing and Asymmetric Multiprocessing. 