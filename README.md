# Round-Robin-Simulator-in-C++
This C++ program simulates Round Robin (RR) scheduling, a CPU scheduling algorithm that assigns a fixed time quantum to each process. Here's the breakdown:

Key Functions:

findWaitingTime():

Calculates the waiting time for each process by iterating through the processes in a round-robin fashion until all are completed.

findTurnAroundTime():

Calculates turnaround time as Turnaround Time = Waiting Time + Burst Time.

findavgTime():

Calls the above functions and calculates the average waiting time and average turnaround time.

Logic Overview:

A copy of burst times (rem_bt[]) is created to track remaining execution time for each process.

The algorithm iterates in cycles, reducing each process's remaining burst time by the quantum value until all processes are completed.

Final waiting and turnaround times are displayed.

Sample Output (For 3 processes with burst times [10, 5, 8] and quantum = 2):
