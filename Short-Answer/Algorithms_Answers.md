#### Please add your answers to the ***Analysis of  Algorithms*** exercises here.

## Exercise I

a) The run time is O(n) linear
    a is increasing by n*n for each run through the while loop
    since it is increasing by (n*n) it will no longer be less than 
    n*n*n after n times. This is (n*n) * n 

b) The run time is O(n*.5n) exponential
    As n increases the number of iterations of the while loop will increase by 1
    In addition, the length of each while loop will increase by 1 every other
    increase in n


c) The run time is O(n) linear
    as bunnies increases by 1 the code will go through one additional level of
    recursion

## Exercise II

Since dropped eggs and broken eggs are treated equally it is important to minimize the total number of drops.

The best way to do this would be to treat it similar to a binary search and continue until you have two consecutive floors where the egg is undamaged and then broken. 

You would check the floor that is halfway up the n-story building. If the egg breaks then you would then repeat this process on the lower half of the building and if it doesn't break on the upper half of the building. The algorithm would continue like this recursively and stop when both the next floor to check is one floor away than the current floor and they have different values for if the egg breaks or not.

The run time complexity of this would be O(log n) since it does not need to 
test for each value of n
