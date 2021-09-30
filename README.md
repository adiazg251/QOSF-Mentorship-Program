# QOSF Mentorship Program
QC Mentorship Program - Task 1

## Task 1
Design a quantum circuit that considers as input the following vector of integers numbers: 

[1,5,7,10]

and returns a quantum state which is a superposition of indices of the target solution, obtaining in the output the indices of the inputs where two adjacent bits will always have different values. In this case the output should be: 1/sqrt(2) * (|01> + |11>) , as the correct indices are 1 and 3.

    1 = 0001
    5 = 0101
    7 = 0111
    10 = 1010
   
The method to follow for this task is to start from an array of integers as input, pass them to a binary representation and you need to find those integers whose binary representation is such that two adjacent bits are different. Once you have found those integers, you must output a superposition of states where each state is a binary representation of the indices of those integers.

The solution is presented in three files:

    Task1 : main solution of the problem, with n=2 and m=4, with input vector [1,5,7,10]
    
    Task1_variation1: shows how the program can easily be changed to m=5, with new input vector [10,3,21,28]  (needs to have 10 and 21; the other two elements are arbitrary)
    
    Task1_variation2: shows how the program runs when input state is prepared just as superposition of input states: 1/2(|0001> + |0101> + |0111> + |1010>) 
