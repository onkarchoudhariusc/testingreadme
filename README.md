
# HW1 EE538
## University of Southern California
## Instructor: Arash Saifhashemi

Please clone this repository, edit README.md to answer the questions, and fill up functions to finish the homework.

- Please find each question in a separate folder under [files](/files).
- For non-coding questions, fill out the answers in the README file.
- For coding questions, edit the files and check them in.
- For coding questions unless specified, you should add unit tests to the student_test.cc.
  We will clone and test your repo using your tests and some other tests (that are not provided). Your code should pass all of them.
- For submission, please push your answers to Github before the deadline.
- Rubrics:
  
| Question | Points |
| -------- | ------ |
| 1        | 18     |
| 2        | 18     |
| 3        | 18     |
| 4        | 18     |
| 5        | 18     |
| 6        | 18     |
| 7        | 18     |

- Total: 126 points. 100 points is considered full credit.


See [cpp-template](https://github.com/ourarash/cpp-template) for help on installing bazel and debugging.

# Question
- Please refer to [files](/files).
- For each question, implement and test it in the [files](/files).
- Write the runtime complexity of each question in this README file.

# Answers
Runtime complexities - 
- Q1.A. Reverse vector function  
  Time Complexity: O(n)  
  Justification: For reversing the vector we need to traverse the entire vector, thus O(n).

- Q1.B. PlusOne function   
  Time Complexity: O(n)  
  Justification: In the worst case we need to check all the elements of vector are valid or not resulting into O(n). Then, let us say number is 999, adding 1 to it results into changing every element of the vector, resulting into O(n). Thus, overall complexity is O(n).

- Q2. IsPrime function  
  Time Complexity: O(sqrt(n))
  Justification: As the for loop iterates only from i=2 to sqrt(n), the time complexity is O(sqrt(n)).

- Q3. CountNumberOfSpaces function  
  Time Complexity: O(n)  
  Justification: As the for loop iterates over all the characters of the string to see whether it is space or not, the time complexity is O(n)

- Q4. Flatten3DVector function  
  Time Complexity: O(n^3)  
  Justification: In this we have 3 nested for loops. The iteration is over all three dimensions of the 3D vector. If the 3D vector is of mxnxp dimensions, the total computations will be product of m, n, and p. Thus the time complexity is O(mnp) = O(n^3)

- Q5. ClimbStairs function  
  Time Complexity: O(n)  
  Justification: Here, we are storing the number of ways (say for a step number x) x-1, x-2, x-3 steps in a vector. Thus, we are not computing it every time, we are using the stored values. We do these computations till we reach nth step, thus time complexity is O(n).

- Q6. Calculator function  
  Time Complexity: O(1)  
  Justification: This function only performs addition, subtraction, multiplication, checking dividebyzero and then dviding if nonzero denominator. All these tasks require constant time, thus O(1).

- Q7. CanBecome function  
  Time Complexity: O(n^2)  
  Justification: In the worst case, comparison will happen for (n-1), (n-2), (n-3), ..., 3, 2, 1 times. 
  "(n-1) + (n-2) + (n-3) + ... + 2 + 1" summation results into O(n^2) time complexity.
