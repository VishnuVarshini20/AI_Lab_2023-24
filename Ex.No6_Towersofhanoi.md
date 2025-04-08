# Ex.No: 6   Logic Programming – Factorial of number   
### DATE: 08.04.25                                                                           
### REGISTER NUMBER : 212223060306
### AIM: 
To  write  a logic program  to solve Towers of Hanoi problem  using SWI-PROLOG. 
### Algorithm:
1. Start the program
2.  Write a rules for finding solution of Towers of Hanoi in SWI-PROLOG.
3.  a )	If only one disk  => Move disk from X to Y.
4.  b)	If Number of disk greater than 0 then
5.        i)	Move  N-1 disks from X to Z.
6.        ii)	Move  Nth disk from X to Y
7.        iii)	Move  N-1 disks from Y to X.
8. Run the program  to find answer of  query.

### Program:
```
move(0, _, _, _).  
move(N, Source, Destination, Auxiliary) :-
    N > 0,
    M is N - 1,
    move(M, Source, Auxiliary, Destination),
    
    write('Move disk '), write(N), write(' from '), write(Source), write(' to '), write(Destination), nl,
    
    move(M, Auxiliary, Destination, Source).
```
### Output:

![Screenshot 2025-04-08 113117](https://github.com/user-attachments/assets/ab86dcee-1890-496a-b304-ba223b88deba)

### Result:
Thus the solution of Towers of Hanoi problem was found by logic programming.
