#### Please add your answers to the ***Analysis of  Algorithms*** exercises here.

## Exercise I

a)
O(n^c) => Polynomial, because the while loop contains n^3 as condition

b)
O(n log n) => Linearithmic. he first loop leads to at least O(n) complexity, as it adds one more execution for n + 1. The loop with the j*=2 condition is sub linear as j grows faster than n. In total the complexity therefore is linearithmic

c)
O(n) => Linear. This function is of linear complexity because for each n+1 one more recursive function call is made. E.g. n=4 => 5 function calls, n=1 => 2 function calls.

## Exercise II
Break as few eggs as possible: 
Repeat until floor value is determined:
    Drop egg from highest unproven floor. Assume all floors above a breaking floor as breaking aswell.
        If the floor was the highest possible floor and egg doesn't break end the function. 
    if egg breaks: Drop egg from floor/2 floor.
    If egg doesn't break: Drop egg from floor between non breaking floor and the next higher breaking floor.
    If there is no middle floor left, end function

    This has logarithmic complexity as fewer than n steps are required as the number of possibilities for f are halved on each execution of the loop.

