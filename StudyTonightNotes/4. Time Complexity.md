# Time Complexity of Algorithms

For any defined problem. there can be N number of solutions. This is true in general. 
If I have a problem and I discuss about the problem with all of my freinds, they will 
all suggest me different solutions. And I am the one who has to decide which solution 
is the best based on the circumstances.

Similaroty for any problem which must be solved using a program, there can be infinite
number of solutions. Let's take a simple example to understand this. Below we have two different 
algorithms to find the square of a number (for some time, forget that square of any number n is n x n):

One solution to this problem can be, running a loop for n times, starting with the number n and adding n to it,
every time. 

```
/* 
    we have to calculate the square of n
*/
for i=1 to n
    do n = n + n
// when the loop ends n will hold its square
return n
```
