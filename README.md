# Context-Switching
A multithreaded simulation of the process switching mechanism in operating systems. This was my project in "Operating Systems" course.

Simulation of the process switching mechanism with custom instruction set. The context of the processes was saved enabling processes to resume execution from the last saved state.

### Description of files:
1. opcode.txt - Each line contains the operation code and is integer representation separated by a space.
2. variables.txt - Each line contains the name of the variable and its current value.
3. processes/filein_(1/2/3/4/5).txt - Each file contains a set of instructions. <br />
The instruction format is as follows: <br />
opcode operand1 operand2 result_variable

# Results
Based on the option chosen by you during the execution of "launchMain.c", logs will be stored in in 2 different files.
1. Implementation with threads -> logs_rr_with_thread
2. Implementation without threads -> logs_rr_without_thread

# Usage
1. Open bash and type the commands specified below: <br/>
        gcc -pthread -o "executable_name" launchMain.c <br/>
        ./"executable_name"
    
<strong>Note:</strong> Recent execution of the code has revealed some peculiarities. The code runs on Ubuntu 16.04 but not on Ubuntu 18.04. Based on a preliminary search, it seems that this is caused due to the gcc compatibility issue with Ubuntu 18.04, primarily because of some changes in the 'newlib' library. You can read more about the bug here: [Github issues](https://github.com/travisgoodspeed/md380tools/issues/871) | [Launchpad Bug page](https://bugs.launchpad.net/gcc-arm-embedded/+bug/1772332)

For more information about the project, please refer to the document 'OS_Project_Context_Switching.pdf'.
