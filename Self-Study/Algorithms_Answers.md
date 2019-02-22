Add your answers to the Algorithms exercises here.

Exercise I -

a) This snippet has essentially three different blocks of code to consider as we think about running time. They are as follows:

a = 0
while (a < n \* n \* n)
a = a + n \* n

The first line of code will run exactly once, so it's complexity is O(1).
The second line of code is also going to run once, which means it is also complexity O(1).
For the third line of code, it helps me to actually see what is happening as the code is run. This is a loop that will be run multiple times depending on the input. The loop stops as soon as (a) is bigger than (n \* n \* n).

For example:
n=1, loop runs once; n=2, loop runs twice...etc. This is showing itself to be a linear complexity, O(N), giving the entire snippet a time complexity of O(N).
