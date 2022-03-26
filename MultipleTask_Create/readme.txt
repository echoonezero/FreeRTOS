Here all 3 tasks have the same priority. Since printf takes too much time to execute, the messages "LED 1 running", "LED 2 running" and "LED 3 running" are not printed on terminal. 

Before the print executes, the time slice for one task ends and next task is scheduled. Check the file output1.

Hence add profiler and check the increment status to verify if all tasks are running. Comment the printf statements in the tasks as they take more time than the allocated time slice.

In the Debug mode, add the Led1/2/3Prof global variables to Live expressions tab to see the increments. All profiler variables are incrementing together proving that all the tasks are getting executed.

