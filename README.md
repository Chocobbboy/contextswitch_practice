# Context-Switching
A multithreaded simulation of the process switching mechanism in operating systems. This was my project in "Operating Systems" course.

A custom instruction set was used for simulation which consisted of some simple operations. The context of the processes consists of the value of variables which are saved in the 'variables.txt' file. This allows the processes to resume from last instruction executed with value of variables intact.

### Description of files:
<strong>1. opcode.txt</strong> - Each line contains the operation code and its integer representation separated by a space.<br>
<strong>2. variables.txt</strong> - Each line contains the name of the variable and its current value.<br>
<strong>3. processes/filein_(1/2/3/4/5).txt</strong> - Each file contains instructions and this file denotes a process. <br><br>
Each process contains a set of instructions with the format as: <strong> opcode operand1 operand2 result_variable </strong>

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
