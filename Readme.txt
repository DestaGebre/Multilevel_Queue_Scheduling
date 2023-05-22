A common division is made between foreground(or interactive) 
processes and background (or batch) processes. These two types of processes have different
 response-time requirements, and so might have different scheduling needs. In addition, foreground processes may have priority over background processes.

A multi-level queue scheduling algorithm partitions the ready queue into several 
separate queues. The processes are permanently assigned to one queue, generally based on
 some property of the process, such as memory size, process priority, or process type. Each queue has its own scheduling algorithm.

For example, separate queues might be used for foreground and background processes.
 The foreground queue might be scheduled by the Round Robin algorithm, while the background queue is scheduled by an FCFS algorithm.

In addition, there must be scheduling among the queues, which is commonly implemented as 
fixed-priority preemptive scheduling. For example, The foreground queue may have absolute priority over the background queue.

Let us consider an example of a multilevel queue-scheduling algorithm with five queues:

System Processes

Interactive Processes

Interactive Editing Processes

Batch Processes

Student Processes

Each queue has absolute priority over lower-priority queues.
 No process in the batch queue, for example, could run unless the queues for system processes, 
interactive processes, and interactive editing processes were all empty. If an interactive editing process 
entered the ready queue while a batch process was running, the batch process will be preempted.



In this case, if there are no processes on the higher priority queue only then the processes on
 the low priority queues will run. For Example: Once processes on the system queue, the Interactive queue,
 and Interactive editing queue become empty, only then the processes on the batch queue will run.

The Description of the processes in the above diagram is as follows:

System Process The Operating system itself has its own process to run and is termed as System Process.

Interactive Process The Interactive Process is a process in which there should be the same kind of interaction (basically an online game ).

Batch Processes Batch processing is basically a technique in the Operating system that collects the programs and data
 together in the form of the batch before the processing starts.

Student Process The system process always gets the highest priority while the student processes always get the lowest priority.

In an operating system, there are many processes, in order to obtain the result we cannot put

 all processes in a queue; thus this process is solved by Multilevel queue scheduling.