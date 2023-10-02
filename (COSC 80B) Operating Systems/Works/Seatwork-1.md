Find the Following and check
## Evolution of OS
>https://www.eecs.harvard.edu/~cs161/videos/history.pdf
>https://www.cs.princeton.edu/courses/archive/fall21/cos318/lectures/1.Introduction.pdf

## Types of OS
>https://www.indeed.com/career-advice/career-development/types-of-operating-systems

## Storage Structure
The CPU can load instructions only from memory, so any programs to run must be stored there. 

### Main or Primary Memory
- usually too small to store all needed programs and data permanently.
-  volatile storage device that loses its contents when power is turned off or otherwise lost.

### Secondary Memory
- extension of main memory. The main requirement for secondary storage is that it be able to hold large quantities of data permanently.
- Most programs (system and application) are stored on a disk until they are loaded into memory. Many programs then use the disk as both the source and the destination of their processing.
### Components Of Component System
![[Pasted image 20230930204918.png]]

The higher levels are expensive, but they are fast. As we move down the hierarchy, the cost per bit generally decreases, whereas the access time generally increases. This trade-off is reasonable; if a given storage system were both faster and less expensive than another—other properties being the same —then there would be no reason to use the slower, more expensive memory. In fact, many early storage devices, including paper tape and core memories, are relegated to museums now that magnetic tape and semiconductor memory have become faster and cheaper. The top four levels of memory in Figure 1.4 may be constructed using semiconductor memory.

**Volatile storage** - loses its contents when the power to the device is removed
**Non-volatile Storage** - Data must be written here to save and keep permanently in the absence of power.
**Solid-state disks** -  In general, it's are faster than magnetic disks and are nonvolatile. One type of solid-state disk stores data in a large DRAM array during normal operation but also contains a hidden magnetic hard disk and a battery for backup power. 
**Magnetic Disk** - Most common secondary-storage device.
