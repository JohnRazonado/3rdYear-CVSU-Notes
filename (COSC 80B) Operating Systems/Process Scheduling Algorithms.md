- A process of scheduling that could be preemptive or non-preemptive

![[Pasted image 20231019134503.png]]
> The algorithms below will just utilize a preemptive process

These are the diagrams needed to answer the Turnaround Time and Waiting to of the given process jobs:
#### Timeline
- Sequence of job arrival time
- Arrival of each job

#### Gantt Chart
- Constructed to identify the sequence of jobs.

#### Table
Holds the information of the jobs

|Jobs | Arrival time| Burst Time| Turnaround Time (ET - AT = TT) | Waiting Time (TT - BT = WT)|
|---|---|---|---|---|
|A|0|4|4-0=4|4-4=0|
|B|0|2|6-0=6|6-2=4|
|C|2|7|13-2=11|11-7=4|
>This is the sample layout of the table

**Arrival Time** - Check whether who's first
**Burst Time** - How long OS will process the job
**Turnaround Time** - How long is the process
**Waiting Time** - How long it wait to start.

> #inProgress : This part needs to be updated to separate the two categories of the scheduling algorithms. The NPP and PEP.


## Non-Preemptive
### [[First Come First Serve (FCFS)]]
- Queue basis of jobs is on the arrival time 
- Since this is a non-preemptive algorithm, it is a one at a time basis
### [[Shortest Job First (SJF)]]
- Who came with shortest original burst will prioritize to run first
- Shortest burst = prioritize on queue

### [[Non-Preemptive Priority]]
- This looks at priority then on the arrival
- Then it will look at the burst time having the lowest original

## Preemptive
### [[Preemptive Priority]]

- Algorithm that will stop as a new jobs arrived and assess the priority 
- If priority is the same, check the **lowest original burst time**
- If they have same **lowest original burst time**, then look at **the first arrival time** and then the sequence of the jobs.

### [[Shortest Remaining Time First (SRTF)]]

- It is under the Preemptive Scheduling Algorithm
	- Which re-evaluate the arrival time
- Evaluates the remaining burst time
	- Unlike the preemptive priority which take a look at priority and the original burst time.

### [[Round Robin]]
- A preemptive scheduling that give each process jobs to process at **specific time**.
- **Quantum time** - the specific time given in each **tier**
- There's a new system in this one, the **Tier System**

## Others
These types of scheduling combines all the scheduling algorithms above.

## [[MultiLevel Queue (MLQ)]]
- According to the priority of process, processes are places in different queues. 
- Generally high priority processes are placed in the top level queue. Online after completion of processes from top level queue, lower level queued processes are scheduled.

## bruh