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

b) This snippet has six blocks of code that will determine runtime complexity:

sum = 0
for i in range(n): i += 1
for j in range(i + 1, n): j += 1
for k in range(j + 1, n): k += 1
for l in range(k + 1, 10 + k): l += 1
sum += 1

The first and the last blocks of code will run exactly once, meaning their complexity is O(1). The other blocks of code are increasing as the input increases, which means that they are linear - O(N). Because we are dealing with nested iterations over the data set, together they become O(N^4).

c) This is a recursive function. The base case is bunnies == 0, so we look at time complexity as we move towards the base case. The number of bunnies decreases every time the function loops, which would indicate to me that there is a linear complexity of O(N).
