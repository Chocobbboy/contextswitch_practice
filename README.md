# Context-Switching
A multithreaded simulation of the process switching mechanism in operating systems. This was my project in "Operating Systems" course.

Simulation of the process switching mechanism with custom instruction set. The context of the processes was saved enabling processes to resume execution from the last saved state.

Usage:
1. Open bash and type in the commands specified below.
2. These commands should be typed without double quotes.
    
    gcc -pthread -o "executable_name" launchMain.c <br/>
    ./"executable_name"
    
Results:
Based on the option chosen by you during the execution of "launchMain.c", logs will be stored in in 2 different files.
1. Implementation with threads -> logs_rr_with_thread
2. Implementation without threads -> logs_rr_without_thread
