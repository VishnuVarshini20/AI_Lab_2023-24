# Ex.No: 5   Logic Programming – Factorial of number   
### DATE : 08.04.25
### REGISTER NUMBER : 212223060306
### AIM: 
To  write  a logic program for finding the factorial of given number using SWI-PROLOG. 
### Algorithm:
1. STEP 1: Start the program
2. STEP 2:  Write a rules for finding factorial of given program in SWI-PROLOG.
3.   a)	factorial of 0 is 1 => written as factorial(0,1).
4.   b)	factorial of number greater than 0 obtained by recursively calling the factorial    function.
5. STEP 3: Run the program  to find answer of  query.
6. STEP 4: Stop the program.

### Program:
```
fact(N,Res):-
    N>1,
    N1 is N-1,
    fact(N1,Res1),
    Res is N*Res1.
fact(0,1).
fact(1,1).

```
### Output:

![Screenshot 2025-04-08 111329](https://github.com/user-attachments/assets/5079ed49-6c2d-4a18-8e76-3cadc7182f4e)

### Result:
Thus the factorial of given number was found by logic programming. 
