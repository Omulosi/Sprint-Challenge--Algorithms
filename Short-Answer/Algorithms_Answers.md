#### Please add your answers to the ***Analysis of  Algorithms*** exercises here.

## Exercise I

a)

Running time: O(n**3)

The size of the input, n, is raised to the 3rd every time, hence there are at
least n**3 executions within the loop for every input n.


b)

Running time: O(n**2)

There are two loops. The maximum possible iteration for each loop is n.
This gives a total of n * n for the worst case scenario.

The function runs in constant time as there are no deferred calculations which
would take up memory.

Memory: O(1)


c)

The running time is equal to the number of bunnies supplied to the function.
i.e for n bunnies, the running time is O(n).

However , the memory used is not constant - it's proportional to the number of
bunnies, n, supplied to the function. i.e O(n)

## Exercise II

min_sum = 0
# f -> max floor to be determined, n -> total floors in the storey
f = 0 # set start floor to be initially zero
max_floor = None

while f >= 0:
    dropped_broken_eggs = broken + dropped
    if dropped_broken_eggs < min_sum:
        min_sum = dropped_broken_eggs
        max_floor = f
    f = n // 2 
return max_floor

Running time: O(log(n))
-> The search is halved through each iteration till the minimum sum of dropped
and broken eggs is found
