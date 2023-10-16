> This is still subject to change due to not having the physical and actual definition of these based on the book that the prof is using.

> #inProgress 


## Process States
The state of a process is defined in part by the current activity of that process. A process may be in one of the following states:
- **New**. The process is being created.
- **Running**. Instructions are being executed.
- **Waiting**. The process is waiting for some event to occur (such as an I/O completion or reception of a signal).
- **Ready**. The process is waiting to be assigned to a processor.
- **Terminated**. The process has finished execution.

![[Pasted image 20231005203532.png]]

There are three types of process states
### Two states process
The first step in designing an OS to control processes is to describe the behavior that we would like the processes to exhibit. We can construct the simplest possible model by observing that, at any time, a process is either being executed by a processor, or it isn’t. In this model, a process may be in one of the two states: **Running** or **Not Running**

**Not Running** - process control block for the process and enters that process into the system. This is the state they will go. (also called "*Ready*" state)
**Running** -  From time to time, the currently running process will be interrupted, and the dispatcher portion of the OS will select some other process to run.
![[Pasted image 20231005214103.png]]

### Three state process
In the second case, it is a technicality of the system (not enough CPUs to
give each process its own private processor). 
In Fig. 2-2 we see a state diagram showing the three states a process may be in:
1. Running (actually using the CPU at that instant).
2. Ready (runnable; temporarily stopped to let another process run).
3. Blocked (unable to run until some external event happens).

Logically, the first two states are similar. In both cases the process is willing to run,
only in the second one, there is temporarily no CPU available for it. The third state is fundamentally different from the first two in that the process cannot run, even if
the CPU is idle and has nothing else to do.

![[Pasted image 20231005213501.png]]

### Five state process
The queue is a first-in-first-out list and the processor operates in round-robin fashion on the available processes (each process in the queue is given a certain amount of time, in turn, to execute and then returned to the queue, unless blocked). 

Some processes in the Not Running state are ready to execute, while others are blocked, waiting for an I/O operation to complete. Thus, using a single queue, the dispatcher could not just select the process at the oldest end of the queue. Rather, the dispatcher would have to scan the list looking for the process that is not blocked and that has been in the queue the longest.

A more natural way to handle this situation is to split the Not Running state
into two states: Ready and Blocked. As a good measure, we have added two additional states that will prove useful. The five states in this new diagram are as follows:

1. **Running**: The process that is currently being executed. For this chapter, we will assume a computer with a single processor, so at most, one process at a time can be in this state.
2. **Ready**: A process that is prepared to execute when given the opportunity.
3. **Blocked/Waiting**: A process that cannot execute until some event occurs, such as the completion of an I/O operation.
4. **New**: A process that has just been created but has not yet been admitted to the pool of executable processes by the OS. Typically, a new process has not yet been loaded into main memory, although its process control block has been created.
5. **Exit**: A process that has been released from the pool of executable processes by the OS, either because it halted or because it aborted for some reason.

![[Pasted image 20231005214751.png]]
The New and Exit states are useful constructs for process management. The
New state corresponds to a process that has just been defined. For example, if a new
user attempts to log on to a time-sharing system, or a new batch job is submitted for
execution, the OS can define a new process in two stages. 

## Process Creation & Termination
### Process Creation
Operating systems need some way to create processes. In general-purpose systems, however, some way is needed to create and terminate processes as needed during opera-
tion. There are four principles causes the process to be created:

1. System Boot-up
	-  typically numerous processes are created. Some of these processes are foreground processes, that is, processes that interact with (human) users and perform work for them. Others run in the background and are not associated with particular users, but instead have some specific function.
	- Processes that stay in the background to handle some activity such as email, Web pages, news, printing, and so on are called **daemons**. 
2. Batch System Initiation
	- When the operating system decides it has the resources to run another job, it creates a new process and runs the next job from the input queue in it.
3. Human User 
	   - interactive systems, users can start a program by typing a command or (double) clicking on an icon. Taking either of these actions starts a new process and runs the selected program in it.  
4. Process Spawning
	 - Often a running process will issue system calls to create one or more new processes to help it do its job. Creating new processes is particularly useful when the work to be done can easily be formulated in terms of several related, but otherwise independent interacting processes. 


### Process Termination
Any computer system must provide a means for a process to indicate its completion. A batch job should include a Halt instruction or an explicit OS service call for termination. In the former case, the Halt instruction will generate an interrupt to alert the OS that a process has completed. 

1. **Normal Completion** - The process executes an OS service call to indicate that it has completed running.
2. **Time Limit Execution** - The process has run longer than the specified total time limit. There are a number of possibilities for the type of time that is measured. These include total elapsed time (“wall clock time”), amount of time spent executing, and, in the case of an interactive process, the amount of time since the user last provided any input.
3. **Memory unavailable** - The process requires more memory than the system can provide.
4. **Bounds Violation** - The process tries to access a memory location that it is not allowed to access.
5. **Protection Error** - The process attempts to use a resource such as a file that it is not allowed to use, or it tries to use it in an improper fashion, such as writing to a read-only file.
6. **Arithmetic Error** - The process tries a prohibited computation (such as division by zero) or tries to store numbers larger than the hardware can accommodate.
7. **Time Overrun** - The process has waited longer than a specified maximum for a certain event to occur.
8. **I/O Failure** - An error occurs during input or output, such as inability to find a file, failure to read or write after a specified maximum number of tries (when, for example, a defective area is encountered on a tape), or invalid operation (such as reading from the line printer).
9. **Invalid Instruction** - The process attempts to execute a nonexistent instruction (often a result of branching into a data area and attempting to execute the data).
10. **Privilege Instruction** - The process attempts to use an instruction reserved for the operating system.
11. **Data Misuse** - A piece of data is of the wrong type or is not initialized.
12. **Operator/ OS Intervention** - For some reason, the operator or the operating system has terminated the process (e.g., if a deadlock exists).
13. **Parent Termination** - When a parent terminates, the operating system may automatically terminate all of the offspring of that parent.
14. **Parent Request** - A parent process typically has the authority to terminate any of its offspring.

### Process Scheduler
The aim of processor scheduling is to assign processes to be executed by the processor or processors over time, in a way that meets system objectives, such as response time, throughput, and processor efficiency. In many systems, this scheduling activity is broken down into three separate functions: long-, medium-, and short-term scheduling.

1. **Long Term Scheduler** - The decision to add to the pool of processes to be executed.
2. **Short Term Scheduler** - The decision as to which available process will be executed by the processor.
3. **Medium Scheduler** - The decision to add to the number of processes that are partially or fully in main memory.
![[Pasted image 20231005220138.png]]



## Preemptive and Non-preemptive process

CPU-scheduling decisions may take place under the following four circum stances:
1. When a process switches from the running state to the waiting state (for example, as the result of an I/O request or an invocation of wait() for the termination of a child process)
2. When a process switches from the running state to the ready state (for example, when an interrupt occurs)
3. When a process switches from the waiting state to the ready state (for example, at completion of I/O)
4. When a process terminates

### Preemptive Process

- Result in race conditions when data are shared among several processes. Consider the case of two processes that share data. While one process is updating the data, it is preempted so that the second process can run. The second process then tries to read the data, which are in an inconsistent state.
- preemptive kernel requires mechanisms such as mutex locks to prevent race conditions when accessing shared kernel data structures. Most modern operating systems are now fully preemptive when running in kernel mode.
### Non-preemptive Process
- once the CPU has been allocated to a process, the process keeps the CPU until it releases it either by terminating or by switching to the waiting state. Virtually all modern operating systems including Windows, macOS, Linux, and UNIX use preemptive scheduling algorithms.
- nonpreemptive kernel will wait for a system call to complete or for a process to block while waiting for I/O to complete to take place before doing a context switch. This scheme ensures that the kernel structure is simple, since the kernel will not preempt a process while the kernel data structures are in an inconsistent state. Unfortunately, this kernel-execution model is a poor one for supporting real-time computing
