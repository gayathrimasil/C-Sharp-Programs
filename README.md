Question 1:

Given an array A consisting of N integers, returns the maximum among all one-digit integers
For exampl, given array A as follows: [-6, -91, 1011, -100, 84, -22, 0, 1, 473], the function should return 1.




Question 2:

A word machine is a system that performs a sequence of simple operations on a stack of integers. Initially the stack is empty. The sequence of operations is given as a string. Operations are seperated by single spaces. The following operations may be specified:

an integer X(from 0 to 2 power 20 -1): the machine pushes X onto the stack;
"POP" the machine removes the topmost number from the stack
"DUP" the machine pushes a duplicate of the topmost number onto the stack
"+" the machine pops the two topmost elements from the stack, adds them together and pushes the sum onto the stack
"-" the machine pops the two topmost elements from the stack, subtract the second one from the first (topmost) one and pushes the difference onto the stack.
After processing all the operations, the machine returns the topmost value from the stack.

The machine processes 20-bit unsigned integers (numbers from 0 to 2 power 20-1). An overflow in addition or underflow in the subtraction causes an error. The machine also reports an error when it tries to perform an operation that expects more numbers on the stack than the stack actually contains. Also, if after performing all the operations, the stack is empty, the machine reports an error.

Examples:

Given S =" 4 5 6 - 7 +", the function should return 8
Given S=" 13 DUP 4 POP 5 DUP + DUP + -", the function should return 7
Given S="5 6 + -", the function should return -1
Given S="3 DUP 5 - -", the function should return -1
Given S="1048575 DUP +", the function should return -1
