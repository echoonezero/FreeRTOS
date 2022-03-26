Experiment 1: Set the priority of vLed3Control as 2 and the other two tasks as 1 (unchanged).
In FreeRTOS higher the priority number, greater the task priority. During debugging it is seen that only vLed3Control is executed as a low priority task cannot interrupt/preempt a high priority task. See output 1.

Experiment 2: Set priority of vLed1Control as 3 and repeat the process. Check output2.